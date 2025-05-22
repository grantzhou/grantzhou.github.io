---
layout: post
title: PostgreSQL 每周新闻 2025-5-22
---
### PostgreSQL每周新闻#601 - 2025年5月22日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/601)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/jytbd3eqzdt5ksgtmibp.jpg)
## [微软在 VS Code 中推出 Postgres IDE](https://postgresweekly.com/link/169528/web)
微软为其 VS Code 编辑器推出了新的 Postgres 扩展的公开预览版，该扩展可让您管理数据库对象、使用 IntelliSense 构建查询以及与 Copilot 集成。

`Microsoft`

## [pgconf.dev 2025 在蒙特利尔圆满落幕](https://postgresweekly.com/link/169529/web)
我从众多渠道得知，上周的 PGConf.dev 活动取得了巨大成功，这是我见过的关于 Postgres 活动最详尽的报道之一（附有照片）。希望在接下来的几周里我们也能看到一些视频。


`Cary Huang`
```
💡 如果您想提前了解 2026 年的活动，它[将于 5 月 19 日至 22 日重返温哥华](https://postgresweekly.com/link/169531/web)。
```

## [(O’Reilly 新品) CockroachDB：权威指南 第二版](https://postgresweekly.com/link/169527/web)
学习如何使用兼容 Postgres 的分布式 SQL 数据库构建高弹性、可扩展的应用。相同的 Postgres 使用体验——熟悉的工具、模式和查询——可在全球范围内、本地或任何云平台进行扩展，并具有原生地理数据放置和低 TCO。

`Cockroach Labs `

### **本周摘要**

* [了解 Postgres 18 对 UUIDv7 的支持](https://postgresweekly.com/link/169532/web)。

* [🤖 并了解 Azure Database for PostgreSQL 最新的生成式 AI 功能](https://postgresweekly.com/link/169533/web)，这些功能来自 Microsoft Build 大会。

* [Postgres 迎来了几位新的 Google Summer of Code 贡献者](https://postgresweekly.com/link/169534/web)。

* [最新 Postgres 扩展迷你峰会的文字记录](https://postgresweekly.com/link/169535/web)，主题是如何利用 CloudNativePG 改进 Kubernetes 中的 Postgres 扩展体验。

## [pgModeler 1.2：Postgres 数据库建模工具](https://postgresweekly.com/link/169408/web) — 一种以更直观的方式轻松创建和编辑数据库模型的方法。它已打包为付费产品，但也是开源的（GPLv3 - 代码库在此），因此您可以自行构建。v1.2 是一个重要更新。

`Raphael Araújo e Silva`

## [创建短字母数字伪随机标识符](https://postgresweekly.com/link/169536/web)
假设您需要创建一个可读且唯一的多字符标识符来表示 ID，但又不能像 UUID 那样长（例如 YouTube 视频 ID）。PL/PgSQL 可以帮您解决！

`Andrew Atkinson`

## [▶ 扩展 Postgres：关于 Postgres 的每周节目](https://postgresweekly.com/link/169537/web)
几年来，Creston 每周都会制作一个视频，深入探讨最新的 Postgres 新闻、文章等 — 就像我们一样，但他会更多地即兴发挥并分享他的经验和见解。

`Creston Jamison`

## [Postgres 中的数据归档与保留](https://postgresweekly.com/link/169538/web)
Daria 展示了她在德国 PGConf 大会上的演讲幻灯片及讲解，她在演讲中介绍了处理大型数据集的最佳实践。这里有很多实用技巧。

`Daria Nikolaenko`

📄 [如何在 TimescaleDB 中安全地执行回填操作](https://postgresweekly.com/link/169539/web) Semab Tariq

📄 [使用 SQL 渲染曼德布洛特集——这仍然是我们最喜欢的查询](https://postgresweekly.com/link/169540/web) PostgreSQL Wiki

### **代码和工具**

## [dblab：一个支持 Postgres、MySQL 等数据库的交互式客户端](https://postgresweekly.com/link/169541/web)
一个基于 Go 语言的跨平台（没错，包括 Windows）TUI 风格的应用，可用于操作各种数据库系统。它的外观与标准的 CLI 客户端截然不同。

`Daniel Omar Vergara Pérez`

## [方便的 PostgreSQL 命令行选项速查表](https://postgresweekly.com/link/169542/web)

`Diego Kartones`

[PostGIS 3.6.0 Alpha 1](https://postgresweekly.com/link/169543/web) 和 [PostGIS 3.5.3](https://postgresweekly.com/link/169544/web) – 广受欢迎的地理空间扩展。

[TimescaleDB 2.20](https://postgresweekly.com/link/169545/web) – 扩展中新增 Postgres 的时间序列功能。包含一些显著的性能改进。

[Barman 3.14](https://postgresweekly.com/link/169546/web) – 备份和灾难恢复工具。现已支持对备份和 WAL 文件进行 GPG 加密。

[node-pg-migrate 8.0](https://postgresweekly.com/link/169547/web) – Node.js 数据库迁移管理。