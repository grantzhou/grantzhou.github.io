---
layout: post
title: PostgreSQL 每周新闻 2026-6-3
---
### PostgreSQL每周新闻#651 - 2026年6月3日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/651)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/k4fty4cyhoq9abd75kbb.jpg)

## [在 Postgres 19 中使用 `SQL/PGQ` 处理图数据](https://postgresweekly.com/link/186020/rss)

Postgres 19 将添加对 SQL/PGQ 的支持，因此您可以在表上声明属性图，并使用类似 Cypher 的 `MATCH (a IS person)-[IS knows]->(b IS person)` 查询进行模式匹配。这一切都由查询*重写器*处理，因此图模式会变成普通的关系查询。

**Hans-Jürgen Schönig**

💡 想在*当前*的 Postgres 上使用图查询？Elizabeth Garrett Christensen [展示了 Apache AGE 扩展如何](https://postgresweekly.com/link/186021/rss)将 openCypher 引入当前版本。


## [存储减少 95%。分析速度提升 40%。CERN 在 Postgres 上的实践](https://postgresweekly.com/link/186019/rss)

CERN 的大型强子对撞机每天产生数百 GB 的时间序列数据。在这场现场网络研讨会中，他们的工程师将演示如何使用 TimescaleDB 现代化传统归档堆栈。6 月 25 日，美国东部时间上午 9 点。

**Tiger Data (TimescaleDB 的创建者)** 赞助商


## [🔓 为什么 Postgres 缺少透明数据加密](https://postgresweekly.com/link/186022/rss)

许多其他数据库都有这个功能，但在 Postgres 中，您需要依赖第三方服务或 [pg-tde](https://postgresweekly.com/link/186023/rss) 扩展。为什么？Shaun 深入研究了关于该功能的旧讨论，发现最大的问题是定义 TDE 实际需要解决的*问题*是什么。

**Shaun Thomas**


**本周摘要：**

- [Postgres 19 Beta 1 已在官方仓库中标记](https://postgresweekly.com/link/186024/rss)，由 Tom Lane 完成。目前还没有太多内容可看，但 beta 公告似乎即将发布。

- Microsoft 已将其用于 Postgres 的 VS Code 扩展[在 Open VSX 注册表上发布](https://postgresweekly.com/link/186025/rss)（VS Code 兼容编辑器的独立扩展商店），因此 Cursor 等工具现在可以直接使用它。

- ClickHouse 托管的 Postgres [现已进入 beta 阶段](https://postgresweekly.com/link/186026/rss)。


## [帮助规划器帮助您](https://postgresweekly.com/link/186027/rss)

当两列相关时，Postgres 假设它们是独立的，规划器的行估计会严重出错。这是对 `CREATE STATISTICS` 及其带来的更好查询计划的实用教程。

**Valerie Parham-Thompson**


## [数据出口问题及如何找到它们](https://postgresweekly.com/link/186028/rss)

如果您的数据库运行在别人的数据中心，数据出口和相关成本的控制就很重要。Simeon 分享了如何降低数字的技巧，以及一些 PlanetScale 特定的建议。

**Simeon Griggs (PlanetScale)**

📄 [我们的表无法停止增长的那个夜晚](https://postgresweekly.com/link/186029/rss) – 生产环境的侦探故事：一个游离的 `statement_timeout` 悄悄地破坏了逻辑复制，导致表膨胀。*Semab Tariq*

📄 [不是 Postgres Bug 的 Postgres 故障](https://postgresweekly.com/link/186030/rss) – 三个表现为数据库故障的操作系统级故障。*Payal Singh*

📄 [相同查询，三种结果](https://postgresweekly.com/link/186031/rss) – 一个查询，三次基准测试，ParadeDB 和 Postgres FTS 之间的三个非常不同的结论。关于方法如何影响答案的教训。*James Blackwood-Sewell (ParadeDB)*

📄 [函数何时是 `LEAKPROOF` 的？](https://postgresweekly.com/link/186032/rss) *Laurenz Albe*


## 分类广告：

发现 N+1 查询，比您的用户更早。[AppSignal](https://postgresweekly.com/link/186033/rss) 通过实时警报自动监控 Postgres 性能。[免费试用](https://postgresweekly.com/link/186033/rss)。

🔎 [介绍 pg_search](https://postgresweekly.com/link/186034/rss)，这是一个 Postgres 扩展，可在 Postgres 中实现 Elasticsearch 质量的全文、向量和混合搜索。

🐘 [Spock 5.0.7](https://postgresweekly.com/link/186035/rss)：PG18 slotsync 集成，add-node 数据竞争修复，apply-worker 恢复。[开源多主 Postgres](https://postgresweekly.com/link/186035/rss)。


## 🛠 代码和工具

## [DeltaX (δx)：适用于 Postgres 的快速时间序列扩展](https://postgresweekly.com/link/186036/rss)

来自 Xata 的新型列式存储扩展，用于时间序列数据，仅使用常规 Postgres 表，因此复制、崩溃恢复、备份和 `pg_dump` 等功能可以像往常一样工作。这里是[它的工作原理](https://postgresweekly.com/link/186037/rss)。

**Xata**


## [Streambed：将 Postgres 流式传输到 S3 上的 Iceberg](https://postgresweekly.com/link/186038/rss)

通过逻辑复制流式传输 WAL，将 Parquet 写入 S3，并提交 Iceberg 元数据。然后您可以使用普通的 `psql` 进行查询，这要归功于内置的 wire-protocol 服务器。

**viggy28**


## [ingestr v1：一条命令在数据库之间复制数据](https://postgresweekly.com/link/186039/rss)

一个由 Go 驱动的工具，可在[众多来源和目标](https://postgresweekly.com/link/186040/rss)之间移动数据（包括 Postgres），支持增量追加/合并，无需编写代码。

**Bruin Data**

- 🔎 [pg_textsearch 1.3](https://postgresweekly.com/link/186041/rss) – Tiger Data 的扩展，用于 BM25 相关性排名的全文搜索。v1.3 包括与分解存储架构兼容的修订。

- [SeaQuery 1.0](https://postgresweekly.com/link/186042/rss) – Rust 中用于 Postgres/MySQL/SQLite 的动态查询构建器。


## 📺 最后一件事 — 值得一看：

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/ytbhvkeve9um151a8cmw.jpg)

## [Postgres 30 周年：与创始人的对话](https://postgresweekly.com/link/186043/rss)

随着 Postgres 今年迎来 30 周年，这里有个惊喜：与启动 Postgres 项目的 Mike Stonebraker 的广泛访谈。他介绍了 Postgres 的诞生过程，他认为 Google 和 Amazon 在数据库方面的错误之处，以及他下一步要构建的东西。

**The Peterman Pod**

💡 更喜欢阅读？这里也有[完整文字稿](https://postgresweekly.com/link/186044/rss)。