---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-10-9
---
### PostgreSQL每周新闻#619 - 2025年10月9日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/619)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/myxf1as8sucatryemg4h.jpg)
## [建置和debug Postgres](https://postgresweekly.com/link/175084/web)
如何设定容器，从原始程式码建置 Postgres，然后使用 GDB 和 VS Code 进行debug。如果你想深入了解 Postgres 的内部机制，这些技巧很有用。

`Stefanos Baziotis`


## [使用 S3 范围读取探索 Postgres 到 Parquet 归档的 JSON 资料](https://postgresweekly.com/link/175083/web)
如何将「冷」 JSON 从 Postgres 移至 S3 上的 Parquet，然后能够快速取回它而无需读取整个档案。

`Shayon Mukherjee `

## [如何实施 Postgres DevOps 和安全性](https://postgresweekly.com/link/175385/web)
审查、批准、部署和强制执行查询存取控制。此外还有动态资料屏蔽和审计追踪。一体化 GUI 工作区，开源，受到 350 多家公司的信赖，包括 Linear 和 note.com。

`Bytebase `

## [▶ Postgres 18 实作：非同步 I/O、B 树跳跃扫描、UUIDv7](https://postgresweekly.com/link/175388/web)
pganalyze 的创办人举办了一场网路研讨会，深入探讨了 Postgres 18 中一些更值得注意的改进。关于非同步 I/O 的部分（从 4:20 到 22:30）特别有用。

`Lukas Fittl `



### **本周摘要**

* 🌐 [PostGIS Day 2025](https://postgresweekly.com/link/175390/web) 是一场免费的线上活动，将于 11 月 20 日举行，面向对地理空间应用感兴趣的 Postgres 用户。

* 🇫🇷 [2026 年巴黎 pgDay 会议](https://postgresweekly.com/link/175391/web)现已开放征文。会议将于 2026 年 3 月举行，投稿截止日期为 12 月 19 日。

* 历史悠久的 Postgres 顾问公司 [CYBERTEC](https://postgresweekly.com/link/175392/web) 为庆祝成立 25 周年，[特采访其执行长兼创办人 Hans-Jürgen Schönig](https://postgresweekly.com/link/175393/web)，讲述公司成立和发展历程。

* 🇯🇵 [2025 年日本 PostgreSQL 大会](https://postgresweekly.com/link/175394/web)将于 11 月 11 日在东京举行。


## [关于开发 Postgres 的 OAuth 支持](https://postgresweekly.com/link/175395/web)
Postgres 中 OAuth 支持的首批倡导者之一（在此以实际意义进行探索）讲述了它在 Postgres 18 中的出现、它为何令人兴奋以及未来的发展。


`Jacob Champion`


📄 [使用 Postgres CONSTRAINT](https://postgresweekly.com/link/175397/web) 进行棘轮操作 – 强制约束（例如「NOT NULL」）的方法，无需立即在全表范围内强制执行。 Andrew Judson

📄 [使用逻辑复制进行 Postgres 迁移](https://postgresweekly.com/link/175398/web) Elizabeth Christensen

📄 [IBM 邀请 CockroachDB 在其大型主机上使用「PostgreSQL」](https://postgresweekly.com/link/175399/web)——这在 The Register 上是一个典型的古怪标题！事实上，IBM 正在寻求在其大型主机硬体上提供类似 Postgres 的资料库。 The Register

📄 [TimescaleDB 中的 SkipScan](https://postgresweekly.com/link/175400/web)：DISTINCT 为什么缓慢，我们如何建造它，以及如何使用它 Aksman 和 Hein（TigerData）

📄 [Postgres 16 中的关键操作增强和整合选项](https://postgresweekly.com/link/175401/web) Sebastian Insausti


## **发布**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/ilr1y1fd1qnoc2gwjagy.jpg)

## [pgwatch 4.0：灵活的 Postgres 监控解决方案](https://postgresweekly.com/link/175402/web)
透过 Grafana 仪表板提供使用者友善的介面，让您可以检查各种指标（运作状况、效能、索引使用情况、I/O 等）和趋势。 v4.0 引入了各种增强功能并放弃了对 Grafana v10 的支援。

`CYBERTEC`

## [pg_statement_rollback v1.5：语句层级的伺服器端回滚](https://postgresweekly.com/link/175404/web)
新增语句层级的伺服器端事务回滚，类似 Oracle 或 Db2。此版本新增了对 Postgres 18 的支援。

`Hexacluster`

[PostgreSQL R2DBC 驱动程式 1.1](https://postgresweekly.com/link/175405/web) – 将响应式 API 引入 Java 世界中的关联式资料库。

[QuestDB 9.1](https://postgresweekly.com/link/175406/web)– 基于 Java 的时间序列资料库，相容于 Postgres 有线协定。

[River 0.26](https://postgresweekly.com/link/175407/web) – 快速可靠的 Postgres 后台作业系统，适用于 Go 语言。

[tbls 1.89](https://postgresweekly.com/link/175408/web) – 自动以 Markdown 格式（例如在 CI 中）记录资料库。

[Goose 3.26](https://postgresweekly.com/link/175409/web) – 资料库迁移工具。支援 SQL 和 Go 函数。

[Mathesar 0.6](https://postgresweekly.com/link/175410/web) – 类似电子表格的 Postgres 表格介面。

[Barman 3.16](https://postgresweekly.com/link/175411/web) – 备份与灾难复原工具。