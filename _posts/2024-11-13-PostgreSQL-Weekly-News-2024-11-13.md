---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-11-13
---
### PostgreSQL每周新闻#577 - 2024年11月13日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/577)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/stfg0zxgqan7cak1j1vp.jpg)
## [pgvector 0.8.0 发布](https://postgresweekly.com/link/162180/web)
Postgres 网站上有一篇关于这个流行的矢量索引和查询扩展版本的文章，但我喜欢这篇文章，因为它深入探讨了索引扫描的变化。使用 0.8，我们获得了改进的性能、对迭代索引扫描的支持以及将数组转换为 sparsevec 的方法。

`Gwen Shapira (Nile)`
## [▶ PostgreSQL 2024 年欧洲会议演讲](https://postgresweekly.com/link/162182/web)
上个月，欧洲年度 Postgres 会议在雅典圆满落幕，目前有多达 60 个视频可供欣赏。我们还没有时间浏览这些视频，但会在即将出版的期刊中介绍一些。


`PostgreSQL Conference `
💡 如果你想从某个地方开始观看，Claire Giordano 的《[Postgres 主要版本中有什么？](https://postgresweekly.com/link/162183/web)》和 Lætitia Avrot 的《[解开 PostgreSQL 权限的网络](https://postgresweekly.com/link/162184/web)》都是亮点。

## [通过 Redgate 学习 PostgreSQL](https://postgresweekly.com/link/162179/web)
刚接触 PostgreSQL？查看 Redgate 的 PostgreSQL 学习资源中心，获取简单易懂的网络研讨会、操作方法文章和支持性社区论坛。通过向专家学习提示、技巧和最佳实践，提升您的技能并节省时间。


`Redgate Software  `
## [编写分析 SQL 查询的 8 个步骤](https://postgresweekly.com/link/162185/web)
如果您需要编写复杂的分析查询，请从小处着手并从头开始构建，以避免问题逐渐出现，Christopher 说，他有一个八步评估标准来做到这一点。


`Christopher Winslett`
## [理解 PL/pgSQL 函数中的波动性](https://postgresweekly.com/link/162186/web)
Deepak 分享了一个真实的例子，说明了理解可以为 PL/pgSQL 函数指定的不同级别的函数波动性的重要性。

`Deepak Mahto`

### 本周摘要：

🇪🇺 Jimmy Angelakos [分享了上个月在雅典举行的 PGConf.EU 2024 的最新进展](https://postgresweekly.com/link/162188/web)。

📄 我们最近推出了 [pgdoc.link](https://postgresweekly.com/link/162189/web)，这是一种跳转到 Postgres 文档中所需内容的绝妙新方法。Hubert 现在已将[系统视图添加到索引中](https://postgresweekly.com/link/162190/web)。

🇨🇿 [2025 年布拉格 PostgreSQL 开发者日](https://postgresweekly.com/link/162191/web)将于明年 1 月 28 日至 29 日在捷克布拉格举行，包括一天的常规会议和一天的研讨会。


## [Postgres 数据库设计中的文本标识符](https://postgresweekly.com/link/162192/web) 
如果您使用文本标识符（而不是数字或 UUID）来记录，则需要考虑各种事项。


`Radim Marek`
## [从备份到完整性：利用 WAL-G](https://postgresweekly.com/link/162193/web) 
进行备份是一回事，在出现硬件或网络问题时确保其完整性是另一回事，但可以使用校验和来检测完整性问题。


`Data Egret`


📄 [熟悉 psql](https://postgresweekly.com/link/162194/web) – 如果说有一款 Postgres 工具值得您全面掌握，那就是 psql。Craig 给出了一些入门级/初学者提示。Craig Kerstiens

📄 [等待 Postgres 18：array_reverse()](https://postgresweekly.com/link/162195/web) 函数 Hubert (depesz) Lubaczewski

📄 [触发 Postgres 中 Autovacuum 的场景](https://postgresweekly.com/link/162196/web) Semab Tariq

📄 [从 Oracle 过渡到 Postgres：索引](https://postgresweekly.com/link/162197/web) Umair Shahid


![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/ydnanymd2edqqwqw61lm.jpg)



## [PostgreSQL 工作负载分析器 (PoWA) 5.0 发布](https://postgresweekly.com/link/162198/web)
一种性能工具，用于从多个 Postgres 实例收集和聚合指标，然后可以通过实时图表查看这些指标并用于帮助优化您的设置。v5 具有大大改进的 Web UI，并提供比以前更多的数据源，包括 WAL 统计视图、IO 统计视图以及有关后台编写器和复制槽的信息。


`PoWA Team`


### 📰 分类广告

🌐 PostGIS 日是 11 月 21 日。加入我们的在线活动，了解开源地理空间工具和用例。[注册和演讲详情](https://postgresweekly.com/link/162199/web)。

您喜欢 Postgres，但您还有更多的爱要给予？[尝试使用 MongoDB 进行矢量搜索](https://postgresweekly.com/link/162200/web)。没人需要知道。


## [Schemalint：Postgres Schemas 的 Linter](https://postgresweekly.com/link/162201/web)
一款可让您针对各种常见问题（如名称大小写、强制 RLS 或强制列的存在）提出错误的 linter（因此，它更像是 ESLint，而不是基本格式化程序）。您还可以编写自己的自定义规则。

`Kristian Dupont`

[PGQueuer 0.15.0](https://postgresweekly.com/link/162203/web) – 使用 Postgres 进行高效作业排队的 Python 库。现在，您可以使用类似 cron 的语法安排重复作业。

[PGSync 3.3](https://postgresweekly.com/link/162204/web) – Postgres 到 Elasticsearch/OpenSearch 同步。

[DBMate 2.23](https://postgresweekly.com/link/162205/web) – 与框架无关、由 Go 提供支持的数据库迁移工具。

[pg_flo 0.0.9](https://postgresweekly.com/link/162206/web) – 实时流式传输、转换和路由 Postgres 数据。

[DoltgreSQL 0.14](https://postgresweekly.com/link/162207/web) – 版本控制的 Postgres 类似工具。