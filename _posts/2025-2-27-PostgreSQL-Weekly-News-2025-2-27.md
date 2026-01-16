---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-2-27
---
### PostgreSQL每周新闻#590 - 2025年2月27日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/590)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/w3pouwxokxckx0tukifx.jpg)
## [用 pgRouting 将 Postgres 用作图形数据库](https://postgresweekly.com/link/166212/web)
pgRouting 是一个提供地理空间路由功能的扩展，通常与 PostGIS 一起使用。但令人惊讶的是，它的图形和路径搜索机制可用于导航以图形形式构建的任何数据。

`Paul Copplestone (Supabase)`

## [Postgres 17.4、16.8、15.12、14.17 和 13.20 发布](https://postgresweekly.com/link/166214/web)
这使得所有维护的发布线在短短几周内出现两次波动（这是一个“周期外”发布 - 解释如下）。与以前一样，重点是错误修复。Postgres 17 修复了 pg_createsubscriber 中的内存泄漏，并对 libpq 中的引用函数行为进行了调整。


`PostgreSQL Global Development Group `
## [不要让 Postgres 维护出现漏洞并让性能一落千丈](https://postgresweekly.com/link/166211/web)
确保您能够学习主动维护和监控实践，以便在数据库中隐藏的性能风险（例如查询速度慢、检查点行为和连接问题）升级之前发现它们，并确保数据库的可靠性。


`pganalyze `

### 本周摘要：

* 🌍 你有没有想过，当 Bruce Momjian 环游世界宣传 Postgres 时，他的生活是怎样的？[EDB 的 Caroline Pickens 回顾了 Bruce 最近参加的几次 Postgres 活动](https://postgresweekly.com/link/166215/web)——他肯定比我更有活力（而且穿衣品味更好）！

* Postgres 的下一个版本将获得在 [pg_upgrade 期间传输统计数据的功能](https://postgresweekly.com/link/166216/web)。

* [Laravel Cloud](https://postgresweekly.com/link/166217/web) 是一个新的官方托管平台，用于使用流行的 PHP 框架构建的应用程序。它的数据库层？无服务器 Postgres！

* EDB 委托了一个独立的基准测试，将其基于 Postgres 的数据库与 Oracle、SQL Server、MongoDB 和 MySQL 在性价比和原始速度等方面进行比较。毫不奇怪（因为他们发布了结果），[EDB 的 Postgres 更快、更便宜](https://postgresweekly.com/link/166218/web)。

* 🇩🇪 [第九届德国 PostgreSQL 大会的报名现已开放。它将于今年 5 月在柏林举行](https://postgresweekly.com/link/166219/web)。


## [当 Postgres 红线出现时，Robinhood 进行分片以扩大规模](https://postgresweekly.com/link/166220/web)
一位曾在 Robinhood 工作的工程师写了一篇简短的文章，介绍了该公司遇到的 Postgres 扩展问题以及分片如何拯救了他们。


`Tom Linford`
## [EdgeDB 现在是 Gel（而 Postgres 是未来）](https://postgresweekly.com/link/166221/web)
Gel（以前称为 EdgeDB）是“Postgres 之上的集成数据平台”，它提供自己的查询语言，试图解决 SQL 的缺陷（这里有更好的解释）。


`Elvis Pranskevichus (Gel)`


* 📄 [使用 PASSING 和 JSON_TABLE() 进行计算](https://postgresweekly.com/link/166223/web) Dave Stokes

* 📄 [使用 Ent、Atlas 和 pgvector 在 Go 中构建 RAG 系统](https://postgresweekly.com/link/166224/web) Rotem Tamir (Ent)

* 📄 [Postgres 的聚合过滤器将如何让您失望](https://postgresweekly.com/link/166225/web) Dave Stokes

### 代码和工具：

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/g3dqd4hiikvsvy8dyr9n.jpg)

## [pg_activity 3.6：类似 top 的活动监控工具](https://postgresweekly.com/link/166226/web)
就像您使用 top 或 htop 来监控进程和 CPU 使用率一样，pg_activity 可以让您在 Postgres 的后台看到正在运行的查询、最新的性能统计数据等。

`Dalibo`
## [BemiDB：Postgres 的零 ETL 数据仓库](https://postgresweekly.com/link/166227/web)
开源，但具有商业角度的更多企业功能，用 Go 编写的 BemiDB 充当 Postgres 读取副本（因此您的所有数据都会自动同步），针对分析工作负载进行了优化。

`Bemi Technologies, Inc.`


[rsql 0.16](https://postgresweekly.com/link/166229/web) – 基于 Rust 的现代 psql 式 CLI，用于处理 Postgres、DuckDB、MySQL、Redshift、SQLite3、SQL Server 和其他数据库。

[PostgreSQL Embedded 0.18](https://postgresweekly.com/link/166230/web)– 一种将 Postgres 分发和嵌入到其他应用程序中的机制，“类似于您使用 SQLite 的方式”。

[River 0.18](https://postgresweekly.com/link/166231/web) – 适用于 Go 的快速可靠的 Postgres 后台作业。

[pgrx 0.13](https://postgresweekly.com/link/166232/web) – 一种使用 Rust 构建 Postgres 扩展的方法。