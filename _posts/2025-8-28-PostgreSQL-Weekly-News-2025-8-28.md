---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-8-28
---
### PostgreSQL每周新闻#613 - 2025年8月28日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/613)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/sv56ilc9yxghvv6sdnem.jpg)
## [DocumentDB 加入 Linux 基金会](https://postgresweekly.com/link/173450/web)
DocumentDB 是一个基于 MIT 许可的文档数据库，基于微软今年早些时候开源的 Postgres 扩展构建。为了使该项目更加开放，更方便多家公司使用，微软将该项目移交给 Linux 基金会。

`Kirill Gavrylyuk (Microsoft)`

## [而且……AWS 加入 DocumentDB 项目](https://postgresweekly.com/link/173454/web)
公告（上文）的一个重要部分是 AWS 即将加入该项目，这肯定会给他们带来一些困惑，因为他们已经在运行名称相似（但在代码方面完全无关）的 Amazon DocumentDB。尽管如此，这对 Postgres 来说仍然是又一个重大胜利，因为它具有扩展友好的特性，并且任何渴望将类似 MongoDB 的功能引入 Postgres 的人都受益匪浅。

`Amazon  `

## [PostgreSQL 性能不佳？用 pgNow 诊断](https://postgresweekly.com/link/173449/web)
刚接触 Postgres 还是时间紧迫？pgNow 提供快速、精准的诊断功能，帮助您调整配置、修复性能下降并立即发现问题。无需设置，无需代理，只需极少权限。免费下载，几秒钟即可开始使用。

`Redgate `

### **本周摘要**

* 本月初，Talking Postgres 播客的 Claire Giordano ▶️ [采访了备受尊敬的法学硕士 (LLM) 专家 Simon Willison](https://postgresweekly.com/link/173456/web)（更值得一提的是，他也是 Django 的联合创始人），探讨了人工智能如何帮助当今的数据工程师，以及他更广泛的工作。

* 后续我们会再次介绍此事，[不过 Shaun Thomas 已经开始了一个关于使用 C 语言进行 Postgres 扩展开发的系列文章](https://postgresweekly.com/link/173457/web)。


## [十年数据库创新：亚马逊 Aurora 的故事](https://postgresweekly.com/link/173458/web)
亚马逊讲述了其 Aurora 服务的故事，从最初的梦想成为“云的关系数据库”到现代的无服务器方法。


`Amazon Science`

## [PostgreSQL 内部原理：简介](https://postgresweekly.com/link/173459/web)
有点儿像“金玉良言”，但会持续更新。对于想要深入了解 Postgres 底层工作原理的资深数据库用户来说，这是一本不错的指南。


`Hironobu Suzuki`


📄 [使用 JWT 为 RLS 建立可信上下文](https://postgresweekly.com/link/173460/web) Tomas Vondra

📄 [我为什么开始使用 Postgres（你可能也会](https://postgresweekly.com/link/173461/web)）—— Brent 是一位（非常）知名的 SQL Server 专家和顾问，但即使是他也看到了它的缺点。Brent Ozar

📺 [Postgres 13 已停用，以下是如何迁移到 17 版](https://postgresweekly.com/link/173462/web) PlanetScale

📄 [使用外部数据包装器进行基本的跨数据库操作](https://postgresweekly.com/link/173463/web) Julien Singler

### **发布**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/ezw7lgbxhszwe5r5rabr.jpg)


## [pg_hint_plan 1.8：使用“提示”调整查询执行计划](https://postgresweekly.com/link/173464/web)
Postgres 的查询规划器通常能够很好地找出针对数据执行查询的最佳方式，但当它需要一些额外的推动力来获得正确的结果时，它可以让您放弃一些提示。请注意，从 v1.8 开始，它仅支持 Postgres 18。

`NTT OSS Center DBMS Development and Support Team`

## [pg_cirrus 2.0：设置高可用性 3 节点 Postgres 集群](https://postgresweekly.com/link/173467/web)
在 Ubuntu 或 Red Hat 上配置一个强大、容错的集群，并尽量减少手动干预。v2.0 增加了对配置由 Pgpool 驱动的看门狗集群的支持，以避免以前设置中出现的单点故障。

`Stormatics`


[pgmoneta 0.19.0] – Postgres 的备份和恢复解决方案，支持增量备份和各种压缩方法。

[pg_parquet v0.4.3](https://postgresweekly.com/link/173471/web) – 一种在 Postgres 中直接导出和导入 Parquet 文件的方法，无需依赖第三方工具。

[pg-promise 12.0](https://postgresweekly.com/link/173472/web) – 适用于 Node.js 的 Postgres 接口。现已取消对自定义 Promise 的支持，改为“全程支持 ES6 Promise”。

[PeerDB 0.33](https://postgresweekly.com/link/173473/web) – 将数据从 Postgres 流式传输到数据仓库、队列和存储引擎。

[BemiDB 1.2](https://postgresweekly.com/link/173474/web) – 针对分析进行了优化的单二进制 Postgres 只读副本。

[PostgREST 13.0.5](https://postgresweekly.com/link/173475/web) – 适用于任何 Postgres 数据库的 REST API。

[PostGIS 3.6.0 RC 2](https://postgresweekly.com/link/173476/web) – 地理空间 Postgres 扩展。

[pgAdmin 4 v9.7](https://postgresweekly.com/link/173477/web) – 流行的 Postgres 管理工具