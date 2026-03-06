---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-2-13
---
### PostgreSQL每周新闻#588 - 2025年2月13日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/588)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/rg252ht4gr5tdyuipsea.jpg)
## [无需费尽心机即可扩展 Postgres](https://postgresweekly.com/link/165750/web)
Postgres 在默认设置下可以扩展很多功能，但一旦服务器开始承受一些严重的负载，“奇怪的问题”就会开始出现。Shayon 解决了一些此类常见问题及其解决方案。

`Shayon Mukherjee`

## [SQL 中的尾随逗号怎么样？](https://postgresweekly.com/link/165751/web)
这可能是最简单但要求最多的 SQL 功能吗？它已在某些方言中实现，但它可以在 Postgres 的方言中实现吗？应该吗？这比听起来要棘手得多。


`Peter Eisentraut `
## [使用 Heroku Postgres 找到您的流程](https://postgresweekly.com/link/165749/web)
世界上最先进的开源数据库比以往更易于使用。借助 Heroku 的 PostgreSQL 数据库服务，您可以充分利用您的数据，并将管理工作交给我们。因此，请继续专注于您的数据驱动型应用 — 我们为您提供帮助。


`Heroku Postgres `

### 本周摘要：

* 🤖 是否可以使用本地[免费 LLM（本例中为 Phi 4）来学习有关 Postgres 的任何知识](https://postgresweekly.com/link/165752/web)，并让它帮助构建 JSONB 查询？令人惊讶的是，是的。

* [Postgres 17 现已在 DigitalOcean 的托管 Postgres 服务上提供](https://postgresweekly.com/link/165753/web)。

* Timescale 团队总结了[八个基本的 Postgres 扩展](https://postgresweekly.com/link/165754/web)，以及如何安装和使用扩展的入门指南。令人惊讶的是，TimescaleDB 不在这八个中！:-)

* 🎤 [Robert Haas 在 Talking Postgres 播客上谈到了指导想要从事 Postgres 项目的开发人员的重要性](https://postgresweekly.com/link/165755/web)。


`Timescale`
## [处理“在 relfrozenxid 之前找到 xmin ...”](https://postgresweekly.com/link/165756/web)
查看一个经常报告的错误，其措辞容易被误解。当未冻结元组的 xmin 早于表的 relfrozenxid 时，它会在清理过程中发生（并中断），表明数据损坏。幸运的是，有解决方案。


`Laurenz Albe`

### 代码和工具：

## [Citus 13：现在支持 Postgres 17](https://postgresweekly.com/link/165760/web)
Citus 是一个长期存在的开源扩展，可以更轻松地水平扩展 Postgres。几年前被微软收购后，它不断发布新版本，包括这个支持 Postgres 17 的新版本，包括使用 JSON_TABLE() 进行分布式查询和对分布式分区表的改进支持。

`Naisila Puka (Citus Data)`

## [锁匠：快速检测 SQL 迁移问题](https://postgresweekly.com/link/165761/web)
一种新的由 Rust 提供支持的工具，用于在模式迁移期间检测表锁、表重写以及修改的表、列和索引。

`Tom Forbes`

## [pgroll 0.9.0 发布，具有新的模式迁移功能](https://postgresweekly.com/link/165762/web)
pgroll 是一种在不关闭数据库的情况下在 Postgres 上执行可逆模式迁移的工具。v0.9 支持在表创建过程中添加表级约束以及生成的列。

`Andrew Farries`

## [Pig v0.1.4：现在有 400 个 Postgres 扩展](https://postgresweekly.com/link/165764/web)
Pig（Postgres Install Genius 的缩写）是较新的尝试之一，旨在以基于包的方式管理 Postgres 扩展。最新版本增加了对 Microsoft 的 DocumentDB、pg_tracing、pg_cooldown、VectorChord-bm25 等的支持。

`Pigsty`


### 📰 分类广告
要从 Oracle 迁移到 Postgres？阅读这份深入指南，了解如何[用 pg_hint_plan 等效项替换 Oracle 提示](https://postgresweekly.com/link/165766/web)以及何时不使用提示。

📑 使用 [Datadog 的便捷备忘单](https://postgresweekly.com/link/165767/web)开始跟踪 PostgreSQL 数据库中的重要资源和活动指标。


[PeerDB 0.25](https://postgresweekly.com/link/165768/web) – 将数据从 Postgres 流式传输到数据仓库、队列和存储引擎。

[pgxmock 4.5](https://postgresweekly.com/link/165769/web) – 模拟驱动程序，用于在 Go 中测试 Postgres 交互。

[Bytebase 3.4.0](https://postgresweekly.com/link/165770/web) – 协作数据库开发平台。

[RisingWave 2.2](https://postgresweekly.com/link/165771/web) – 与 Postgres 兼容的流式数据库。

[postgres-meta 0.86](https://postgresweekly.com/link/165772/web) – 用于管理 Postgres 的 RESTful API。

[DoltgreSQL 0.17](https://postgresweekly.com/link/165773/web) – 版本控制的 Postgres 类似版本。