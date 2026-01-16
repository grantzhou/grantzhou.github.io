---
layout: post
title: PostgreSQL 每周新闻 2022-10-5
---
### PostgreSQL每周新闻#474 - 2022年10月5日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/474)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/lptsku1eiqhutlgtukyj.jpg)
## [带有 pg_eventserv 的实时数据库事件](https://postgresweekly.com/link/129642/web)
pg_eventserv 是一个新的 Go 驱动的服务器，它通过 NOTIFY 从 Postgres 获取事件，然后将这些事件传递给等待的 WebSocket 客户端。 “以这种方式构建实时系统允许任何数据库客户端更改系统状态并实时传播到所有其他客户端。”


`PAUL RAMSEY (CRUNCHY DATA) `
## [PostgreSQL 15 候选版本 1 发布](https://postgresweekly.com/link/129644/web)
在过去的几年里，主要的 Postgres 版本已经在 10 月初左右发布，我们现在正倒数计时到 10 月 13 日 Postgres 15 的最终版本。这个候选版本的与最终版本“基本相同”，但提供了一个机会来测试和捕捉最后一分钟的错误，并使扩展顺利运行。 以下是发行说明。


`POSTGRESQL GLOBAL DEVELOPMENT GROUP`
## [TimescaleDB 如何扩展 PostgreSQL 性能](https://postgresweekly.com/link/129641/web)
了解 TimescaleDB 如何将 PostgreSQL 查询性能提高 1000 倍，将存储利用率降低 90%，并为时间序列和分析应用程序提供节省时间的功能，同时仍然是 100% 的 Postgres。


`TIMESCALE `
## [直接从 DuckDB 查询 Postgres 表](https://postgresweekly.com/link/129646/web)
DuckDB（一种进程内 SQL OLAP 数据库，可能被称为“用于分析的 SQLite”）现在可以在 Postgres 运行时直接读取 Postgres 表，并运行查询以加速复杂的分析查询而无需重复数据。


`HANNES MÜHLEISEN (DUCKDB) `
## [互联网上的大多数 Postgres 服务器不安全吗？](https://postgresweekly.com/link/129656/web)
“在互联网上监听的大约 820,000 台 PostgreSQL 服务器中，最多有 15% 需要加密，”作者声称，但他进一步研究了一些 Postgres 客户端如何通过默认不使用加密来解决问题，即使这是可能的。 （标题中的“互联网上”起到了很大的提升作用，因为 Postgres 服务器通常位于防火墙后面、或专用内网里。）


`JONATHAN MORTENSEN`
## [如何深入了解 Postgres 的内部结构](https://postgresweekly.com/link/129657/web)
如果你想深入研究 Postgres 代码库，Paul 分享了一些关于学习 Postgres 如何从内部运行的便利资源的指南。


`PAUL RAMSEY `
## [为什么 VACUUM 不能让您的表变小？](https://postgresweekly.com/link/129658/web)
如果你曾经问过这个问题，那么这篇关于正在发生的事情的介绍就是为你准备的。 简而言之，您需要 VACUUM FULL - 但需要考虑权衡和替代方案。


`HANS-JÜRGEN SCHÖNIG `
## [pg_stat_monitor 1.1.0：查询性能监控工具](https://postgresweekly.com/link/129659/web)
旨在成为普遍流行的 pg_stat_statements 的“高级替代品”，用于挖掘查询起源、执行、计划统计和详细信息等。 Percona 之前写过它是如何工作的。


`PERCONA`
## [Dynaboard：专为开发人员打造的 Pro-Code Web App Builder](https://postgresweekly.com/link/129661/web)


`DYNABOARD `
## [pgBackRest 2.41：可靠的 Postgres 备份和恢复](https://postgresweekly.com/link/129662/web)
备份注释是一项新功能，用于将信息键/值对附加到备份以提供扩展信息。

`STEFAN FERCOT `
## [PL/Haskell 1.0](https://postgresweekly.com/link/129663/web)
↳ 在 Haskell 中编写 Postgres 函数。


## [Bytebase 1.5](https://postgresweekly.com/link/129664/web)
↳ 安全架构更改和版本控制工具。

## [serverless-pg 2.0](https://postgresweekly.com/link/129665/web)
↳ node-pg 的包装器，用于改进无服务器的 PG 连接。

## [Jet 2.9](https://postgresweekly.com/link/129666/web)
↳ 使用 Go(lang) 的代码生成键入安全的 SQL 构建器。

## [pg_graphql 0.4.1](https://postgresweekly.com/link/129667/web)
↳ GraphQL 对 Postgres 的支持。



