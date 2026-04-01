---
layout: post
title: PostgreSQL 每周新闻 2026-4-1
---
### PostgreSQL每周新闻#642 - 2026年4月1日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/642)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/lyjxqudhjidan4ihgpuy.jpg)

## [pg_textsearch 1.0: 使用 Postgres 页面的 BM25 搜索引擎](https://postgresweekly.com/link/183105/rss)

基于 C 语言构建的真正 [BM25 评分](https://postgresweekly.com/link/183106/rss)，运行在 Postgres 自身的存储层之上，因此您可以创建索引、编写查询并获得相关性排序的结果。v1.0 版本从预览版升级到生产版本，支持并行索引构建和基于磁盘的段（而不是 1.0 之前仅基于内存）。[GitHub 仓库](https://postgresweekly.com/link/183107/rss)。

Todd J. Green (Tiger Data)


💡 还有其他基于 BM25 的选项可用，包括 [ParadeDB](https://postgresweekly.com/link/183108/rss)（在幕后使用 [Tantivy](https://postgresweekly.com/link/183109/rss)）和 [VectorChord-BM25](https://postgresweekly.com/link/183110/rss)。很期待看到它们之间的对比和基准测试。

## [大多数团队在 Postgres 上进行分析时会遇到瓶颈](https://postgresweekly.com/link/183104/rss)

Postgres 可以扩展分析能力，只需要一些帮助。与其使用第二个数据库，不如添加 TimescaleDB：hypertables、95% 压缩率和连续聚合。无需管道、无同步延迟、无漂移。基于实时数据的分析。免费开始构建。

Tiger Data (creators of TimescaleDB) 赞助商

## [Postgres 中的高内存使用率实际上是好事](https://postgresweekly.com/link/183111/rss)

Postgres 中的高内存*使用率*通常是系统正在执行其工作的标志，将频繁访问的数据保持在近处。需要担心的是*内存压力*，Simeon 解释了如何区分这两者。

Simeon Griggs (PlanetScale)


**本周摘要：**

- 🇦🇹 Microsoft 的 Cornelia Biacsics 讲述了[她如何在上周在维也纳组织 Postgres 聚会](https://postgresweekly.com/link/183112/rss)的故事。如果您想在自己的城市做同样的事情，这可能会给您带来启发。

- Amazon Aurora PostgreSQL [现已在 AWS 免费套餐上提供](https://postgresweekly.com/link/183113/rss)。

- ♟️ 您能[使用 SQL 渲染国际象棋棋盘](https://postgresweekly.com/link/183114/rss)并移动棋子吗？一个关于实现方法的有趣的交互式探索。

## [Postgres 19 通过 `COPY` 添加内置 JSON 导出功能](https://postgresweekly.com/link/183115/rss)

在下一个版本的 Postgres 中，`COPY ... TO ... WITH JSON` 将允许您将查询结果或表数据直接导出为 JSON 对象流。

Hubert Lubaczewski


## [`pg_service.conf`：您的团队忘记学习的法术](https://postgresweekly.com/link/183116/rss)

[`pg_service.conf`](https://postgresweekly.com/link/183117/rss) 有点像 `ssh` 的 `config` 文件，它允许您将连接参数捆绑到单个服务名称中，这样您就可以执行像 `psql service=prod` 这样的操作。一个更巧妙的技巧是为每个环境设置不同的文件，并在它们之间切换，同时保持逻辑名称不变。

Lætitia Avrot


## [随机 I/O 的真实成本](https://postgresweekly.com/link/183118/rss)

在 25 年后，`random_page_cost` 默认值 4.0 是否仍然正确？Vondra 在闪存存储上使用直接 I/O 进行受控实验，发现答案比*"只需将其设置为 1.0"*更加微妙。

Tomas Vondra


📄 [`plan_cache_mode` 的隐藏行为](https://postgresweekly.com/link/183119/rss) – 您知道查询规划器可以在多次执行后更改预准备语句的执行计划吗？ *Richard Yen*

📄 [2026 年数据库模式迁移方法综述](https://postgresweekly.com/link/183120/rss) *Jeremy Schneider*

▶️ [如何在 Go 和 Postgres 中实现 Outbox 模式](https://postgresweekly.com/link/183121/rss) *Package Main*


## 分类广告：

在用户发现之前发现 N+1 查询。AppSignal 通过实时警报自动监控 Postgres 性能。[免费试用](https://postgresweekly.com/link/183122/rss)。

👾 一个为进行了大重写并活着讲述故事的工程师举办的会议。[BugBash](https://postgresweekly.com/link/183123/rss) 2026，4月23-24日，华盛顿特区。


## 🛠 代码和工具

## [pgmetrics: 从运行中的 Postgres 服务器收集和报告统计信息](https://postgresweekly.com/link/183124/rss)

一个 Go 应用程序（因此无需依赖项），可收集超过 350 种不同的指标并生成[像这样的报告](https://postgresweekly.com/link/183125/rss)。除了一目了然非常有用外，该格式也非常适合 LLM 分析。

RapidLoop


## [`pg_regresql`: 真正可移植的 Postgres 统计信息](https://postgresweekly.com/link/183126/rss)

一个扩展，强制规划器使用 `pg_class` 统计信息而不是读取实际文件大小，这样注入的生产统计信息在小型开发/测试数据库中可以完整保留。

Radim Marek


## [Multigres Operator: 用于 Multigres 的 Kubernetes Operator](https://postgresweekly.com/link/183127/rss)

[Multigres](https://postgresweekly.com/link/183128/rss) 是一个受 Vitess 启发的水平可扩展/分片 Postgres 架构，这个 operator 将其引入 Kubernetes。请注意*"目前它还没有达到生产就绪状态，但我们进展迅速 - 预计几个月后就能就绪。"*

Supabase


- [pg_ivm 1.14](https://postgresweekly.com/link/183129/rss) – 使用增量变更使物化视图保持最新。

- [pgschema 1.8](https://postgresweekly.com/link/183130/rss) – 用于 Postgres 的 Terraform 风格声明式模式迁移。

- [pg-boss 12.15.0](https://postgresweekly.com/link/183131/rss) – 基于 Postgres 的 Node.js 应用程序作业队列。