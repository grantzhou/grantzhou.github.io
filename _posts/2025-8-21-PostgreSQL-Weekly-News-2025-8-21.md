---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-8-21
---
### PostgreSQL每周新闻#612 - 2025年8月21日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/612)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/ucqadf2e63yxb6fh3ac7.jpg)
## [Postgres 日志性能优化](https://postgresweekly.com/link/173127/web)
一篇关于日志记录的详尽文章，这个主题很容易被忽视。Elizabeth 从头到尾讲解了这个主题，涵盖了日志记录级别、选择需要记录的查询、日志格式、日志轮换以及日志处理方法。

`Elizabeth Christensen`

## [专为您的团队打造的 Postgres 性能研讨会](https://postgresweekly.com/link/173126/web)
专家指导，专为您的数据库打造的研讨会，面向拥有大量 Postgres 数据的团队。学习如何调优慢查询、选择合适的索引并预防事件。您是 pganalyze 的新手吗？这正适合您。立即申请。

`pganalyze  `

## [Postgres 17.6、16.10、15.14、14.19、13.22 和 18 Beta 3 发布](https://postgresweekly.com/link/173129/web)
Postgres 的每个受支持版本的发布都已发布（以及即将发布的 Postgres 18 的第三个测试版 - 最终版本预计在大约一个月后发布）以解决一些安全漏洞并部署大量错误修复。

`PostgreSQL Global Development Group `

### **本周摘要**

* 🌐 如果您想尝试 [PlanetScale 的全新 Postgres 产品](https://postgresweekly.com/link/173130/web)，但又不喜欢等待，那么本周所有等待名单上的用户都将受邀加入。他们还整理了一份指南，介绍[如何将现有的 Postgres 数据库迁移到他们的平台](https://postgresweekly.com/link/173132/web)。

* [Curt Kolovson](https://postgresweekly.com/link/173133/web) 是最新一期的 PostgreSQL 本周人物访谈嘉宾。

* 🎤 一向精彩的 [Postgres FM](https://postgresweekly.com/link/173134/web) 播客的最新一期探讨了[“自动驾驶”Postgres](https://postgresweekly.com/link/173135/web)（即自动调优和维护）的概念。

* Neon 托管的 Postgres 平台采用了一种[新的基于使用量的定价模式](https://postgresweekly.com/link/173153/web)，本质上是“按需付费”，最低费用为 5 美元/月。


## [SSD 的趣味与奇特之处](https://postgresweekly.com/link/173136/web)
调查查询性能如何受到 SSD 怪癖的影响，而成本模型无法预料。


`Tomas Vondra`

## [在 Postgres 中索引 JSONB](https://postgresweekly.com/link/173137/web)
如何从检索角度充分利用 JSONB？了解 Postgres 丰富的索引支持。


`Craig Kerstiens`


📄 [向量搜索并非万能，那究竟是什么？](https://postgresweekly.com/link/173138/web)—— 使用 Postgres 和 pgvector 构建混合搜索解决方案的实践探索。Jacky Liang (TigerData)

📄 [使用直接分区哈希计算绕过 Postgres 目录开销](https://postgresweekly.com/link/173139/web) Shayon Mukherjee

📄 [为什么 Postgres 是持久工作流执行的理想选择](https://postgresweekly.com/link/173140/web) Peter Kraft (DBOS)


📰 分类广告
超越缓存。与 7.2 相比，Redis 8.2 新增了 150 条命令和 8 种数据结构，处理数据量提升了 5 倍。[立即开始使用吧](https://postgresweekly.com/link/173141/web)！

💌 你知道我们有一系列新闻简报吗？查看 [JavaScript](https://postgresweekly.com/link/173142/web) Weekly、[Go Weekly](https://postgresweekly.com/link/173143/web) 和 [Ruby Weekly](https://postgresweekly.com/link/173144/web)，更全面地了解我们的工作。


### **发布**

## [VectorChord 0.5：可扩展、快速且磁盘友好的向量搜索](https://postgresweekly.com/link/173145/web)
一个适用于 Postgres 的开源（AGPLv3 或 ELv2）向量搜索扩展，它与 pgvector 的数据类型和查询语法兼容，并有望显著提升性能。GitHub 仓库。

`TensorChord Inc.`

## [BemiDB 1.0：针对分析优化的 Postgres 读取副本](https://postgresweekly.com/link/173147/web)
Snowflake/Fivetran 的替代方案，可连接不同的数据源，以压缩的列式格式将数据同步到 S3，并允许您使用与 Postgres 兼容的分析查询引擎运行复杂查询。采用 AGPL 3.0 许可证。

`Bemi`


[FerretDB 2.5](https://postgresweekly.com/link/173148/web) – 类似 MongoDB，但基于 Postgres（或 SQLite）。

[PGSync 4.2](https://postgresweekly.com/link/173149/web) – Postgres 到 Elasticsearch/OpenSearch 的同步。

[pg 10.15](https://postgresweekly.com/link/173150/web) – Go 语言的 PostgreSQL 客户端和对象关系映射 (ORM)。

[pgsql_tweaks](https://postgresweekly.com/link/173151/web) 0.11.5

[PostGIS 3.6.0 RC1](https://postgresweekly.com/link/173152/web)