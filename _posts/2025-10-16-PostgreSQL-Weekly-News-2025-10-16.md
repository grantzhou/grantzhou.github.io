---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-10-16
---
### PostgreSQL每周新闻#620 - 2025年10月16日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/620)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/e692qah5p8cek2vviye8.jpg)
## [对 Postgres 17 与 18 进行基准测试](https://postgresweekly.com/link/175714/web)
作者在 Postgres 17 和 18 之间进行了一系列详细的性能基准测试，大约有 96 种组合，令人欣慰的是，Postgres 18 为我们带来了良好的性能提升、本地磁碟规则，并且调整设置仍然是值得的。

`Ben Dicken (PlanetScale)`


## [note.com 如何实现即时 (JIT) 资料库存取控制](https://postgresweekly.com/link/175713/web)
note.com 是日本领先的 C2C 创作者平台，它用 Bytebase 的即时 (JIT) 访问控制取代了用于临时 Aurora Postgres 访问的内部 GitHub Actions + SSH 代理流。

`Bytebase `

## [PGConf NYC 2025 的 Postgres 之旅报告](https://postgresweekly.com/link/175385/web)
PGConf NYC 2025 于两周前举行，取得了巨大成功。以播客 Talking Postgres 闻名的 Claire 详细讲述了此次活动的点滴，并分享了许多精彩的照片。

`Claire Giordano (Microsoft) `

[EDB 团队也回顾了 PGConf NYC 的主要内容](https://postgresweekly.com/link/175717/web)。

## [▶ Postgres 18 实作：非同步 I/O、B 树跳跃扫描、UUIDv7](https://postgresweekly.com/link/175388/web)
pganalyze 的创办人举办了一场网路研讨会，深入探讨了 Postgres 18 中一些更值得注意的改进。关于非同步 I/O 的部分（从 4:20 到 22:30）特别有用。

`Lukas Fittl `

### **本周摘要**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/kgq3heua484bbrb3amtp.jpg)

* JetBrains 发布了[其最新的开发者生态系统现状报告](https://postgresweekly.com/link/175719/web)（见上文），Postgres 首次超越 MySQL，成为 JetBrains 生态系统中最受欢迎的资料库系统。

* Heroku 常被誉为 Postgres 云端平台/服务概念的先驱，近日，Heroku [发布了「下一代」Heroku Postgres 的预告](https://postgresweekly.com/link/175720/web)，将其提升到了更高的规模。

* 🇨🇿 [2026 年布拉格 PostgreSQL 开发者日](https://postgresweekly.com/link/175721/web)将于明年 1 月 27 日至 28 日在捷克共和国举行。如果您想发言，其提案征集截止日期为 11 月 14 日。

* 微软 Azure 团队分享了 Azure Database for PostgreSQL [2025 年 9 月新功能的综述](https://postgresweekly.com/link/175723/web)。

* 一个使用 Postgres 和 SQL [解决逻辑难题的精彩范例](https://postgresweekly.com/link/175724/web)。


## [探索 Postgres 18 新增的 UUIDv7 支援](https://postgresweekly.com/link/175725/web)
与 UUIDv4 不同，UUIDv7 值具有单调性且可按时间排序，这带来了一些优势。


`Fridriksson and Miller (Aiven)`

📄 [从文本到标记](https://postgresweekly.com/link/175726/web)：标记化管道的工作原理 James Blackwood-Sewell

📄 [理解并设定 Postgres JDBC 的获取大小](https://postgresweekly.com/link/175727/web) Shane Borden


## **发布**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/rrsyyhvvev1npg7ro4z5.jpg)

## [pqr.sql：在 Postgres 中使用纯 SQL 产生二维码](https://postgresweekly.com/link/175728/web)
这个想法很巧妙，但可能有一些不太明显的用例。不过，它确实需要几百行 SQL 才能实现。

`Tanel Põder`

## [PGSync 5.0：Postgres 到 ElasticSearch/OpenSearch 的同步](https://postgresweekly.com/link/175730/web)
一款中间件，用于撷取资料库中的变更并将结构化文件写入搜寻丛集。 v5.0 最初仅适用于 Postgres，现已新增 MySQL/MariaDB 支援。 GitHub 程式码库。

`Tolu Aina`

## [使用 SQL 清理 SQL](https://postgresweekly.com/link/175732/web)
一种概念验证 PL/pgSQL 函数，可以取得原始 SQL 并传回经过清理的版本（不含任何个人识别资讯）。

`Jeremy Schneider`

## [pg_qualstats：用来收集谓词统计资料的扩充](https://postgresweekly.com/link/175733/web)
分析资料库查询中最常用的谓词，或许可以以此创造最有效的索引。 POWA（Postgres 工作负载分析器）专案的一部分。

`Powa Team`

[BemiDB 1.7](https://postgresweekly.com/link/175735/web) – 开源 Snowflake 与 Fivetran 替代方案捆绑在一起。

[ParadeDB 0.19](https://postgresweekly.com/link/175736/web) – 基于 Postgres 建构的事务型 Elasticsearch 替代方案。

[PgDog 0.1.10](https://postgresweekly.com/link/175737/web) – 支援 Postgres 的水平扩展和自动分片功能。