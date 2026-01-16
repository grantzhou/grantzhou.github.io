---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-7-3
---
### PostgreSQL每周新闻#606 - 2025年7月3日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/606)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/airmujwtkqsnko34s0al.jpg)
## [PlanetScale 携 Benchmarks-a-Plenty 进军 Postgres 市场](https://postgresweekly.com/link/171269/web)
本周，商业 Postgres 领域的重磅新闻是，以其高性能、可扩展的 MySQL 服务而闻名的 PlanetScale 也决定进军 Postgres 市场。目前，Postgres 还处于“私人预览”阶段，但他们似乎已经准备好从一开始就向其他提供商发起挑战。

`Ben Dicken (PlanetScale)`

## [PostgreSQL 性能不佳？用 pgNow 诊断](https://postgresweekly.com/link/171268/web)
刚接触 Postgres 还是时间紧迫？pgNow 提供快速、精准的诊断功能，帮助您调整配置、修复性能下降并立即发现问题。无需设置，无需代理，只需极少权限。免费下载，几秒钟即可开始使用。


`Redgate  `

## [关于 Postgres 计划缓存模式管理](https://postgresweekly.com/link/171272/web)
对查询计划的世界进行了有趣的观察，在使用通用计划时如何平衡优点和缺点（即提前为准备好的语句生成的查询计划，可以快速重用），以及是否有办法在适当的时候有效地切换/更新计划。

`Andrei Lepikhov `

## [查询计划多久一次是最佳的？](https://postgresweekly.com/link/171273/web)
既然我们讨论这个话题了……

`Tomas Vondra`

### **本周摘要**

* [PostgreSQL 17 现已在 Azure Database for PostgreSQL](https://postgresweekly.com/link/171274/web) 灵活服务器上正式发布。

* [Samed Yildirim](https://postgresweekly.com/link/171275/web) 是本周 PostgreSQL 人物的采访对象。

## [在 Postgres 中构建复制安全的 LSM 树](https://postgresweekly.com/link/171276/web)
深入了解将 Elasticsearch 风格的搜索引入 Postgres 所需的工程，其方式远远超出了 Postgres 的标准全文搜索实现。

`Hood, Ying, Pregasen and Ratliff (ParadeDB)`

📄 [简化代码及与 Postgres 的交互](https://postgresweekly.com/link/171277/web) – “与 Postgres 交互时，或许该问问自己：你是否以最精简的方式进行操作？” Manni Wood

📄 [使用 pgroll 实现零停机模式迁移](https://postgresweekly.com/link/171278/web) Dhanush Reddy (Neon)

📄 [幕后花絮：加速 pgstream 快照](https://postgresweekly.com/link/171279/web) Sanz (Xata)

📄 [将 Postgres 分区归档到 Iceberg](https://postgresweekly.com/link/171280/web) Craig Kerstiens


### **🛠 代码和工具**

## [Squawk：Postgres 迁移的 Linter](https://postgresweekly.com/link/171281/web)
想象一下类似 ESLint 的东西，但用于 Postgres 迁移和其他 SQL。如果你想在不安装任何东西的情况下在某些 SQL 上测试它，这里有一个在线测试平台。

`Steve Dignam`

## [pgrx 0.15：使用 Rust 构建 Postgres 扩展](https://postgresweekly.com/link/171283/web)
这个广受欢迎且历史悠久的 Rust 扩展构建框架现已获得 Postgres 18 的初步支持。GitHub 代码库。

`PgCentral Foundation, Inc.`

* [pgtt 4.4](https://postgresweekly.com/link/171285/web) – 创建、管理和使用 Oracle 风格的全局临时表。

* [Barman 3.14.1](https://postgresweekly.com/link/171286/web)– 远程备份和灾难恢复工具。

* [PGSync 4.1](https://postgresweekly.com/link/171287/web) – Postgres 与 Elasticsearch/OpenSearch 同步。

* [pgAdmin 4 v9.5](https://postgresweekly.com/link/171288/web) – 流行的基于 Web 的管理界面。

* [Prisma 6.11](https://postgresweekly.com/link/171289/web) – 下一代 Node.js + TypeScript ORM。