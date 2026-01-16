---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-6-19
---
### PostgreSQL每周新闻#604 - 2025年6月19日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/604)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/sapfz2tfizqacc9feyu5.jpg)
## [PostgreSQL 与 Ducks：完美的分析组合](https://postgresweekly.com/link/170646/web)
DuckDB 是一款针对 OLAP 工作负载优化的进程内 SQL 数据库，近年来备受关注。将其与 Postgres 结合，可以实现高性能分析任务，而无需构建完整的数据仓库或复杂的 ETL 管道。本文将探讨主要的集成选项。

`Matson and Somani (MotherDuck)`

## [▶ 30+ 场来自 PGConf.dev 2025 的演讲可供欣赏](https://postgresweekly.com/link/170648/web)
过去几周，五月流行的 PostgreSQL 开发大会的演讲视频已经上传，有很多内容值得欣赏，从 OpenAI 如何扩展 Postgres 和构建 Postgres 扩展的棘手性到调查多线程 Postgres 以及 10 位 Postgres 贡献者如何成为黑客。


`PostgreSQL Development Conference `

## [错过了 POSETTE 2025？现在即可点播观看全部 42 场演讲](https://postgresweekly.com/link/170645/web)
了解 PostgreSQL 生态系统中 45 位专家的最新功能、性能技巧和实际应用。POSETTE：Postgres 盛会是由微软 Postgres 团队组织的免费线上开发者活动。立即观看。

`Microsoft `

## [SELECT .. FOR UPDATE 是否有害？](https://postgresweekly.com/link/170653/web)
如果在事务中执行 SELECT 时指定了 FOR UPDATE，则选定的行将被锁定，以防止您计划随后更新这些行时进行并发更新。Laurenz 指出，这种锁定在很多情况下可能“过于强大”，而 FOR NO KEY UPDATE 可能更合适，并且能够提供足够的保护。

`Laurenz Albe`

### **本周摘要**

* 🐅 Timescale，也就是开发同名 [TimescaleDB](https://postgresweekly.com/link/170654/web) 时间序列扩展程序的公司，现已不复存在：它现在更名为 [TigerData](https://postgresweekly.com/link/170655/web)。
* 
* 🇦🇺 [PG Down Under 202](https://postgresweekly.com/link/170656/web) 将于今年 10 月在澳大利亚举行。其 CFP 截止日期为 7 月 15 日。

* 🇺🇸 2025 年还不到一半，但如果您想在日历上安排一项 2026 年的 Postgres 活动，[PG Data Conference 2026](https://postgresweekly.com/link/170657/web) 将于明年 6 月在芝加哥举行。

* Nisha Moond，曾就职于 Oracle，现就职于富士通的 Postgres 团队，是[本周 PostgreSQL 人物的采访对象](https://postgresweekly.com/link/170658/web)。


## [双活复制，你真的需要它吗？](https://postgresweekly.com/link/170659/web)
上周我们提到亚马逊开源了 pgactive，这是一个用于执行双活复制的扩展程序。Jan 探讨了它可能在哪些情况下发挥作用。

`Jan Wieremjewicz`

📄 [逻辑复制入门](https://postgresweekly.com/link/170661/web) – 基本概念和技术的入门指南。Radim Marek

📄 [我如何在周五晚上搞垮了生产数据库](https://postgresweekly.com/link/170662/web) – “切勿对关键外键使用 CASCADE 删除。” Vincent Josse

📄 [避免时区陷阱：在 Django 中使用 Postgres 正确提取日期/时间子字段](https://postgresweekly.com/link/170663/web) Colin Copeland

📺 [Postgres 开发者 ClickHouse 更新和删除指南](https://postgresweekly.com/link/170664/web) Mark Needham

📄 [罗马数字到数字的转换以及 Postgres 的乐趣](https://postgresweekly.com/link/170665/web) Laurenz Albe

📄 [检查清单：你的 Postgres 部署是否达到“生产级”标准？](https://postgresweekly.com/link/170666/web) Umair Shahid


### **代码和工具**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/wwxcrqzhrv5anvfbsz6f.jpg)

## [▶ 介绍微软针对 Postgres 的 VS Code 扩展](https://postgresweekly.com/link/170667/web)
我们最近提到微软宣布推出针对 VS Code 的新 Postgres 扩展，Matt 在 POSETTE 上发表了演讲，其中包括一些如何使用它的演示。

`Matt McFarland`

## [XTDB v2：一个支持时间旅行的不可变 SQL 数据库](https://postgresweekly.com/link/170669/web)
一个有趣的 SQL 数据库，所有表都是双时态的（同时存储数据的有效时间和记录时间），并且“时间旅行”是首要关注点。它与 Postgres 无关，但提供了与 Postgres 兼容的接口，以便于采用。GitHub 代码库。

`Jeremy Taylor (JUXT)`

## [pg_auto_reindexer 1.5：自动 B 树重建索引工具](https://postgresweekly.com/link/170671/web) 
一个脚本，通过使用 REINDEX CONCURRENTLY 以最少的锁定检测和重新索引臃肿的 B 树索引。

`Vitaliy Kukharik`

[qsv 5.1](https://postgresweekly.com/link/170673/web) – 用于查询、切片、过滤、转换、排序和转换表格数据的 CLI 工具。

[PostgREST 13.0.4](https://postgresweekly.com/link/170674/web) – 适用于任何 Postgres 数据库的 REST API。

[Prisma 6.10](https://postgresweekly.com/link/170675/web) – 下一代 Node.js + TypeScript ORM。

[pg_dumpbinary v2.20](https://postgresweekly.com/link/170676/web)