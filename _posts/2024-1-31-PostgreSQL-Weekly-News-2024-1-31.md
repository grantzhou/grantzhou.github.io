---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-1-31
---
### PostgreSQL每周新闻#540 - 2024年1月31日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/540)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/rmrxh02ntgmptq2xt5d3.jpg)
## [迈向理想的 Postgres 扩展生态系统](https://postgresweekly.com/link/150709/web)
Tembo 聘请了 PGXN 的创建者 David Wheeler 来负责 Postgres 扩展生态系统的工作，他已经开始分享他对事物的初步想法。 虽然有一些独立的尝试来聚合 Postgres 扩展（我们甚至自己做了一些），但 Postgres 可以从更官方、更权威的方法中受益吗？


`David Wheeler `
## [pgvector 0.6.0：现在通过并行索引构建速度提高约 30 倍](https://postgresweekly.com/link/150712/web)
pgvector 向量相似性搜索扩展可以说是当前的 Postgres 扩展，并且它在不断变得更好。 v0.6 引入了 HNSW 的并行索引构建，这对于重建可能覆盖数百万个向量的索引来说是一个巨大的胜利。


`Egor Romanov (Supabase) `
## [使用 Hasura 在 PostgreSQL 上提供即时实时 GraphQL API](https://postgresweekly.com/link/150708/web)
将 Hasura 连接到您的 PostgreSQL 数据库并获得安全且高性能的 GraphQL API。 通过过滤、排序、分页、聚合等查询表和视图。 通过订阅立即提取对数据的任何实时更改。


`Hasura `
## [DuckDB 的多数据库支持](https://postgresweekly.com/link/150714/web)
DuckDB 是一种 SQLite 式的进程内 DBMS，但专注于 OLAP 用例。 随着可插拔存储和事务层的引入，DuckDB 现在可以连接到 Postgres（或 MySQL 或 SQLite）数据库并使用它们。 这开启了一些有趣的用例，例如在不同数据库或格式（包括 Parquet）之间移动数据，所有这些都在 DuckDB 内进行。


`Mark Raasveldt (DuckDB) `

**本周摘要：**

*   🤖 [SQLCoder-70b-Alpha](https://postgresweekly.com/link/150716/web) 是 CodeLlama-70B LLM 的微调变体，旨在将自然语言查询转换为 SQL。 它甚至获得了许可，您可以将其用于商业用途。


*   无服务器 Postgres 平台 [Nile 已筹集 1160 万美元](https://postgresweekly.com/link/150717/web)，用于继续构建其无服务器 Postgres 平台，该平台目前仍处于内测阶段。


*   Robert Haas 按照惯例对过去一年中[谁为 Postgres 开发做出了贡献](https://postgresweekly.com/link/150718/web)进行了年度分析。 一如既往，Tom Lane 获得金牌！ 🥇


*   Bun JavaScript 运行时的创建者 Jarred Sumner 🐦 思考了[“Postgreslite”](https://postgresweekly.com/link/150721/web)的想法，本质上是 SQLite 和 Postgres 彼此更加兼容的梦想。


*   🐦 [Phil Eaton 已加入 EDB](https://postgresweekly.com/link/150722/web)，致力于开发他们的多主机分布式 Postgres 产品。


*   Lætitia Avrot 邀请您撰写有关 UUID 以及如何使用它们的[博客](https://postgresweekly.com/link/150723/web)（希望能与 Postgres 一起！）截止日期是本周五。


*   了解 Postgres 本周末将如何参加 [FOSDEM 2024](https://postgresweekly.com/link/150724/web)。 挺有趣的！


## [将 JSON 和 SVG 从 PostGIS 导入 Google Sheets](https://postgresweekly.com/link/150725/web)
使用 pg_featureserv 创建 JSON 和 pg_svg 直接从数据库创建 SVG 图像以输入电子表格的演练。


`Elizabeth Christensen `
## [如何将 Stack Overflow 的 StackExchange 数据加载到 Postgres 中](https://postgresweekly.com/link/150726/web)
这本身就是一个有趣的过程，但该数据集提供了试验您的分析技能或只是了解 Postgres 如何扩展的潜力。


`Francesco Tisiot `
## [按基于时间戳的 UUID 对 Postgres 表进行分区](https://postgresweekly.com/link/150727/web)
来自 Elixir 论坛的一个故事，内容涉及对包含 2800 万行的表进行分区以提高查询速度。 （注意：所示方法主要针对 Elixir 开发人员。）


`Chris O'Brien `

**本周机密：**

* 📢 100% PostgreSQL 分布在 3 个区域，在完全托管的云中提供多主、基于延迟的 DNS 路由 - [免费注册](https://postgresweekly.com/link/150728/web)。
* 🪐 使用 Go 和开源构建您的权限系统。 [SpiceDB](https://postgresweekly.com/link/150729/web) 是 Google Zanzibar 的开源实现。


## [pg_show_plans：显示所有运行语句的查询计划](https://postgresweekly.com/link/150730/web)
允许您通过 SELECT * FROM pg_show_plans 进行实时访问，或者您可以通过 pg_show_plans_q 视图查看它与 pg_stat_activity 的结合。

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/vgvmip7umszc8ajysylb.jpg)

`CYBERTEC PostgreSQL International GmbH `


## [FerretDB 1.19](https://postgresweekly.com/link/150731/web): 就像Mongodb，但在Postgres上。
## [pg_timetable 5.8](https://postgresweekly.com/link/150732/web): 高级调度扩展。
## [Prisma 5.9](https://postgresweekly.com/link/150733/web): 适用于 Node.js 和 TypeScript 的下一代 ORM。
## [PGRX 0.11.3](https://postgresweekly.com/link/150734/web): 一种使用 Rust 构建 Postgres 扩展的方法。
## [PGWIRE 0.19.2](https://postgresweekly.com/link/150735/web): Rust 库中的 Postgres 线路协议。

