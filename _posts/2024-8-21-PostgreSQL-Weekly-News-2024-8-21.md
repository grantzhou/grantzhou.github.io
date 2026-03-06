---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-8-21
---
### PostgreSQL每周新闻#566 - 2024年8月21日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/566)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/ibspujzcfsdysseetixe.jpg)
## [Postgres 的每个维护产品线都有新版本发布](https://postgresweekly.com/link/158704/webb)
即 16.4、15.8、14.13、13.16、12.20，甚至 Postgres 17 的第三个测试版。这些版本主要用于推出错误修复，但 pg_dump 漏洞也已得到解决。Postgres 17 最终版本（暂定）预计将于 9 月发布。

`PostgreSQL Global Development Group `

## [🦆🐘 拼接 Duck(DB) 和 Elephant DNA](https://postgresweekly.com/link/158705/web)
DuckDB 是一种快速、进程内 OLAP 数据库系统，也是一项出色的工程。因此，很高兴看到官方 pg_duckdb 扩展将 DuckDB 的功能带入 Postgres 世界，并得到了 Microsoft、Hydra 和 Neon 的支持。

💡 The Register 有一篇[新闻报道](https://postgresweekly.com/link/158708/web)，详细介绍了这项工作的背景。
`Tigani 和 Griffin (MotherDuck) `
## [简化PostgreSQL 升级](https://postgresweekly.com/link/158703/web)
简化您的 PostgreSQL 升级，无需停机。我们的专业 DBA 确保顺利过渡，解决阻碍因素和性能问题。轻松规划、测试、设置和升级。填写表格，立即开始升级！


`Percona  `
## [Postgres 如何在磁盘上存储数据（这是一本值得一读的书）](https://postgresweekly.com/link/158709/web)
对 Postgres 如何在磁盘上存储数据进行了很好的概述，涵盖了段、页面等。比你需要知道的更深入，直到有一天，你突然明白了……


`Drew Silcock `
## [使用 Postgres 作为搜索引擎](https://postgresweekly.com/link/158710/web)
人们多年来一直在搜索系统中使用 Postgres，尤其是其强大的全文索引功能。但是，您可以进一步使用基于向量的语义搜索和模糊匹配。Eric 在此处汇总了一些想法，并附有查询。


`Eric Zakariasson `

### 本周摘要：

* 作为 Postgres 版本（上文）的一部分，我们提醒您，Postgres 12 将从 2024 年 11 月 14 日起停止接收修复。

* 您知道 Postgres 中包含两个 JSON 解析器吗？Andrew Dunstan 讲述了[为什么以及如何发生这种情况](https://postgresweekly.com/link/158711/web)。

## [在 pgsql-hackers 上发布您的补丁](https://postgresweekly.com/link/158237/web)
Robert 继续努力鼓励新的 Postgres 贡献者，并提供一些关于如何最好地提交补丁的提示，特别是当您以前尝试过 [pgsql-hackers](https://postgresweekly.com/link/158713/web) 列表却没有任何进展时。


`Robert Haas `
💡 如果您不确定要创建什么补丁，Tomas Vonda 已经写了有关[如何选择您的第一个补丁](https://postgresweekly.com/link/158714/web)的文章。
## [通过 WASM 和 PGlite 在 Node-RED 内部运行 Postgres](https://postgresweekly.com/link/158715/web)
Node-RED 是一种流行的基于 Node.js 的“低代码”编程环境，您可以在浏览器中构建“流”来将代码连接在一起。


`Conor O'Neill`
## [在 Amazon Aurora 和 RDS 中构建自定义 HTTP 客户端](https://postgresweekly.com/link/158717/web)
Oracle 数据库用户可以使用 UTL_HTTP 包从他们的程序与 HTTP 服务器进行通信，但是当他们迁移到 Aurora 或 RDS 上的 Postgres 时，需要一种新的方法。


`Gudivada, Jammula, et al.`

### 机密：

📊 您如何驾驭数据库领域？参加 [Redgate 的问卷调查](https://postgresweekly.com/link/158718/web)并参加抽奖，有机会赢得 250 美元的亚马逊代金券。

[Blacksmith](https://postgresweekly.com/link/158719/web) 只需更改一行代码，即可将 GitHub Actions 的运行速度提高 2 倍，成本降低一半。受到 GitBook 和 Slope 等 100 多家公司的信赖。

📄 [Postgres 开发会永远依赖邮件列表吗？](https://postgresweekly.com/link/158720/web) Tomas Vondra

📄 [消除关于 Postgres 默认权限的误解](https://postgresweekly.com/link/158721/web) Sagar Jadhav

📄 [您未使用的最佳 Postgres 功能：CTE 又名 WITH 子句 – 经典之作](https://postgresweekly.com/link/158722/web) Craig Kerstiens

📄 [Postgres 中的哈希与 B 树索引](https://postgresweekly.com/link/158723/web) Evgeniy Demin

### 🛠 代码和工具
## [Pigsty v3.0 Beta 1 发布，重点关注扩展](https://postgresweekly.com/link/158724/web)
Pigsty 是一款有趣的 Postgres 发行版，承诺“内置电池”。它基本上是一个类似 RDS 的平台，但可以根据需要进行部署。现在，它允许您轻松安装 333 个扩展以及 Babelfish、IvorySQL 和 PolarDB 等“可插入内核”。


`Ruohang Feng`
## [PostgREST 12.2 发布：以 RESTful 方式访问 Postgres](https://postgresweekly.com/link/158726/web)
现在包括 Prometheus 兼容性和语句超时，PostgREST 是一个基于 Haskell 的系统，可从任何 Postgres 数据库提供完全 RESTful API。GitHub 存储库。


`Steve Chavez and Joe Nelson`

[DoltgreSQL 0.11](https://postgresweekly.com/link/158728/web) – 版本控制的 Postgres 类似版本。

[PGlite 0.2](https://postgresweekly.com/link/158729/web) – 轻量级 Postgres 打包为 WASM，用于浏览器、Node.js、Bun 和 Deno 的 TypeScript 库。

[River 0.11.3](https://postgresweekly.com/link/158730/web) – 快速可靠的 Postgres 后台作业，适用于 Go。

[pg_cron 1.6.4](https://postgresweekly.com/link/158731/web) – 运行定期作业。比 pg_timetable 更简单。

[Good Job 4.2](https://postgresweekly.com/link/158732/web) – Postgres 支持的 Ruby on Rails 作业队列。

[SeaORM 1.0](https://postgresweekly.com/link/158733/web) – Rust 的动态异步 ORM。

[sqlc 1.27](https://postgresweekly.com/link/158734/web) – 从 SQL 生成类型安全的 Go 代码。

[PostgreSQL 高可用性集群 2.0](https://postgresweekly.com/link/158735/web)