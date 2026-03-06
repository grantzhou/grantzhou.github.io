---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-6-12
---
### PostgreSQL每周新闻#602 - 2025年6月12日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/603)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/fyfw3cojzzqul41wwmku.jpg)
## [宣布推出 Multigres：Vitess for Postgres](https://postgresweekly.com/link/170358/web)
Vitess 是一款流行的 MySQL 集群系统，用于扩展和分片。Supabase 已聘请其创始人之一 Sugu Sougoumarane 构建 Vitess for Postgres，并运用多年来构建 Vitess 的经验。Citus 和 PgDog 也是该领域的其他选择，但 Sugu 认为还有更多可以改进的地方。

`Paul Copplestone (Supabase)`

## [AWS 开源 pgactive，其主动-主动复制扩展](https://postgresweekly.com/link/170362/web)
pgactive 是一个复制扩展，它建立在 Postgres 的逻辑复制功能之上，并添加了简化管理主动-主动复制场景的功能。GitHub 仓库。


`Amazon `

## [O’Reilly CockroachDB 权威指南（第二版）](https://postgresweekly.com/link/170357/web)
掌握如何使用基于 Postgres 的分布式 SQL 数据库构建可扩展、高弹性的应用。无论是在本地还是云端，都能享受熟悉的工具和查询，以及内置的全局扩展、地理数据控制和低 TCO。

`Cockroach Labs`

### **本周摘要**

* 🇱🇻 [2025 年 PostgreSQL CFP 大会](https://postgresweekly.com/link/170364/web)将于今年 10 月在拉脱维亚里加举行，现已开放。

* Teresa Lopes 是[最新一期 PostgreSQL 人物访谈嘉宾](https://postgresweekly.com/link/170365/web)。

* 热门 Postgres 公司 [Crunchy Data 已被“AI 数据云”公司 Snowflake 收购](https://postgresweekly.com/link/170366/web)。

## [▶ 使用 PGlite 将 Postgres 编译为 WebAssembly](https://postgresweekly.com/link/170367/web)
PGlite 是一个简洁的项目，它是 Postgres 的完整 WASM 构建，使 Postgres 能够在一些不常见的环境中运行，例如直接在浏览器中运行。本次演讲将讲解该项目以及使其运行所涉及的一些复杂因素。

`Sam Willis`

* 📄 [使用 pg_stat_statements 估算查询的 P99 值](https://postgresweekly.com/link/170370/web) Michael Christofides

* 📄 [在 Postgres 中使用正则表达式和数组——基础知识回顾](https://postgresweekly.com/link/170371/web)。Hans-Jürgen Schönig

* 📄 [不要模拟数据库：数据夹具并行安全且快速](https://postgresweekly.com/link/170372/web) Brandur Leach（Crunchy Data）

* 📄 [我希望 MySQL 拥有但 Postgres 已经拥有的功能](https://postgresweekly.com/link/170373/web) Tianzhou

* 📄 [Postgres 18 的新功能——DBA 视角](https://postgresweekly.com/link/170374/web) Tianzhou


### **代码和工具**

## [py-pglite：一个用于测试的 Python PGlite 包装器](https://postgresweekly.com/link/170375/web)
安装一个 Python 包，即可获得一个由 PGlite 驱动的 WebAssembly Postgres 实例，无需 Docker、设置或配置文件即可运行。

`Wey Gu`

## [pgrwl：零数据丢失的流式 Postgres WAL](https://postgresweekly.com/link/170376/web)
一个用 Go 编写的预写日志 (WAL) 接收器。它是 pg_receivewal 的一个嵌入式、容器友好的替代方案，支持流式复制、加密、压缩和远程存储（S3、SFTP）。

`Alexey ZH`

## [Greenmask：Postgres 数据屏蔽和混淆工具](https://postgresweekly.com/link/170378/web) 
一个由 Go 语言驱动的实用程序，用于转储 Postgres 数据库并以确定性的方式对数据进行匿名化处理。GitHub 代码库。

`Greenmask`

## [ClickPipes 的 Postgres CDC 连接器现已正式发布](https://postgresweekly.com/link/170380/web)


`Sai Srirampur (ClickHouse)`

📰 分类广告
使用此[月度性能检查清单](https://postgresweekly.com/link/170381/web)，防止 Postgres 在生产环境中速度变慢，并在问题恶化之前发现它们。

Notion 工程团队如何应对病毒式增长的用户增长，并使用 pganalyze 在 [Amazon RDS 上大规模运行 PostgreSQL](https://postgresweekly.com/link/170382/web)。


[Addax 6.0](https://postgresweekly.com/link/170383/web) – 一款快速且多功能的 ETL 工具，支持超过 20 种 SQL/NoSQL 数据源。

[Bytebase 3.7](https://postgresweekly.com/link/170384/web) – 面向团队的数据库 DevOps 和 CI/CD 系统。

[ChartDB 1.13](https://postgresweekly.com/link/170385/web) – 基于图表的开源数据库编辑器。

[🗾 Martin 0.17](https://postgresweekly.com/link/170386/web) – 基于 Rust 的快速 PostGIS 地图瓦片服务器。

[Citus 13.1](https://postgresweekly.com/link/170387/web) – 分布式 Postgres 扩展。