---
layout: post
title: PostgreSQL 每周新闻 2024-4-24
---
### PostgreSQL每周新闻#552 - 2024年4月24日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/552)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/eptvqhqvvax5evxaxp2q.jpg)
## [PDF：MySQL 的未来是 Postgres](https://postgresweekly.com/link/154132/web)
这个幻灯片的标题确实引起了我的注意！ 这是上周在 Postgres Conference 2024 上发表的演讲的幻灯片。 一位演讲者在这里解释了这一切。 他们正在开发 Postgres 扩展，以使 MySQL 应用程序能够在 Postgres 上运行，而无需更改任何代码（因此它将支持有线协议、SQL 方言等）。预计今年夏天将发布 alpha 版本。


`Jonah Harris and Mason Sharp `
## [电子书：调整 Autovacuum 以获得最佳 Postgres 性能](https://postgresweekly.com/link/154131/web)
了解调整调度和性能设置、减少工作时间的 autovacuum 开销、xmin 范围及其阻止真空、为什么要避免反环绕真空以及如何通过调整死元组来减少膨胀 阈值。


`pganalyze `
## [PGXN v2 的架构](https://postgresweekly.com/link/154135/web)
David Wheeler 和其他人正在对 PGXN 方法进行重大更新，以便为 Postgres 生态系统提供扩展分发、发现和工具。 这个新的维基页面概述了当前的情况以及下一步的发展方向。


`The PostgreSQL Wiki `

**本周摘要：**

*   [PGDay UK](https://postgresweekly.com/link/154137/web) 宣布将于 [9 月 11 日在伦敦](https://postgresweekly.com/link/154138/web)回归。如果您想发言，他们的 CFP 也开放。


*   Microsoft 的 Claire Giordano 解释了年度虚拟 Postgres 会议 [POSETTE 的演讲选择流程](https://postgresweekly.com/link/154140/web)。 他们收到了 184 份谈话提案，但只能接受 38 份，所以还有很多工作要做。


## [创建多租户队列](https://postgresweekly.com/link/154141/web)
在 Postgres 上启动一个基本队列相当容易，但是如果您不希望某个用户的工作成为众人瞩目的焦点，那该怎么办呢？ 为每个用户设置单独的队列，使其更加公平。


`Alexander Belanger `

📄 [PostgreSQL 社区辩论 ALTER SYSTEM](https://postgresweekly.com/link/154142/web) - JONATHAN CORBET 

📄 [如何使用 PERCENTILE_CONT 计算百分位数](https://postgresweekly.com/link/154143/web) - VLAD MIHALCEA

📄 [10 个 psql 命令，让您的生活更轻松](https://postgresweekly.com/link/154144/web) - JAMES BLACKWOOD-SEWELL（Timescale）

📄 [通过 Reshape 进行复杂的零停机模式迁移](https://postgresweekly.com/link/154146/web) – FABIAN LINDFORS

📄 [在 Postgres 上操作矢量数据库](https://postgresweekly.com/link/154147/web) - ADAM HENDEL (TEMBO)

📄 [Postgres 中的模糊字符串匹配](https://postgresweekly.com/link/154148/web) - PAUL RAMSEY


**📰 机密：**


🗓️ [预留 POSETTE 的日期](https://postgresweekly.com/link/154149/web)：Postgres 的免费虚拟开发者活动（6 月 11 日至 13 日）。 加入 4 个独特直播中的 44 位演讲者，聆听 PG 专家的演讲。 时间表已于 5 月 1 日发布。

🪝 [Hookdeck](https://postgresweekly.com/link/154150/web)：用于事件驱动应用程序的无服务器队列。 [了解更多](https://postgresweekly.com/link/154150/web)。

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/tvtuulraerdgp0odk66n.jpg)

## [pgddl / ddlx：DDL EXtractor 函数](https://postgresweekly.com/link/154151/web)
纯 SQL 扩展，可以为系统目录/表模式等创建 SQL DDL（例如 CREATE TABLE），因为使用 pg_dump 并不适合所有场景。


`Alexi Theodore `
## [ParadeDB：基于 Postgres 的 Elasticsearch 替代方案](https://postgresweekly.com/link/154152/web)
采用常见的“云产品 + 开源项目”方法，ParadeDB 提供 AGPL 许可（此处为存储库）的方式来加速 Postgres 的搜索和分析工作。


`Retake, Inc. `
## [pgvector-remote：一个用于处理远程向量的 pgvector fork](https://postgresweekly.com/link/154154/web)
目前仅限 Pinecone。 有一篇[博客文章](https://postgresweekly.com/link/154155/web)介绍了这个想法。


`Georgia Tech Database Group `
## [node-pg-migrate 7.0：Postgres 的数据库迁移管理](https://postgresweekly.com/link/154156/web)
该项目的新维护者 Shinigami（也是 Vite 的核心维护者）进行了大量清理和重构。


`Salsita Software `

[PGlite 0.1.5](9https://postgresweekly.com/link/154157/web) – 轻量级 Postgres 作为 WASM 打包到浏览器、Node.js、Bun 和 Deno 的 TypeScript 库。

[Goose 3.20](https://postgresweekly.com/link/154158/web) – 数据库迁移工具。 支持SQL和Go函数。

[pgxmock 3.4](https://postgresweekly.com/link/154159/web) – 用于测试 Go 中数据库交互的模拟驱动程序。

[pgrx 0.11.4](https://postgresweekly.com/link/154160/web) – 一种使用 Rust 构建 Postgres 扩展的方法。

[pgwire 0.21](https://postgresweekly.com/link/154161/web) – Rust 库中的 Postgres 线路协议。

[Slonik 41.1](https://postgresweekly.com/link/154162/web) – 具有类型安全性的 Node.js Postgres 客户端。

[pspg 5.8.5](https://postgresweekly.com/link/154163/web) – 用于表格数据的 Unix 终端寻呼机。
