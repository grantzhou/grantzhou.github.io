---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2022-11-30
---
### PostgreSQL每周新闻#483 - 2022年11月30日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/483)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,e_trim,w_350,h_100/e_make_transparent/co_white,e_outline:7/lhwcvgc1asd4fzaahty4.png)
## [索引合并与复合索引](https://postgresweekly.com/link/132300/web)
使用复合索引（又名多列索引）是否比合并索引更快？ 是的，至少在 Postgres 中，很多，因为当查询涉及索引合并时，Postgres 不支持仅索引扫描。


`Simon Hørup Eskildsen `
## [电子书：如何为您的查询创建最佳 Postgres 索引](https://postgresweekly.com/link/132299/web)
了解如何为您的查询创建最佳 Postgres 索引。 我们深入探讨了索引类型、运算符、数据类型等。 创建正确的索引通常可以将查询性能提高 10 倍甚至 100 倍。


`pganalyze `
## [使用窗口函数进行百分比计算](https://postgresweekly.com/link/132302/web)
与其获取数据然后对其执行百分比计算，不如在一个查询中完成所有操作？ 窗口函数的完美用例，Paul 说，他给出了一个实际示例，以及一个指向交互式沙箱的链接，您可以在其中自己玩。


`Paul Ramsey `
## [Fly.io 如何运行其新的 Postgres 平台](https://postgresweekly.com/link/132304/web)
我们是 Fly（一种分布广泛的现代 Heroku-a-like）的忠实粉丝，所以看到他们构建自己的平台很有趣。 运行 Postgres 非常简单，但诀窍在于管理副本、故障转移等，而 Fly 使用完全开源的部分来使其全部工作。


`Nicoll and Davis (Fly) `
## [AWS Database Migration Service 添加托管模式迁移](https://postgresweekly.com/link/132308/web)
AWS Database Migration Service (DMS) 是一项长期存在的服务，用于将数据库（尤其是在 Oracle 或 SQL Server 上运行的数据库）迁移到 AWS。 在本周的 re:Invent 大会上，AWS 推出了一个新的自动数据库架构转换器，作为该服务的一个组成部分。 它支持从 SQL Server 2008+ 和 Oracle 10.2+、11g-12.2、18c 和 19c 迁移到在 RDS 上运行的 MySQL 或 Postgres。


`Channy Yun (AWS) `
## [📅 注册 Unblock - Buildkite 的 CI/CD 会议](https://postgresweekly.com/link/132309/web)
📅  


`Buildkite `
## [使用 Postgres 作为 Rowdy Gophers 的任务队列](https://postgresweekly.com/link/132310/web)
一位开发人员讲述了他在 Postgres 之上构建快速高效排队系统的经验，以便他的 Go 例程用于分配工作。

## [如何在 TimescaleDB 中使用宽表布局降低查询成本](https://postgresweekly.com/link/132311/web

`FLORIAN HERRENGT`

`Manav at Ente `
## [从 Postgres 模式创建 D2 ERD 图](https://postgresweekly.com/link/132312/web)
一个简单的节点脚本，可以使用 D2 声明性图表 DSL 将 Postgres 数据库的模式转换为优雅的图表。 （同样有趣的是这个脚本依赖于一次获取模式的大型 SQL 查询。）


`Zeke Nierenberg `
## [pgvector：向量相似性搜索扩展](https://postgresweekly.com/link/132315/web)
支持 L2 距离、内积和余弦距离。 还有一整套适用于 Node、Go、Ruby、PHP、Rust 等的客户端库。


`pgvector `
