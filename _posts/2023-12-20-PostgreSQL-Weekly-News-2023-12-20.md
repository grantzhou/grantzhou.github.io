---
layout: post
title: PostgreSQL 每周新闻 2023-12-20
---
### PostgreSQL每周新闻#535 - 2023年12月20日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/535)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/i8d5jxu85x1n4rwkzowr.jpg)
## [Postgres 中的事务隔离解释](https://postgresweekly.com/link/149202/web)
尽管数据库事务的概念已经很古老了，但它们仍然让最勤奋的开发人员感到困惑，隔离在影响并发事务交互方式方面的作用增加了另一个层面的复杂性。 GWEN 在这本关于这个主题的入门书中做得很好。


`Gwen Shapira `
## [外键损坏：怎么会发生这种情况？](https://postgresweekly.com/link/149203/web)
在 PostgreSQL 中，有很多方法会导致外键损坏，”Laurenz 说道，他在这里展示了一些这样的方法。 如果您的外键出现问题，需要注意一些细节，记住这些细节可能会很有价值。

`Laurenz Albe `
## [Ryan Booz 的 PostgreSQL 基础知识](https://postgresweekly.com/link/149201/web)
在本系列文章中，Ryan Booz 将帮助 PostgreSQL 新用户掌握从角色和权限开始的基础知识。


`Redgate `
## [📊 完整的 2023 年 PostgreSQL 调查结果](https://postgresweekly.com/link/149204/web)
就在他们向我们展示最新调查结果一周后，Timescale 放弃了来自 888 名受访者的完整报告和原始（但匿名）数据。


`Timescale `
## [在 PostGIS 中使用 GPS 数据](https://postgresweekly.com/link/149206/web)
在 PostGIS 中导入和细化 GPS 数据的实用分步演练，重点是消除不准确性并提高实际使用的质量，并配有代码和示例。


`Ryan Lambert `
**本周摘要：**

*   基于 Fly 微虚拟机的托管平台引入了名为 Fly Postgres 的托管 Postgres 产品，该产品基于 Supabase 平台，但托管在 Fly 上。


*   Elizabeth Christensen 对最近的 2023 年 PostGIS Day 进行了总结。


*   Tembo Postgres 平台刚刚宣布筹集了 700 万美元的资金。 它的主张是将 Postgres 视为一个数据平台，而不仅仅是一个数据库。


*   Ubicloud 有一项新的托管 Postgres 服务，该服务专门宣传自己可以在德国流行的低成本服务器提供商 Hetzner 上使用。


*   Supabase 在过去一周有如此多的更新，他们不得不写一篇十大发布帖子。


## [提高 Amazon RDS 和 Aurora 上的性能和事件的可见性](https://postgresweekly.com/link/149214/web)


`VALTER REHN (AWS)`
## [79 个（且还在增加）Postgres HOWTOs/教程](https://postgresweekly.com/link/149215/web)


`NIKOLAY SAMOKHVALOV`

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/vocho151qkpv9avjq3yk.jpg)

## [pg_idkit：用于生成 ID 的扩展](https://postgresweekly.com/link/149216/web)
Rust 构建的扩展，可以生成从 UUID 到 NanoID 和 ksuids 的无数不同的唯一 ID 方案。 它在生产中成熟且快乐。 作者说：“我只是在半自动发布过程中投入了很多精力，并确保可以轻松地在容器中以 RPM 的形式运行扩展，并在基于 glibc 的系统上进行常规安装。”


`VADOSWARE LLC `

## [使用相同的 Postgres 本地、云或混合环境降低成本并简化您的 Postgres 资产](https://postgresweekly.com/link/149217/web)


`EDB Postgres`
## [pg_sparse：Postgres 中的稀疏向量相似性搜索](https://postgresweekly.com/link/149218/web)
ParadeDB 是一个基于 Postgres 的开源 ElasticSearch 替代品，他们创建了一个扩展（从 pgvector 分叉）来存储和使用 Postgres 中的稀疏向量，以进一步扩展它：“pg_sparse 是稀疏的 向量就像 pgvector 与稠密向量一样。”


`ParadeDB `
## [sqlauthz：一种声明式权限管理方法](https://postgresweekly.com/link/149220/web)
该工具使您能够使用 Polar 语言以声明式方式管理 Postgres 中的权限。 请注意，它被认为是实验性的


`Cam Feenstra `
## [🪐 Q3C：球体上空间索引的扩展](https://postgresweekly.com/link/149222/web)
我的天文学知识很薄弱，但显然这个扩展对于处理天体在天球上的位置很有用。 或许。


`Sergey Koposov `
## [每个开发人员从 Oracle 迁移时必须了解的关键 Postgres 扩展](https://postgresweekly.com/link/149223/web)
方便的综述。


`Deepak Mahto `
## [FerretDB 1.17.0](https://postgresweekly.com/link/149224/web)
类似 MongoDB，但位于 Postgres（或 SQLite）之上。

## [PLV8 3.2.1](https://postgresweekly.com/link/149225/web)
在 Postgres 中使用 V8 JavaScript 引擎。

## [hYDRA 1.1](https://postgresweekly.com/link/149226/web)
面向列的 Postgres

## [pgAdmin 4 v8.1](https://postgresweekly.com/link/149227/web)
流行的管理工具。


附： 上周我们链接到了 Supavisor 连接池程序的 v1.0 版本，但现在 Supabase 有一篇关于它的完整博客文章。
附言 两周后见！

