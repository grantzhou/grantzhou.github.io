---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 June 5, 2024
---
### PostgreSQL每周新闻#557 - 2024年6月5日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/557)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/gdejdtkucw4kksxfzdbo.jpg)

[为什么要升级Postgres？这就是为什么](https://postgresweekly.com/link/155919/web "why-upgrade.depesz.com") —
自从我们链接到这个方便资源已经过去两年多了，它让你选择“从”和“到”版本，并查看Postgres在此期间取得的进展。即使是从版本16升级到16.3的示例中，也充满了各种有趣的细节。

`Hubert depesz Lubaczewski`
  
  
⭐  [PostgreSQL 17 Beta 1 发布](https://postgresweekly.com/link/155920/web
"www.postgresql.org") — 上周我们休息的时候，时间不太充裕，因为在我们发送上一期之后，Postgres 17的第一个beta版本刚刚发布！尽管如此，这仍然是一个重大消息，而且这篇文章很好地总结了这里的新内容。

`PostgreSQL Global Development Group`
  
[![](https://copm.s3.amazonaws.com/f0e60e0d.png)](https://postgresweekly.com/link/155918/web)

[别错过POSETTE：一个关于Postgres的活动](https://postgresweekly.com/link/155918/web "www.addevent.com") —
[POSETTE](https://postgresweekly.com/link/155921/web) 快要来了！在6月11日至13日加入我们，参加POSETTE，这是最大规模的免费虚拟Postgres活动。活动将包括42场讲座，分布在4个直播流中，涵盖世界上最先进的开源数据库的各个方面。由微软的Postgres团队呈现。

`Microsoft sponsor`
  
  
💡 Claire Giordano 还编写了一份[关于POSETTE的精彩指南](https://postgresweekly.com/link/155922/web) 以及由整个Postgres社区的人士主持的各种讲座和下周即将举行的其他活动。  
  
  
[PGConf.dev有多引人入胜？真的很吸引人。](https://postgresweekly.com/link/155923/web "peter.eisentraut.org") —
PGConf.dev上周举行，[取得了巨大成功](https://postgresweekly.com/link/155924/web) 但它是否真正吸引了核心开发者？Peter发现它导致了20多年来核心提交的最长间断！

`Peter Eisentraut`  
  
  
[为什么我的`COMMIT`速度慢](https://postgresweekly.com/link/155925/web
"www.cybertec-postgresql.com") — 当涉及到提交事务时，越快越好。但是是什么原因导致它们变慢呢？

`Laurenz Albe`  
  
  
[使用Linux的cgroup2控制资源消耗](https://postgresweekly.com/link/155926/web "www.percona.com") —
控制组（cgroup）限制分配给进程的资源，并且也可以用于控制Postgres，特别是在“喧闹邻居”多租户场景中。

`Jobin Augustine`  
  
  
[外键中的循环依赖](https://postgresweekly.com/link/155927/web "www.cybertec-
postgresql.com") — A需要B，而B又需要A。噢哦！这样的循环依赖是如何发生的，以及如何解决？“INITIALLY DEFERRED”来拯救。

`Hans-Jürgen Schönig`  
  
  
[使用Rust创建自定义的Postgres扩展](https://postgresweekly.com/link/155928/web "notso.boringsql.com") —
[pgrx](https://postgresweekly.com/link/155929/web) 这（可能）是前进的方式，以下是一些入门指南。

`Radim Marek`  
  
  
[使用Postgres和pgvector构建一个RAG应用](https://postgresweekly.com/link/155930/web "www.enterprisedb.com") —
RAG (Retrieval Augmented Generation) 是一种增强大型语言模型输出的技术，它通过从其他数据集中检索上下文来增强查询。

`Gulcin Yildirim Jelinek (EDB)`  
  
  
📄 [将Postgres视为理所当](https://postgresweekly.com/link/155931/web) –
快速浏览Postgres中的预定义角色。 `Shaun M. Thomas`

📄 [在Ubuntu 24.04上使用Patroni设置高可用性的3节点Postgres集群](https://postgresweekly.com/link/155932/web) `Semab Tariq (Stormatics)`

📄 [Postgres中的数据加密：方法概述](https://postgresweekly.com/link/155933/web) `Greg Nokes (Crunchy Data)`

📄 [将DMS转换为PostGIS点几何](https://postgresweekly.com/link/155934/web) `Elizabeth Christensen (Crunchy Data)`

📄 [碳足迹和查询优化？](https://postgresweekly.com/link/155935/web) `Henrietta Dombrovskay` 
  
  
📰 Classifieds  
  
  
使用[Rocketadmin](https://postgresweekly.com/link/155936/web)从您的数据库结构创建一个管理面板. 无需编码。我们提供SAAS和自托管版本。

* * *

🔄 Local-first w/ Postgres:
[PowerSync](https://postgresweekly.com/link/155937/web) 使用逻辑复制仅将相关子集的数据同步到每个用户，确保一致性。

* * *

您通往生产的最快途径。[使用Render，您可以轻松构建、部署和扩展您的应用](https://postgresweekly.com/link/155938/web) – 从您的第一个用户到您的第十亿个用户。  
  
  
🛠 代码和工具
  
[![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/gjauwz1tjddw4adtpeh1.jpg)](https://postgresweekly.com/link/155939/web)  
  
[tbls：一个适用于CI的数据库文档工具](https://postgresweekly.com/link/155939/web "github.com") — 自动以Markdown格式记录数据库，通过DOT、PlantUML、Mermaid或直接生成图像渲染模式。默认情况下，您将获得包含列、索引、关系和其他模式细节的文档（这里是[一个示例](https://postgresweekly.com/link/155940/web)).

`Ken’ichiro Oyama`
  
  
[介绍pgCompare：一款多数据库比较工具](https://postgresweekly.com/link/155941/web "www.crunchydata.com") —
[pgCompare](https://postgresweekly.com/link/155942/web) 是一款来自Crunchy Data的开源工具。它设计用于在从不同来源复制数据后需要验证数据一致性时使用。

`Brian Pace (Crunchy Data)` 
  
  
[SQLFluff：一个针对“人类”的SQL语法检查工具](https://postgresweekly.com/link/155943/web "www.sqlfluff.com") —
使用Python构建的SQL语法检查工具，涵盖多种SQL方言（包括当然也包括Postgres）。

`Alan Cruickshank`  
  
  
📄 [快速了解两个用于PostGIS的终端工具](https://postgresweekly.com/link/155944/web) `Dian M Fay`
  
  
  * [QuestDB 8.0](https://postgresweekly.com/link/155945/web) – Java驱动的时间序列数据库，具有Postgres的协议兼容性。

  * [Bob 0.27](https://postgresweekly.com/link/155946/web) – 用于Go的SQL查询构建器和ORM/工厂生成器。

  * [pgxmock 4.0](https://postgresweekly.com/link/155947/web) – 用于在Go中测试数据库交互的模拟驱动。

  * [pgweb 0.16](https://postgresweekly.com/link/155948/web) – 跨平台的Postgres数据库客户端。

  * [Piccolo 1.7](https://postgresweekly.com/link/155949/web) – 用户友好的Python ORM和查询构建器。

  * [DoltgreSQL 0.8](https://postgresweekly.com/link/155950/web) – 类似于Postgres的版本控制数据库。

  * [pgvector 0.7.1](https://postgresweekly.com/link/155951/web)

  


# 💡本周提示


**🗓即将举办的Postgres活动**
