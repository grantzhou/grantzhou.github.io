---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2023-7-26
---
### PostgreSQL每周新闻#516 - 2023年7月26日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/516)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/v7rbnepgzc8ey5fs1uke.jpg)
## [给初学者的 10 个 Postgres 技巧](https://postgresweekly.com/link/142993/web)
作者是 🎤 Postgres.fm 播客的联合主持人之一，他和他的联合主持人提出了一些解释透彻、深思熟虑的技巧。 诚然，它们处于入门级水平，但仍然值得一看。


`Nikolay Samokhvalov (Postgres․ai) `
## [🕒 时间和时间戳数据类型的复杂性](https://postgresweekly.com/link/142996/web)
全面了解使用 TIMESTAMP 和 TIMESTAMPTZ 等类型的实用性、它们的相关函数和运算符，以及如何在查询中使用时区。


`Oliver Tan (Cockroach Labs) `
## [我们致力于提供出色的 Postgres 支持](https://postgresweekly.com/link/142992/web)
“Crunchy 是一种多么不同的支持体验啊。它不仅及时、信息丰富、还很切合主题。我们鼓励提出问题。与我们合作，我们能够做更多的事情 一个和我们一样关心数据的合作伙伴。” Rob Sullivan。


`Crunchydata `
## [在 Postgres 中使用 JSON(B) 的基础知识](https://postgresweekly.com/link/142997/web)
这是一种非常简洁的交互式方式，用于了解 Postgres JSON 的强大功能，包括在基于浏览器的 Postgres 环境中操作、查询、保存和优化简单的对象结构。


`Crunchy Data `

**本周摘要：**
*   DigitalOcean 的托管 Postgres 服务现在支持 pgvector 扩展。


*   📅 PGConf NYC 2023 将于今年 10 月在纽约市举行，刚刚发布了完整的日程安排，包括 Andy Pavlo 的主题演讲、Claire Giordano、Bruce Momjian、Ryan Booz 等人的演讲。


*   Timescale 不满足于挑战时间序列数据索引和查询的极限，现在将转向向量和人工智能，您可以对当前称为 Timescale Vector 的服务注册初步了解。


*   Postgres 15 现已在 Azure Database for PostgreSQL 灵活服务器上正式发布。


*   我们最近分享了 PostgreSQL 社区协会（管理“PostgreSQL”商标）的最新动态，介绍了该协会为捍卫该商标免受西班牙 Postgres 倡导团体涉嫌侵权而采取的行动。 Fundación PostgreSQL 的 Álvaro Hernández 予以回击，“Postgres 核心团队试图关闭 Postgres 社区会议”——看来这个事件还会持续一段时间。


## [分区会损害性能吗？](https://postgresweekly.com/link/143005/web)
......使用太多分区将显着增加规划器完成其工作所需的时间。 拥有数百个分区很容易导致真正的大灾难。


`Hans-Jürgen Schönig `
## [▶ Postgres 现在可以做什么？](https://postgresweekly.com/link/143006/web)
▶37 分钟的演讲，涉及各种主题，例如数据透视表、窗口函数和行级安全性。


`Vagmi Mudumbai `
## [如何衡量网络对 Postgres 性能的影响](https://postgresweekly.com/link/143007/web)
在大多数情况下，Postgres 与使用它的应用程序不在同一服务器上运行，因此网络可能会对性能产生影响。 尽管如此，从数据库方面衡量这种影响并不是特别容易，但是来自 pg_stat_activity 的 “等待事件”信息可以提供一些线索。


`Jobin Augustine `
## [PostgresML 如何从 Canonical Rust SDK 生成 JS 和 Python SDK](https://postgresweekly.com/link/143008/web)
PostgresML 是一个将机器学习功能添加到 Postgres 中的扩展。 它的团队喜欢并且更喜欢 Rust，但它的大多数用户都使用 JavaScript 或 Python。 该怎么办？ 使用 Rust 同时编写多语言库..


`Silas Marvin (PostgresML) `
## [▶ 如何在 Amazon RDS Postgres 上启用更改数据捕获](https://postgresweekly.com/link/143010/web)

`GUNNAR MORLING`
## [PgCat 1.1：现代 Postgres 池化器和代理](https://postgresweekly.com/link/143011/web)
PgCat 采用 Rust 构建，提供对分片的支持（包括实验性地基于 SQL 语法）、负载平衡和故障转移支持。 v1.1 添加了对准备好的语句和服务器 TLS 连接的支持。


`PostgresML `

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/qiaelobszxsekguxdthj.jpg)

## [推出适用于 Postgres 的新 pganalyze VACUUM Advisor](https://postgresweekly.com/link/143013/web)

`pganalyze`
## [libpqxx 7.8：Postgres 的官方 C++ 客户端 API](https://postgresweekly.com/link/143014/web)
他们说有很多好处。 C++17 用户可以获得一个新的数组类来处理 SQL 数组、更快的大型数据集流、大量错误修复、改进的异常等等。


`Jeroen Vermeulen `
## [Aquameta 0.4：基于 Postgres 构建的 Web 堆栈](https://postgresweekly.com/link/143016/web)
围绕多个 Postgres 扩展组织的 “全数据库” Web 开发扩展。


`Aquameta `
## [PgBouncer 1.20.0：轻量级连接池](https://postgresweekly.com/link/143017/web)
使用新的 track_extra_parameters 设置更好地支持跟踪 PG 设置，该设置可与 Citus 12+ 结合使用来跟踪 search_path。 现在，它还默认使用 TLS 进行连接，并且各种错误已得到解决。


`PgBouncer Team `
## [从 Oracle 到 Postgres 的迁移：7 个使之成为可能的工具](https://postgresweekly.com/link/143018/web)

`ODED VALIN (EVERSQL)`