---
layout: post
title: PostgreSQL 每周新闻 2024-10-2
---
### PostgreSQL每周新闻#572 - 2024年10月2日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/572)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/kwfnttiwnfhqxipayqji.jpg)
## [Postgres 17 有什么优点？](https://postgresweekly.com/link/160512/web)
Postgres 17 终于发布了，我们开始看到一些对其众多增强功能的看法。Laurenz 在这里介绍了引起他注意的内容。

`Laurenz Albe`
## [您适合在 SQL 中使用 NULL 吗？](https://postgresweekly.com/link/160514/web)
一个有趣的测验，旨在测试您对 NULL 行为的直觉以及它如何与其他类型、谓词、聚合等交互。这真是一个令人费解的问题。（注意：至少我的 Postgres 的行为与最后一个问题的预期答案不同，这表明这一切是多么令人困惑。）


`AgentM `
## [以一半的成本将 GitHub Actions 运行速度提高 2 倍](https://postgresweekly.com/link/160511/web)
Blacksmith 通过在现代游戏 CPU 上运行 GitHub Actions 来显著提高运行速度。集成 Blacksmith 只需更改一行代码。Ashby、Superblocks 和 Slope 等 100 多家公司使用 Blacksmith 帮助开发人员更快地合并代码。


`Blacksmith  `
## [▶ Heroku 的辉煌岁月和 Postgres 与世界的较量](https://postgresweekly.com/link/160515/web)
Postgres 传奇人物 Craig Kerstiens 与 Aaron Francis（正在研究即将推出的 Mastering Postgres 课程）一起谈论他在 Heroku、Citus Data 和现在的 Crunchy Data 与 Postgres 的历史。不过，这不仅仅是关于他；采访中充满了关于构建生态系统、扩展 Postgres 甚至 DuckDB 的见解。


`Aaron Francis `
## [▶ Postgres 17 中的 SQL IN 子句速度提高了很多](https://postgresweekly.com/link/160517/web)
Hussein 对 PG17 在使用 IN 时对 b 树扫描性能的增强感到非常惊讶，因此他录制了一个截屏视频，解释其工作原理，将其与 SQL Server 的方法进行比较，并通过现场演示进行展示。


`Hussein Nasser`

### 本周摘要：

* [DBA Vasilis Ventirozos](https://postgresweekly.com/link/160518/web) 是本周 PostgreSQL 人物的受访者。上周，受访者是[OVHcloud 的 Nicolas Payart](https://postgresweekly.com/link/160519/web)。

* 🎤 本周，[Postgres.fm](https://postgresweekly.com/link/160520/web) 播客开始[讨论 Postgres 17](https://postgresweekly.com/link/160521/web)。

* 🇮🇳 Pavlo Golub 分享了他在 [2024 年海得拉巴 PGDay 上的经历](https://postgresweekly.com/link/160522/web)。


## [等待 Postgres 18：添加时间 PRIMARY KEY 和 UNIQUE 约束](https://postgresweekly.com/link/160523/web) 
Postgres 17 可能刚刚推出，但 Hubert 正在展望 Postgres 18，以及一种在某个时间段内强制唯一性的新方法，比如使用 WITHOUT OVERLAPS 而不仅仅是针对静态值。


`Hubert depesz Lubaczewski`
## [探索 Postgres 的极限：何时突破？](https://postgresweekly.com/link/160524/web)
Postgres 的极限在纸面上很容易理解，但在现实世界中，你能将单节点 Postgres 服务器推到多远，瓶颈在哪里？


`Andrew Atkinson`


📄 [使用 Go 中的 pgx 和 sqlc 更轻松地编写原始 SQL](https://postgresweekly.com/link/160525/web) - remvn

📄 [在现代 Mac 上将 Homebrew Postgres 16 升级到 17](https://postgresweekly.com/link/160526/web) - Ian van der Linde

📄 [构建 AI 图像库：使用 pgvector 和 Claude Sonnet 的高级 RAG](https://postgresweekly.com/link/160527/web)- Haziqa Sajid（Timescale）


### 📰 分类广告

明智地选择 PostgreSQL 数据类型可以为您节省时间和避免日后的麻烦。参加 10 月 8 日的 [Redgate 现场网络研讨会](https://postgresweekly.com/link/160528/web)，了解如何操作。

在 Postgres 上构建 AI 应用程序？[pgai 为开发人员提供 AI 超能力](https://postgresweekly.com/link/160617/web)，支持集成 AI 工作流以执行嵌入创建和模型完成等任务。


### 🛠 代码和工具

## [pg_stat_kcache：收集有关磁盘访问和 CPU 消耗的统计数据](https://postgresweekly.com/link/160529/web)
位于 pg_stat_statements 之上并创建视图，您可以使用它们来测量 CPU 时间、页面错误、交换、读取和写入的字节数以及数据库和查询级别的更多内容。


`Dalibo and PoWA Team`
## [pgsql-tweaks：一套有用的 Postgres 函数](https://postgresweekly.com/link/160532/web)
一套有趣的函数，作者（前 PostgreSQL 本周人物）在作为 Postgres 用户的日常工作中使用，涵盖检查数据类型、收集统计数据、一些聚合和转换函数等领域。


`Powa Team`

[pg_qualstats：用于收集谓词统计数据的扩展](https://postgresweekly.com/link/160433/web)
分析针对数据库的查询中最常用的谓词，或许可以作为创建更有效索引的一种方法。POWA（Postgres 工作负载分析器）项目的一部分。


`Dan Lynch`


[pg_idkit 0.2.4](https://postgresweekly.com/link/160534/web)– 用于生成 UUID 和类似 ID 的扩展。

[Pongo 0.15](https://postgresweekly.com/link/160535/web) – 用于 Node.js 的 Postgres 驱动程序，以 MongoDB 样式 API 的形式呈现。

[node-pg-migrate 7.7](https://postgresweekly.com/link/160536/web) – 从 Node.js 进行数据库迁移管理。

[pgwire 0.25](https://postgresweekly.com/link/160537/web) – 在 Rust 库中实现的 Postgres 线路协议。

[DoltgreSQL 0.12](https://postgresweekly.com/link/160538/web) – 版本控制的 Postgres-a-like。

[pspg 5.8.7](https://postgresweekly.com/link/160539/web) – 用于表格数据的 Unix 终端寻呼机。