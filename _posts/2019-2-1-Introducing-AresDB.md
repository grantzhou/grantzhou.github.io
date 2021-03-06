---
layout: post
title: AresDB介绍：Uber基于GPU的开源实时分析引擎
---

By Jian Shen, Ze Wang, David Wang, Jeremy Shi, and Steven Chen

链接：https://eng.uber.com/aresdb/

![aresdb img](https://eng.uber.com/wp-content/uploads/2019/01/Featured-1-1068x457.png)


在优步，实时分析使我们能够获得业务洞察力和运营效率，使我们能够制定数据驱动的决策，以改善优步平台的体验。
例如，我们的运营团队依靠数据来监控市场健康状况并发现我们平台上的潜在问题; 由机器学习模型驱动的软件利用数据来预测骑车者的供应和驾驶员需求; 数据科学家使用数据来改进机器学习模型，以便更好地进行预测。

过去，我们使用了许多第三方数据库解决方案进行实时分析，但没有一个能够同时满足我们的所有功能，可扩展性，性能，成本和运营要求。

AresDB于2018年11月发布，是一个开源的实时分析引擎，利用非常规的处理能力：图形处理单元（GPU），使我们的分析能够大规模增长。 GPU技术是一种新兴的实时分析工具，多年来发展迅速，非常适合并行实时计算和数据处理。

在接下来的部分中，我们将介绍AresDB的设计以及这种功能强大的实时分析解决方案如何使我们能够更加全面，高效地统一，简化和改进优步的实时分析数据库解决方案。 阅读本文后，我们希望您为自己的项目尝试AresDB，并找到有助于您自己的分析需求的工具！


## 优步的实时分析应用程序
数据分析对优步业务的成功至关重要。 在其他功能中，这些分析用于：
- 构建仪表板以监控我们的业务指标
- 根据我们收集的汇总指标做出自动决策（例如[旅行定价](https://www.uber.com/drive/partner-app/how-surge-works/)和[欺诈检测](https://eng.uber.com/advanced-technologies-detecting-preventing-fraud-uber/)）
- 进行即席查询以诊断和解决业务运营问题

<style>
table {
  border-collapse: collapse;
  width: 100%;
}

table, th, td {
  border: 1px solid black;
  text-align: left;
  padding: 8px;
}

tr:nth-child(even) {background-color: #f2f2f2;}
</style>

|---| 仪表板Dashboard | 决策系统Decision Systems | 即席查询 Ad Hoc Queries |
|:---:|:---:|:---:|:---:|
| **查询模式** | 已知 | 已知 | 随意 |
| **查询QPS** | 高 | 高 | 低 |
| **查询延迟** | 低 | 低 | 高 |
| **数据集** | 子集 | 子集 | 全部数据 |

仪表板和决策系统利用实时分析系统，在高QPS和低延迟的情况下，通过相对较小但非常有价值的数据子集（具有最大数据新鲜度）进行类似查询。

## 另一个分析引擎的必要性

实时分析在优步解决的最常见问题是如何计算时间序列聚合，计算使我们能够洞察用户体验，从而相应地改进我们的服务。
通过这些计算，我们可以在任意过滤（或有时加入）数据的时间范围内按特定维度（例如日，小时，城市ID和旅行状态）请求指标。
多年来，优步已经部署了多种解决方案，以不同的方式解决这个问题。

我们用于解决此类问题的一些第三方解决方案包括：
- **[Apache Pinot](https://github.com/apache/incubator-pinot)** 是一个用Java编写的开源分布式分析数据库，可用于大规模数据分析。 Pinot在内部使用lambda架构来查询柱状存储中的批处理和实时数据，使用反转位图索引进行过滤，并依赖星形树进行聚合结果缓存。但是，它不支持基于密钥的重复数据删除，upsert，联接和高级查询功能，例如地理空间过滤。此外，作为基于JVM的数据库，Pinot上的查询执行在内存使用方面以更高的成本运行。
- **[Elasticsearch](https://www.elastic.co/)** 优步在内部使用Elasticsearch来满足各种流分析需求。它建立在Apache [Lucene](http://lucene.apache.org/)上，用于存储文档和反向索引的全文关键字搜索。它已被广泛采用并扩展到也支持聚合。反向索引允许过滤，但它没有针对基于时间范围的存储和过滤进行优化。它将记录存储为JSON文档，从而增加了额外的存储和查询访问开销。与Pinot一样，Elasticsearch是一个基于JVM的数据库，因此不支持连接，并且其查询执行以更高的内存成本运行。

虽然这些技术具有自己的优势，但它们缺乏我们用例的关键功能。 我们需要一个统一，简化和优化的解决方案，并且开箱即用（或者更确切地说，在GPU内部）以实现解决方案。

## 利用GPU进行实时分析
为了以高帧速率渲染图像的逼真视图，GPU高速并行处理大量几何和像素。 虽然处理单元的时钟速率在过去几年中已经趋于稳定，但芯片上的晶体管数量仅根据摩尔定律增加。 因此，以千兆浮点每秒（GFLOP/s）为单位测量的GPU计算速度正在迅速增加。 下面的图1描述了多年来比较NVIDIA GPU和Intel CPU的理论GFLOP/s趋势：
![pic 1](https://eng.uber.com/wp-content/uploads/2019/01/image11-2-1068x559.png)

*图1：多年来CPU和GPU单精度浮点性能的比较。 图片取自Nvidia的CUDA C编程指南。*

在设计我们的实时分析查询引擎时，集成GPU处理非常适合。 在优步，典型的实时分析查询处理数天到数十亿条记录的数天数据，然后在短时间内过滤和汇总它们。 此计算任务非常适合通用GPU的并行处理模型，因为它们：


- 高速并行处理数据。
- 提供更高的计算吞吐量（GFLOPS/s），使其非常适合可以并行化的繁重计算任务（每单位数据）。
- 与中央处理单元（CPU）相比，提供更高的计算到存储（ALU到GPU全局内存）数据访问吞吐量（而不是延迟），使其成为处理需要大量数据的I/O（内存）绑定并行任务的理想选择。

一旦我们决定使用基于GPU的分析数据库，我们评估了一些利用GPU满足我们需求的现有分析解决方案：
- [Kinetica](https://www.kinetica.com/) Kinetica是一个基于GPU的分析引擎，最初于2009年向美国军事和情报应用程序推广。虽然它展示了GPU技术在分析方面的巨大潜力，但我们发现我们的用例缺少许多关键功能，包括架构更改，部分插入或更新，数据压缩，列级内存/磁盘保留配置以及地理空间关系的连接。
- [OmniSci](https://www.omnisci.com/) OmniSci是一个开源的，基于SQL的查询引擎，似乎是一个很有前途的选择，但在我们评估产品时，我们意识到它没有Uber用例的关键功能，例如重复数据删除。虽然OminiSci在2017年开放了他们的项目，但在对他们基于C++的解决方案进行了一些分析之后，我们得出的结论是，无论是贡献还是创建代码库分支都不可行。
- 基于GPU的实时分析引擎，包括[GPUQP](https://www.cse.ust.hk/gpuqp/)，[CoGaDB](http://cogadb.dfki.de/)，[GPUDB](http://www.vldb.org/pvldb/vol6/p817-yuan.pdf)，[Ocelot](http://www.vldb.org/pvldb/vol6/p709-heimel.pdf)，[OmniDB](http://www.vldb.org/pvldb/vol6/p1374-he.pdf)和[Virginian](https://github.com/bakks/virginian)，经常被学术机构使用。然而，鉴于其学术目的，这些解决方案专注于开发算法和设计概念证明，而不是处理现实世界的生产场景。出于这个原因，我们为我们的范围和规模打了折扣。

总的来说，这些引擎展示了使用GPU技术进行数据处理的巨大优势和潜力，它们激励我们构建我们自己的基于GPU的实时分析解决方案，以满足优步的需求。 考虑到这些概念，我们构建并开源了AresDB。

## AresDB架构概述
从大方面来讲，AresDB将其大部分数据存储在主机内存（连接到CPU的RAM）中，使用CPU处理数据摄取和通过磁盘恢复数据。 在查询时，AresDB将数据从主机内存传输到GPU内存，以便在GPU上进行并行处理。 如下面的图2所示，AresDB由内存存储，元数据存储和磁盘存储组成：
![pic 2](https://eng.uber.com/wp-content/uploads/2019/01/image20-1068x605.png)

*图2：AresDB单实例体系结构具有内存和磁盘存储以及元存储。*

### 表 Tables
与大多数关系数据库管理系统（RDBMS）不同，AresDB中没有数据库或模式范围。 所有表都属于同一AresDB集群/实例中的相同作用域，使用户可以直接引用它们。 用户将其数据存储为事实表和维度表。
### 事实表 Fact Table
事实表存储无限的时间序列事件流。 用户使用事实表来存储实时发生的事件/事实，并且每个事件都与事件时间相关联，表通常由事件时间查询。 事实表存储的信息类型的一个例子是旅行，其中每次旅行是一个事件，旅行请求时间通常被指定为事件时间。 如果事件具有与之关联的多个时间戳，则只有一个时间戳被指定为事实表中显示的事件的时间。
### 维度表 Dimension table
维度表存储实体（包括城市，客户和驱动程序）的当前属性。 例如，用户可以在维度表中存储城市信息，例如城市名称，时区和国家/地区。 与随时间无限增长的事实表相比，维度表总是受大小限制（例如，对于Uber，城市表以世界上实际的城市数量为界）。 维度表不需要特殊的时间列。

### 数据类型
下表详细介绍了AresDB中支持的当前数据类型：

| 数据类型 | 字节长度 | 详细内容 |
| :---: | :---: | :---: |
| Bool | 1/8 |	布尔类型数据，存储为一个 位/bit |
| Int8, Uint8  | 	1	||
| Int16, Uint16  | 	2 | 整数类型。 用户可以根据字段的基数和内存成本进行选择。|
| Int32, Uint32 | 	4 ||
| SmallEnum	 | 1	|Strings 会自动翻译成枚举。 SmallEnum可以保存String类型，最大256|
| BigEnum | 	2	| 类似SmallEnum,但是可以最大到65535|
| Float32 | 	4	| 浮点数。 我们支持Float32，并打算根据需要添加Float64支持|
| UUID	 | 16	| 通用唯一标识符|
| GeoPoint | 	4	| 地理点 Geographic points |
| GeoShape | 	|可变长度多边形或多边形 |

使用AresDB，字符串在进入数据库之前会自动转换为枚举类型（enums），以提高存储和查询效率。 这允许区分大小写的相等性检查，但不支持连接，子串，全局和正则表达式匹配等高级操作。 我们打算在将来添加完整的字符串支持。

### 主要特点
AresDB的架构支持以下功能：
- 基于列的存储，具有压缩功能，可实现存储效率（在存储数据的字节数方面的内存使用量更少）和查询效率（在查询期间从CPU内存到GPU内存的数据传输更少）
- 使用主键重复数据删除实时升级，可在几秒钟内实现高数据准确性和接近实时的数据新鲜度
- GPU驱动的查询处理，用于GPU支持的高度并行化数据处理，提供低查询延迟（亚秒到秒）

## 列式存储
### 向量
AresDB以列式格式存储所有数据。 每列的值存储为列式值向量。 每列中值的有效性/无效性存储在单独的空向量中，每个值的有效性由一位表示。

### 实体存储
AresDB在实时存储中存储未压缩和未排序的列式数据（实时向量）。 实时存储中的数据记录被划分为（实时）批量配置容量。 在摄取时创建新批次，而在归档记录后清除旧批次。 主键索引用于查找重复数据删除和更新的记录。 下面的图3演示了我们如何组织实时记录并使用主键值来定位它们：
![pic 3](https://eng.uber.com/wp-content/uploads/2019/01/image23.png)

*图3：我们使用主键值来定位每个记录的批次和批次位置。*

批次中每列的值存储为列式矢量。 每个值向量中的值的有效性/无效性被存储为单独的空向量，每个值的有效性由一位表示。 在下面的图4中，我们提供了一个包含city_id列的五个值的示例：
![pic 4](https://eng.uber.com/wp-content/uploads/2019/01/image3-4-e1548709370771-1068x783.png)
*图4：我们为数据表中的未压缩列存储值（实际值）和空向量（有效性）。*

### 归档存储
AresDB还通过事实表将成熟，排序和压缩的列式数据（存档向量）存储在存档存储中。 归档存储中的记录也分为批次。 与实时批处理不同，存档批处理包含特定世界时协调（UTC）日的记录。 存档批处理使用自Unix Epoch以来的天数作为其批处理ID。

记录按照用户配置的列排序顺序进行排序。 如下面的图5所示，我们首先按city_id列排序，然后是状态列：
![pic 5](https://eng.uber.com/wp-content/uploads/2019/01/image16-1-e1548709469337-1055x420.png)

*图5：我们按行所有行排序bycity_id，然后是status，然后使用行程编码压缩每列。 每个列在排序和压缩后都有一个计数向量。*

配置用户配置的列排序顺序的目标是：

- 通过先前对低基数列进行排序来最大化压缩效果。 最大化压缩可提高存储效率（存储数据所需的字节数更少）和查询效率（从CPU传输到GPU内存的字节更少）。
- 允许对常见的等效过滤器进行基于范围的廉价预过滤，例如city_id = 12。 预过滤使我们能够最小化从CPU内存传输到GPU内存所需的字节数，从而最大限度地提高查询效率。

仅当列出现在用户配置的排序顺序中时才会压缩列。 我们不会尝试压缩高基数列，因为压缩高基数列所节省的存储量可以忽略不计。

排序后，使用行程编码的变体压缩每个限定列的数据。 除了值向量和空向量之外，我们还引入了计数向量来表示相同值的重复。

## 使用upsert支持实时提取
客户端通过发布upsert批处理通过摄取HTTP API来提取数据。 upsert批处理是一种自定义的序列化二进制格式，可最大限度地减少空间开销，同时仍可随意访问数据。

当AresDB收到一个用于摄取的upsert批处理时，它首先将upsert批处理写入重做日志以进行恢复。 将upsert批处理附加到重做日志的末尾后，AresDB会识别并跳过事实表上的延迟记录，以便提取到实时存储中。 如果记录的事件时间早于存档的截止事件时间，则该记录被视为“迟到”。 对于不被视为“迟到”的记录，AresDB使用主键索引在应用于应用程序的实时存储中查找批处理。 如下面的图6所示，全新记录（以前未见过的基于主键值）将应用于空白区域，而现有记录将直接更新：
![pic 6](https://eng.uber.com/wp-content/uploads/2019/01/image10-2.png)

*图6：在摄取期间，在将upsert批处理附加到重做日志之后，“late”记录将附加到回填队列，而其他记录将应用于实时存储。*

## 存档
在摄取时，记录将在实时存储中追加/更新，或者附加到等待放入存档存储的回填队列中。

我们会定期在实时存储记录上运行一个称为归档的计划流程，以将新记录（之前从未存档过的记录）合并到归档存储中。 归档仅处理实时存储中的记录，其事件时间落入旧截止时间（上次归档过程的截止时间）和新截止时间（新的截止时间基于 表模式中的存档延迟设置）。

记录的事件时间将用于确定记录应合并到哪个归档批次中，因为我们将归档数据批量转换为每日批次。 归档在合并期间不需要主键值索引重复数据删除，因为只会存档旧截止和新截止范围之间的记录。

下面的图7描述了基于给定记录的事件时间的时间线：

![pic 7](https://eng.uber.com/wp-content/uploads/2019/01/image14.png)

*图7：我们使用事件时间和截止时间来确定哪些记录是新的（实时）和旧的（事件时间早于归档截止）。*

在此方案中，归档间隔是两次归档运行之间的时间，而归档延迟是事件时间之后但在归档事件之前的持续时间。 两者都在AresDB的表模式配置中定义

## 回填Backfill
如上面的图7所示，事实表的旧记录（事件时间早于归档截止）将附加到回填队列，最终由回填过程处理。 此过程也由回填队列的时间或大小触发，达到其阈值。 与实时存储的提取相比，回填是异步的，并且在CPU和内存资源方面相对更昂贵。 回填用于以下场景：
- 处理偶尔很晚到达
- 手动修复上游的历史数据
- 填充最近添加的列的历史数据
- 与归档不同，回填是幂等的，需要基于主键值的重复数据删除。 回填的数据最终将对查询可见。

回填队列在内存中以预先配置的大小维护，并且在大规模回填加载期间，客户端将在回填运行清除队列之前被阻止继续。

## 查询处理
使用当前实现，用户将需要使用由Uber创建的Ares查询语言（AQL）来对AresDB运行查询。 AQL是一种有效的时间序列分析查询语言，并不像其他类SQL语言那样遵循SELECT FROM WHERE GROUP BY的标准SQL语法。 相反，AQL在结构化字段中指定，可以使用JSON，YAML和Go对象携带。 例如，代替`SELECT count（*）FROM trip GROUP BY city_id WHERE status ='completed' AND request_at >= 1512000000`，JSON中的等效AQL写为：

<pre><code>
{
 “table”: “trips”,
 “dimensions”: [
   {“sqlExpression”: “city_id”}
 ],
 “measures”: [
   {“sqlExpression”: “count(*)”}
 ],
;”>  “rowFilters”: [
   “status = ‘completed'”
 ],
 “timeFilter”: {
   “column”: “request_at”,
   “from”: “2 days ago”
 }
}
</code></pre>

在JSON格式中，AQL为仪表板和决策系统开发人员提供了比SQL更好的编程查询体验，因为它允许他们使用代码轻松编写和操作查询，而无需担心SQL注入等问题。 它作为Web浏览器，前端服务器和后端服务器的典型架构的通用查询格式，一直回到数据库（AresDB）。 此外，AQL提供方便的语法糖，用于时间过滤和bucketization，具有本机时区支持。 该语言还支持隐式子查询等功能，以避免常见的查询错误，并使后端开发人员可以轻松进行查询分析和重写。

尽管AQL提供了各种好处，但我们完全清楚大多数工程师更熟悉SQL。 公开SQL接口进行查询是我们为了增强AresDB用户体验而采取的后续步骤之一。

我们在下面的图8中描述了AQL查询执行流程：
![pic 8](https://eng.uber.com/wp-content/uploads/2019/01/image19.png)

*<center>图8：AresDB的查询执行流程利用我们自己开发的AQL查询语言进行快速，高效的数据处理和检索。</center>*

### 查询编译
AQL查询被编译到内部查询上下文中。 过滤器，维度和度量中的表达式被解析为抽象语法树（AST），以便稍后通过GPU进行处理。

### 数据馈送
AresDB利用预过滤器在将存档数据发送到GPU进行并行处理之前对其进行廉价过滤。 由于归档数据是根据配置的列顺序排序的，因此某些过滤器可能能够通过应用二进制搜索来定位相应的匹配范围来利用此排序顺序。 特别是，所有第一个X排序列上的等效过滤器和排序X + 1列上的可选范围过滤器可以作为预过滤器处理，如下面的图9所示：
![pic sort](https://eng.uber.com/wp-content/uploads/2019/01/image13-2.png)

*图9：AresDB在将列式数据发送到GPU进行处理之前对其进行预过滤。*


在预先过滤之后，仅需要将绿色值（满足过滤条件）推送到GPU以进行并行处理。 输入数据被送到到GPU并一次一批地执行。 这包括实时批次和归档批次。

AresDB利用[CUDA流](https://devblogs.nvidia.com/gpu-pro-tip-cuda-7-streams-simplify-concurrency/)进行流水线数据提供和执行。 在每个查询上交替使用两个流以在两个重叠阶段中进行处理。 在下面的图10中，我们提供了此过程的时间表说明：
![pic 10](https://eng.uber.com/wp-content/uploads/2019/01/image8-2.png)

*<center>图10：使用AresDB，两个CUDA流交替进行数据传输和处理。</center>*

## 查询执行

为简单起见，AresDB利用[Thrust库](https://developer.nvidia.com/thrust)来实现查询执行过程，该过程提供了精细调整的并行算法构建块，以便在当前查询引擎中快速实现。

在Thrust中，使用随机访问迭代器访问输入和输出向量数据。 每个GPU线程寻找输入迭代器到其工作负载位置，读取值并执行计算，然后将结果写入输出迭代器上的相应位置。

AresDB遵循每个内核的一个运算符（OOPK）模型来评估表达式。

下面的图11演示了一个示例AST的过程，它是在查询编译阶段通过维度表达式`request_at  -  request_at％86400`生成的：

![pic 11](https://eng.uber.com/wp-content/uploads/2019/01/image7-1.png)

*<center>图11：AresDB利用OOPK模型模型进行表达式评估。</center>*

在OOPK模型中，AresDB查询引擎遍历AST树的每个叶节点并返回其父节点的迭代器。 如果根节点也是叶子，则直接在输入迭代器上执行根操作。

在每个非根非叶节点（在该示例中为[模运算](https://en.wikipedia.org/wiki/Modulo_operation)），分配临时临时空间向量以存储从`request_at％86400`表达式产生的中间结果。 利用Thrust，启动内核函数来计算GPU上此运算符的输出。 结果存储在临时空间迭代器中。

在根节点处，以与非根非叶节点相同的方式启动内核函数。 根据表达式类型采取不同的输出操作，详述如下：
- 过滤动作以减少输入向量的基数
- 将维度输出写入维度向量以供以后聚合
- 将度量输出写入度量向量以供以后聚合

在表达评估之后，执行排序和减少以进行最终聚合。 在排序和缩减操作中，我们使用维度向量的值作为排序和缩减的关键值，并使用度量向量的值作为要聚合的值。 通过这种方式，具有相同维度值的行将组合在一起并进行聚合。 下面的图12描述了这种分类和减少过程：

![pic 12](https://eng.uber.com/wp-content/uploads/2019/01/image22.png)

*图12：在表达式评估之后，AresDB按维度（键值）和度量（值）向量上的键值对数据进行排序和减少。*


AresDB还支持以下高级查询功能：
- Join：目前AresDB支持从事实表到维度表的散列连接
- Hyperloglog基数估计：AresDB实现Hyperloglog算法
- Geo Intersect：当前AresDB仅支持GeoPoint和GeoShape之间的交叉操作

## 资源管理
作为基于内存的数据库，AresDB需要管理以下类型的内存使用：
| --- | 分配 | 管理模式 |
| --- | --- | --- |
| 实时存储矢量（实时存储列式数据）| C |	Tracked| 
| 存档存储矢量（存档存储列数据）| C |管理（负载和驱逐）Managed (Load and eviction) |
| 主键索引（记录重复数据删除的哈希表）| C |	Tracked |
| 回填队列（存储“迟到”数据等待回填）| Golang | Tracked |
| 归档/回填过程临时存储（归档和回填过程中分配的临时内存） | C |	Tracked |
| 摄取/查询临时存储; |
| 流程开销; | Golang和C | 静态配置估计 |
| 分配碎片 | | |

当AresDB投入生产时，它会利用配置的总内存预算。 此预算由所有六种内存类型共享，并且还应为操作系统和其他进程留出足够的空间。 此预算还包括静态配置的开销估计，服务器监控的实时数据存储以及服务器可根据剩余内存预算决定加载和驱逐的归档数据。

下面的图13描绘了AresDB主机内存模型：

![pic 13](https://eng.uber.com/wp-content/uploads/2019/01/image12-2.png)

*图13：AresDB管理自己的内存使用情况，使其不超过配置的总进程预算。*

AresDB允许用户在事实表的列级别配置预加载日期和优先级，并且仅在预加载日期内预加载存档数据。非预装数据按需从磁盘加载到内存中。一旦完成，AresDB还会从主机内存中驱逐归档数据。 AresDB的驱逐策略基于预加载天数，列优先级，批次日期和列大小。

AresDB还管理多个GPU设备并将设备资源建模为GPU线程和设备内存，跟踪GPU内存使用情况作为处理查询。 AresDB通过设备管理器管理GPU设备，设备管理器在两个维度（GPU线程和设备内存）中对GPU设备资源进行建模，并在处理查询时跟踪使用情况。在查询编译之后，AresDB使用户能够估计执行查询所需的资源量。在允许查询开始之前，必须满足设备内存要求;如果在任何设备上当时没有足够的内存，则查询必须等待才能运行。目前，AresDB可以同时在同一GPU设备上运行一个或多个查询，只要该设备满足所有资源要求即可。

在当前的实现中，AresDB不会将输入数据缓存在设备内存中，以便在多个查询中重用。 AresDB的目标是支持对实时不断更新且难以正确缓存的数据集的查询。我们打算在AresDB的未来迭代中实现数据缓存功能GPU内存，这一步骤将有助于优化查询性能。

## 使用案例：优步的摘要仪表板
在优步，我们使用AresDB构建仪表板，以提取实时业务洞察 （business insights）。 AresDB扮演着通过持续更新存储最新原始事件的角色，并使用低功耗的GPU功能在几秒钟内计算针对它们的关键指标，以便用户可以交互使用仪表板。 例如，在数据存储中具有较长周期的匿名旅行数据由多种服务更新，包括我们的调度，支付和评级系统。 为了有效地利用旅行数据，用户将数据切片并切成不同的维度，以获得实时决策的见解。

利用AresDB，Uber的摘要仪表板是一个广泛使用的分析仪表板，由公司各团队利用，以检索相关的产品指标并实时响应以改善用户体验。

![pic 14](https://eng.uber.com/wp-content/uploads/2019/01/image18.png)

*<center>图14：Uber Summary Dashboard的每小时视图使用AresDB查看特定时间段内的实时数据分析。</center>*

为了构建上面的模型仪表板，我们对以下表进行了建模：

### Trips（事实表）

| trip_id | request_at | city_id | status | driver_id | fare |
| --- | --- | --- | --- | --- | --- |
| 1 | 1542058870 |	1 |	completed |	2 |	8.5 |
| 2 |	1541977200 |	1 |	rejected  |	3 |	10.75 |
| ... | | | | | |

### Cities （维度表）

| city_id | city_name | timezone | 
| --- | --- | --- |
| 1	| San Francisco	| America/Los_Angeles |
| 2	| New York |	America/New_York |
| ... | | |

### AresDB中的表结构
要创建上述两个建模表，我们首先需要在AresDB中创建在以下结构的表：

<table>
  <tr>
    <td>Trips</td>
    <td>Cities</td>
  </tr>
  <tr><td>
  <pre><code>{
 “name”: “trips”,
 “columns”: [
   {
     “name”: “request_at”,
     “type”: “Uint32”,
   },
   {
     “name”: “trip_id”,
     “type”: “UUID”
   },
   {
     “name”: “city_id”,
     “type”: “Uint16”,
   },
   {
     “name”: “status”,
     “type”: “SmallEnum”,
   },
   {
     “name”: “driver_id”,
     “type”: “UUID”
   },
   {
     “name”: “fare”,
     “type”: “Float32”,
   }
 ],
 “primaryKeyColumns”: [
   1
 ],
 “isFactTable”: true,
 “config”: {
   “batchSize”: 2097152,
   “archivingDelayMinutes”: 1440,
   “archivingIntervalMinutes”: 180,
  “recordRetentionInDays”: 30
 },
 “archivingSortColumns”: [2,3]
} </code> </pre>
    </td> 
    <td>
      <pre><code> {
 “name”: “cities”,
 “columns”: [
 {
     “name”: “city_id”,
    “type”: “Uint16”,
   },
   {
     “name”: “city_name”,
     “type”: “SmallEnum”
   },
   {
     “name”: “timezone”,
     “type”: “SmallEnum”,
   }
 ],
 “primaryKeyColumns”: [
   0
 ],
 “isFactTable”: false,
 “config”: {
   “batchSize”: 2097152
 }
}</code> </pre></td>
</tr>
</table>

如模式中所述，trips表被创建为事实表，表示实时发生的行程事件，而cities表被创建为维度表，存储有关实际城市的信息。

创建表后，用户可以利用[AresDB客户端库](https://github.com/uber/aresdb/blob/master/client/connector.go#L48)从事件总线（如Apache [Kafka](https://kafka.apache.org/)）或流式或批处理平台（如Apache [Flink](https://flink.apache.org/)或Apache [Spark\(https://spark.apache.org/)）中提取数据。

### 针对AresDB的查询示例
在模型仪表板中，我们选择两个指标作为示例，总行程票价和活动驾驶员。 在仪表板中，用户可以过滤城市的指标，例如, 旧金山。 要绘制仪表板中显示的过去24小时这两个指标的时间序列，我们可以在AQL中运行以下查询：

| 过去24小时内旧金山的总旅行费用按小时计算 | 过去24小时内旧金山的活跃司机小时数 |
| --- | --- |
| ```{
 “table”: “trips”,
 “joins”: [
   {
     “alias”: “cities”,
     “name”: “cities”,
     “conditions”: [
       “cities.id = trips.city_id”
     ]
   }
 ],
 “dimensions”: [
   {
     “sqlExpression”: “request_at”,
     “timeBucketizer”: “hour”
   }
 ],
 “measures”: [
   {
     “sqlExpression”: “sum(fare)”
   }
 ],
 “rowFilters”: [
   “status = ‘completed'”,
   “cities.city_name = ‘San Francisco'”
 ],
 “timeFilter”: {
   “column”: “request_at”,
   “from”: “24 hours ago”
 },
 “timezone”: “America/Los_Angeles”
}``` | ``` {
 “table”: “trips”,
 “joins”: [
   {
     “alias”: “cities”,
     “name”: “cities”,
     “conditions”: [
       “cities.id = trips.city_id”
     ]
   }
 ],
 “dimensions”: [
   {
     “sqlExpression”: “request_at”,
     “timeBucketizer”: “hour”
   }
 ],
 “measures”: [
   {
     “sqlExpression”: “countDistinctHLL(driver_id)”
   }
 ],
 “rowFilters”: [
   “status = ‘completed'”,
   “cities.city_name = ‘San Francisco'”
 ],
 “timeFilter”: {
   “column”: “request_at”,
   “from”: “24 hours ago”
 },
 “timezone”: “America/Los_Angeles”
} |

###  查询的结果示例：

上述模拟查询将在以下时间序列结果中生成结果，可以很容易地将其绘制到时间序列图中，如下所示：

| 过去24小时内旧金山的总旅行费用按小时计算 | 过去24小时内旧金山的活跃司机小时数 |
| --- | --- |
| ```{
 “results”: [
   {
     “1547060400”: 1000.0,
     “1547064000”: 1000.0,
     “1547067600”: 1000.0,
     “1547071200”: 1000.0,
     “1547074800”: 1000.0,
     … 
   }
 ]
}``` | ``` {
 “results”: [
   {
     “1547060400”: 100,
     “1547064000”: 100,
     “1547067600”: 100,
     “1547071200”: 100,
     “1547074800”: 100,
    …  
   }
 ]
} ``` |

在上面的示例中，我们演示了如何利用AresDB在几秒钟内实时摄取实时发生的原始事件，并立即针对数据发出任意用户查询，以便在亚秒内计算指标。 AresDB可帮助工程师轻松构建数据产品，从而提取对企业至关重要的指标，这些指标需要对人员或机器决策提供实时洞察。


## 下一步
AresDB在优步广泛使用，为我们的实时数据分析仪表板提供支持，使我们能够针对业务的各个方面大规模地制定数据驱动的决策。通过开源这个工具，我们希望社区中的其他人可以利用AresDB进行自己的分析。

在未来，我们打算通过以下功能来增强项目：

- 分布式设计：我们正在构建AresDB的分布式设计，包括复制，分片管理和模式管理，以提高其可扩展性并降低运营成本。
- 开发人员支持和工具：自2018年11月开源AresDB以来，我们一直致力于构建更直观的工具，重构代码结构，丰富文档以改善入职体验，使开发人员能够快速将AresDB集成到他们的分析堆栈中。
- 扩展功能集：我们还计划扩展我们的查询功能集，以包括窗口函数和嵌套循环连接等功能，从而允许该工具支持更多用例。
- 查询引擎优化：我们还将研究开发更高级的方法来优化查询性能，例如低级虚拟机（LLVM）和GPU内存缓存。

AresDB是根据Apache许可证[开源](https://github.com/uber/aresdb)的。我们鼓励您试用AresDB并加入我们的社区。

*如果构建大规模的实时数据分析技术，请考虑申请我们团队的角色。*


## 致谢

特别感谢Kate Zhang，Jennifer Anderson，Nikhil Joshi，Abhi Khune，Shengyue Ji，Chinmay Soman，Xiang Fu，David Chen和Li Ning让这个项目取得了圆满成功！












