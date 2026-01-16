---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-1-16
---
### PostgreSQL每周新闻#584 - 2025年1月16日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/584)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/j3ist8tv2e3hd5e19jo2.jpg)
## [不要这样做（在 Postgres 中）](https://postgresweekly.com/link/164439/web)
Postgres 官方 wiki 上一个有趣的页面，其中总结了使用 Postgres 时“常见错误”的各种建议以及不该做的事情，例如“不要使用 char(n)”和“不要使用 serial”。其中一些可能会引起争议，但有充分的理由支持。该页面已更新，但希望看到更多内容得到添加。

`Postgres Wiki`

## [Postgres 中的开源力量](https://postgresweekly.com/link/164419/web)
Laurenz 展示了 Postgres 的开源特性在回答有关其运作方式的问题时是多么宝贵，例如通过追踪 autovacuum_vacuum_scale_factor 默认设置的原因。了解如何做他在这篇文章中做的事情是一项宝贵的技能。


`Laurenz Albe `
## [寻找 2025 年最佳 Postgres 监控和调优供应商](https://postgresweekly.com/link/164417/web)
下载我们的免费供应商评估模板，快速比较功能、评分演示，并自信地选择最佳的 Postgres 性能和监控解决方案来满足您的 2025 年预算需求。

`pganalyze  `

### 本周摘要：

* 🇧🇪 [FOSDEM PGDay](https://postgresweekly.com/link/164420/web) 是即将举行的年度 [FOSDEM](https://postgresweekly.com/link/164421/web) 活动中以 Postgres 为重点的附带活动。它将于 1 月 31 日在比利时布鲁塞尔举行，目前仍开放报名。

* 🥈 奇怪的是，[DB-Engines](https://postgresweekly.com/link/164440/web) 早些时候宣布 [Postgres 是他们 2024 年度数据库管理系统](https://postgresweekly.com/link/164418/web)，但最近几个小时，这一称号被更正为 Snowflake，将 Postgres 排在第二位。（这原本是我们的主要功能，但排在第二位听起来不太一样……？😅）

* [SQL Squid Game](https://postgresweekly.com/link/164441/web) 是一个以 Squid Game 为主题的九级 SQL 挑战。

## [表级锁的剖析](https://postgresweekly.com/link/164423/web)
了解数据库系统中锁定背后的含义和动机，然后更仔细地研究在 Postgres 中锁定表的各种方式以及如何解决这些锁之间的冲突。


`Gulcin Yildirim Jelinek `
## [空闲事务会导致表膨胀？等等，什么](https://postgresweekly.com/link/164424/web)
“是的，你没看错。空闲事务可能会导致严重的表膨胀，而清理过程可能无法解决这个问题。”


`Umair Shahid `


* 📄 Postgres 18 让您可以动态更改 Autovacuum Workers 的最大数量 - Daniel Westermann

* 📄 使用非常规设置进行测试的重要性——追踪 pgagroal 连接池中的错误所学到的教训 - Luca Ferrari

* 📄 等待 Postgres 18：默认使用 EXPLAIN ANALYZE 时启用 BUFFERS 功能- Hubert depesz Lubaczewski

* 📄 等待 Postgres 18：支持使用非确定性排序规则的 LIKE - Hubert depesz Lubaczewski

* 📄 为什么量子安全 Postgres 在今天至关重要 - Timothy Steward (富士通)


### 代码和工具：

## [pg_mooncake：Postgres 中用于分析的快速列存储表](https://postgresweekly.com/link/164444/web)
Postgres 扩展，它添加了列式存储和矢量化执行（使用 DuckDB），以便在 Postgres 中实现快速分析。列存储表作为 Iceberg 或 Delta Lake 表存储在本地文件系统或云存储中。v0.1 刚刚发布。

`Mooncake Labs`

## [🐕 pgDog：一种新的由 Rust 驱动的 Postgres 查询路由器和代理](https://postgresweekly.com/link/164446/web)
PgCat Postgres 池化器的主要开发人员已经转向开发这个以狗为主题的“精神继承者”，它提供类似的池化、负载平衡和代理，但具有插件系统和 AGPL 许可证（PgCat 是 MIT）。

`Lev Kokotov`

## [适用于 AWS Aurora DSQL 的 Ruby Active Record 适配器](https://postgresweekly.com/link/164429/web)
适用于 Amazon 新 Aurora DSQL 数据库（本质上是一种与 Postgres 兼容的无服务器分布式数据库服务）的 Active Record（Ruby on Rails）连接适配器的“最初版本”。

`Samuel Cochran`

[IvorySQL 4.2](https://postgresweekly.com/link/164431/web) – 功能齐全、开源 Oracle 兼容的 Postgres 实现，现在具有更多 Postgres 17.1 和 17.2 增强功能。

🤖 [pgai 0.4](https://postgresweekly.com/link/164432/web) – Timescale 的工具，用于在 Postgres 中与 RAG 和 LLM 配合使用。

[node-pg-migrate 7.9](https://postgresweekly.com/link/164433/web) – 从 Node.js 进行数据库迁移管理。

[ParadeDB 0.14](https://postgresweekly.com/link/164434/web) – 用于搜索和分析的 Postgres。

[pgBouncer 1.24.0](https://postgresweekly.com/link/164435/web) – 流行的连接池。


## 对 Postgres 做出贡献的奖励

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/v1737038472/eiyt8bwg12yjkywcfmpb.png)

在 LinkedIn 上，我注意到 Postgres 贡献者 Andrew Atkinson 分享了他收到的最新 Postgres 贡献者硬币的图片（上图）。多年来，此类[贡献者礼物](https://postgresweekly.com/link/164437/web)一直颁发给为 Postgres 的主要版本做出贡献的人，您可以在[此处查看最新的获奖者](https://postgresweekly.com/link/164438/web)。

祝贺大家，也许这可以激励其他人更多地参与 Postgres？这是一个很棒的荣誉！😀
