---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-5-8
---
### PostgreSQL每周新闻#599 - 2025年5月8日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/598)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/omacmxvsxigzrz01yepn.jpg)
## [Postgres 18 发行说明草稿](https://postgresweekly.com/link/169068/web)
Bruce Momjian 刚刚完成了 Postgres 18 发行说明的初稿，以赶上 Beta 1 的发布。最终版本预计将于 9 月或 10 月发布。

`Bruce Momjian et al.`

## [Postgres 18 Beta 1 发布](https://postgresweekly.com/link/169088/web)
Postgres 18 的首次官方预览于过去几个小时内发布。发行说明概述了整体情况，但 PG18 正在逐渐成为一个稳健的版本，它拥有更快的 Linux 扫描和清理速度、并行 GIN 构建、虚拟生成列、OAuth 支持、增强的 EXPLAIN ANALYZE 输出等等。现在就可以开始体验了。


`Jonathan Katz et al.`
`📢[Postgres 17.5、16.9、15.13、14.18 和 13.21](https://postgresweekly.com/link/169089/web) 也已发布。`

## [[O’Reilly 新品] CockroachDB：权威指南 第二版](https://postgresweekly.com/link/168700/web)
学习如何使用兼容 Postgres 的分布式 SQL 数据库构建高弹性、可扩展的应用。相同的 Postgres 使用体验——熟悉的工具、模式和查询——可在全球范围内、本地或任何云平台进行扩展，并具有原生地理数据放置和低 TCO。


`Cockroach Labs`
## [Postgres 18 中的异步 I/O 加速磁盘读取](https://postgresweekly.com/link/169070/web)
Postgres 18 的第一个 Beta 版本添加了有限的异步 I/O (AIO) 支持——这项功能已经酝酿多年。本文将解释它的含义、工作原理以及它对性能优化的意义。

`Lukas Fittl`

### **本周摘要**

* [微软的 Claire Giordano 发表了一篇相当精彩的文章](https://postgresweekly.com/link/169071/web)，介绍了微软过去一年在 Postgres 方面的工作——无论是关于其自身的服务（例如 Azure Database for PostgreSQL），还是其对核心 Postgres 项目的贡献。

* 🇺🇸 [PGConf NYC 2025](https://postgresweekly.com/link/169072/web) 将于今年 9 月在纽约举行。如果您想发言，请在 5 月 25 日之前[提交提案](https://postgresweekly.com/link/169073/web)。

* 🇨🇭 [Swiss PGDay 2025]（https://postgresweekly.com/link/169074/web） 将于 6 月 26 日至 27 日举行，具体[日程]（https://postgresweekly.com/link/169075/web）刚刚公布。

* Timescale [宣布 pgai Vectorizer 现已兼容任何 Postgres 设置](https://postgresweekly.com/link/169076/web)。

* Koyeb 宣布其 [Koyeb Serverless Postgres 平台现已正式发布](https://postgresweekly.com/link/169077/web)。

📄 再谈 [CTE 物化和非幂等子查询](https://postgresweekly.com/link/169078/web) Shayon Mukherjee

📊 [PgDog 与 PgBouncer](https://postgresweekly.com/link/169079/web) 的数据对比——三种扩展方案的较量。Lev Kokotov

📄 [在 .NET EF Core 应用中从 Postgres 迁移到 MongoDB](https://postgresweekly.com/link/169080/web)——这不是我想要的方向，但如果你需要的话……Luce Carter

📄 [Jacob Champion 成为 Postgres 提交者](https://postgresweekly.com/link/169081/web) Caroline Pickens (EDB)

📄 [哪位 (LLM) 编写的分析型 SQL 最棒](https://postgresweekly.com/link/169082/web)？Ramirez 和 Romeu (Tinybird)


### **快速发布**

[pg_parquet v.0.4.0 正式发布](https://postgresweekly.com/link/169083/web) — pg_parquet 提供了一种在 Postgres 中直接导出和导入 Parquet 文件的方法，无需依赖第三方工具。 - Aykut Bozkurt (Crunchy Data)

[external_file 1.2](https://postgresweekly.com/link/169084/web) – 一款允许从 Postgres 服务器文件系统访问外部文件的扩展程序。

[csv-to-sql-insert](https://postgresweekly.com/link/169085/web) – 一款将 CSV 文件转换为 SQL INSERT 语句的工具。

[River 0.21](https://postgresweekly.com/link/169086/web) – 适用于 Go 和 Postgres 的强大作业处理系统。

[pg_timetable 5.13](https://postgresweekly.com/link/169087/web) – 高级调度扩展程序。