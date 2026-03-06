---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2023-10-4
---
### PostgreSQL每周新闻#524 - 2023年10月4日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/524)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/picufmm614atovsqr22r.jpg)
## [pgroll：零停机、可逆架构迁移](https://postgresweekly.com/link/145984/web)
Xata 的人员希望数据库迁移变得简单、无风险且可逆，因此他们构建了一个工具来实现这一目标。 pgroll 使用各种技术（例如“扩展和收缩”模式）将迁移拆分为多个可逆块，并且仅在短锁定（带超时）下执行操作。 [GitHub 代码库](https://postgresweekly.com/link/145986/web)

`Carlos Pérez-Aradros Herce (Xata) `
## [Postgres 表的版本历史记录和生命周期策略](https://postgresweekly.com/link/145951/web)
从 AWS S3 的版本历史记录功能中汲取灵感，本文概述了如何使用temporal_tables 和 pg_partman 扩展来实现 Postgres 表的版本控制和自动数据过期。


`Steven Miller `
## [专为现代工作负载构建的数据存储](https://postgresweekly.com/link/145950/web)
Dragonfly 是 Redis 的直接替代品。 基于 Dragonfly 构建的应用程序具有现代应用程序所需的速度、可靠性和可扩展性，使您能够为用户提供令人难以置信的体验，同时降低成本和复杂性。


`Dragonfly `
## [关于 Oracle 支持 Postgres](https://postgresweekly.com/link/145952/web)
上周，我们注意到 Oracle（云）正在加入 Postgres 游戏。 布鲁斯认为这是个好消息，让我们所有人都感到高兴。 关注这个新闻..😅


`Bruce Momjian `
**本周摘要：**
*   🎨 微软将在 PGConf NYC（正在举行）和 PGConf EU（今年 12 月在捷克布拉格）上分发一本以 Postgres 为主题的“活动手册”，其中包含着色和拼图 - 是的，真的！


*   🎧 Lukas Fittl（pganalyze CEO）▶️ 在 Stack Overflow 播客上谈论为 Postgres 编写高性能 SQL 以及人工智能在数据库优化中的作用。


*   Azure 用户？ Postgres 16 现已在由 Citus 提供支持的 Azure Cosmos DB for PostgreSQL 中提供。


*   在 Hacker News 上，有人勇敢地（？）称 Postgres“神秘且笨重”，并询问为什么 HN 如此喜爱 Postgres？ 🙈


*   Postgres 在矢量存储和索引用例方面的受欢迎程度迅速增长（主要归功于 pgvector），但无服务器 MySQL 平台 PlanetScale 通过分叉 MySQL 来添加矢量支持，从而加大了赌注。


*   但是，如果您还没有完全了解矢量数据库或其用例，Vercel 已经为它们编写了指南：矢量数据库解释。


*   最新的 PGSQL Phriday 博客挑战是写一篇关于为什么使用 Postgres 的文章。


## [查找 Postgres 集群何时初始化](https://postgresweekly.com/link/145962/web)
“使用 Postgres 12 年后的一个很好的发现 - 似乎人们实际上可以检索集群/实例初始化的时间。”


`Kaarel Moppel `
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/jfdkqlmuwskbsng0jevq.jpg)
## [Postgres 国际化的故事](https://postgresweekly.com/link/145963/web)
1996 年，Oleg 在使用 Postgres 构建俄语数据库时遇到了困难，因为当时它仅支持 ASCII 操作。 这引发了 Postgres 国际化故事的开始，Oleg 在此对此进行了更深入的探讨。


`Oleg Bartunov `
## [进入矩阵：Postgres 扩展的四种类型？](https://postgresweekly.com/link/145964/web)
一种可能的思维模型，用于思考可能的不同类型的扩展。


`Steven Miller `
## [使用 Postgres 扩展 GraphQL：经验教训](https://postgresweekly.com/link/145965/web)
Cycle 的一位工程师解释了他们如何遇到影响其服务的数据库超时问题以及他们如何追踪问题。


`Martin Delobbe `

## [使用 OtterTune 的 AI 使您的 AWS RDS 或 Aurora Postgres 速度提高 2 倍](https://postgresweekly.com/link/145967/web)


`Ottertune`
## [允许在 Postgres 中的高度压缩数据中进行 DML 操作](https://postgresweekly.com/link/145968/web)
特别是使用 TimescaleDB。

`TIMESCALE`
## [Postgres 分区管理器的五个重要功能](https://postgresweekly.com/link/145969/web)
Postgres 分区项目 pg_partman 刚刚达到版本 5。本文将介绍五个显着功能，这些功能使其成为管理大型表时的有用工具。


`Keith Fiske (Crunchy Data) `
## [pg_branch：快速分支数据库的实验性扩展](https://postgresweekly.com/link/145982/web)
通过使用写时复制文件系统上的快照，为 Postgres 提供 Neon 式分支功能。 Pre-alpha、使用风险自负等等。


`Alex Pearson `
## [PG_GRAPHQL 1.4](https://postgresweekly.com/link/145972/web)
Supabase 为 Postgres 带来 GraphQL 支持的解决方案。 现在支持 Postgres 16。

## [pgenv 1.3.3](https://postgresweekly.com/link/145973/web)
用于构建、运行和在 Postgres 版本之间切换的实用程序。

## [pgmetrics 1.16](https://postgresweekly.com/link/145974/web)
收集并呈现正在运行的 Postgres 服务器的指标。 现在也支持 Postgres 16。

## [Bytebase 2.9](https://postgresweekly.com/link/145975/web)
团队的数据库开发和 CI/CD 系统。

## [Barman 3.9](https://postgresweekly.com/link/145976/web)
备份和灾难恢复工具。

## [Martin 0.9](https://postgresweekly.com/link/145977/web)
基于 Rust 的快速 PostGIS 地图图块服务器。

## [Slonik 37.0](https://postgresweekly.com/link/145978/web)
类型安全的 Node.js Postgres 客户端。 创建者还刚刚发布了将 Slonik 集成到 Express.js 应用程序中的指南。

## [pg_cron 1.6.1](https://postgresweekly.com/link/145980/web)
在 Postgres 中运行定期作业。

## [Unisub](https://postgresweekly.com/link/145981/web)
由 Postgres 支持的 Rust pub/sub 库。