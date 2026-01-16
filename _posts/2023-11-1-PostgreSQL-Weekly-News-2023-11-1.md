---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2023-11-1
---
### PostgreSQL每周新闻#528 - 2023年11月1日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/528)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/fp6nvxhxl8fgulotrd56.jpg)
## [让 Postgres 发挥作用：pg_cron 中的新功能](https://postgresweekly.com/link/147099/web)
pg_cron 是一个扩展，可以轻松在 Postgres 中运行定期作业，无需外部调度程序。 它不像 pg_timetable （上周介绍）那么先进，但它的简单性可能更适合您的用例。 在这里，Marco 展示了 pg_cron 如何以每秒精细的粒度运行作业。


`Marco Slot (Citus Data) `
## [使用 AI 自动优化您的 RDS 或 Aurora Postgres 数据库](https://postgresweekly.com/link/147098/web)
需要帮助优化 Postgres 运行、查询、索引和 autovacuum？ OtterTune 是您的人工智能数据库副驾驶，可以提高性能、降低成本并保持数据库健康。 获得三个数据库的 30 天免费试用。


`OtterTune `
## [Nile：新的无服务器 Postgres 平台](https://postgresweekly.com/link/147102/web)
Neon 可能是目前最著名的无服务器 Postgres 平台，但一些新的竞争即将到来。 Nile 的角度专注于 SaaS 使用，通过无缝租户隔离和扩展支持多租户设置。 它位于候补名单后面，但这篇文章深入探讨了他们的方法。


`Sriram Subramanian (Nile) `
🗣 Nile 的声明在 Hacker News 上引起了广泛的讨论，主要围绕多租户的利弊。
## [SQL 标识列](https://postgresweekly.com/link/147105/web)
您也可以将它们称为自动增量列或串行列，但此类标识列（最终）在 SQL:2003 中标准化，并且 Postgres 自 Postgres v10 以来就支持其 GENERATED ALWAYS AS IDENTITY 语法。


`Peter Eisentraut `

**本周摘要：**

*   📅 FOSDEM PGDay 2024 的日期已公布 - 将于 2024 年 2 月 2 日在比利时布鲁塞尔举行。演讲主题已开放申请，提交截止日期为 11 月 27 日。


*   Heroku 已向 Heroku Postgres 添加了对 pgvector 扩展的支持。


*   Bruce Momjian 查看了 Postgres 16 的新 pg_stat_*_tables last_seq_scan 和 last_idx_scan 列。


*   当您收到 “错误：当前事务被中止，命令被忽略直到事务块结束” 时，发生了什么？ – Hans-Jürgen Schönig 解释了一切。


## [▶ 使用 Django、Postgres 和 pgvector 存储和查询 LLM 嵌入](https://postgresweekly.com/link/147111/web)
我们最近多次提到 pgvector，这里看一下它的实际用例 - 构建基于 LLM 嵌入的搜索系统，该系统能够使用非结构化的描述做搜索。 [GitHub repo](https://postgresweekly.com/link/147113/web)。


`William Huster `
## [使用 Postgres 进行 GDB 调试要点](https://postgresweekly.com/link/147114/web)
使用 Postgres 作为实际示例，探索使用 GDB 进行调试的要点。 （注意：日常 Postgres 用户不需要这，但如果您是 C/C++ 开发人员或从事 Postgres 内部工作，您会发现它很有用。）


`Cary Huang `
## [📅 11 月 15 日网络研讨会：使用约束编程自动选择索引](https://postgresweekly.com/link/147115/web)


`pganalyze `
## [什么是 TOAST（以及为什么它不足以用于 Postgres 中的数据压缩）](https://postgresweekly.com/link/147116/web)


`CARLOTA SOTO (TIMESCALE)`
## [如何理解 Explain Plan]


`MUHAMMAD ALI (STORMATICS)`

**代码和工具：**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/dgcjlpuobbo9delcqffg.jpg)

## [PL/Haskell 3.1：在 SQL 函数中使用 Haskell](https://postgresweekly.com/link/147118/web)
Haskell 是一种函数式语言，但您仍然可以使用它来定义过程，以便 Postgres 可以很好地使用。


`Edward F. Behn, Jr. `
## [pg_graphql 1.4.2：为 Postgres 提供 GraphQL 支持](https://postgresweekly.com/link/147119/web)
从现有 SQL 模式反映 GraphQL 模式，让任何 GraphQL 客户端通过 GraphQL 查询数据库，无需额外的服务器、进程或库。


`Supabase `
## [PostgresNIO 1.19.0](https://postgresweekly.com/link/147120/web)
 - 适用于 Swift 的非阻塞、事件驱动的 Postgres 客户端。

## [DBMate 2.7](https://postgresweekly.com/link/147121/web)
 - 轻量级、与框架无关的数据库迁移工具。

## [data-diff 0.9.9](https://postgresweekly.com/link/147122/web)
 - 比较数据库内或跨数据库的表。

## [Bytebase 2.10](https://postgresweekly.com/link/147123/web)
 - 数据库开发和 CI/CD 平台。

## [Slonik 37.2](https://postgresweekly.com/link/147124/web)
 - Node.js 的类型安全 Postgres 客户端。

## [Patroni 3.2](https://postgresweekly.com/link/147125/web)
 - PostgreSQL 高可用性模板。