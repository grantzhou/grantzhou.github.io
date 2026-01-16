---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2023-8-9
---
### PostgreSQL每周新闻#518 - 2023年8月9日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/518)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/xxnh7tmfkpiolqqtllgq.jpg)
## [Postgres语言服务器](https://postgresweekly.com/link/143643/web)
语言服务器添加了自动完成、“转到定义”或悬停文档等功能到 VS Code 等 IDE。现在，在 Supabase 的帮助下，Postgres 有了自己的postgres_lsp。 现在还处于早期阶段，尚未考虑投入生产，但 Supabase 希望让社区参与其开发。黑客新闻上的人们当然对这种潜力感到兴奋。


`Supabase `
## [PGMQ 简介：基于 Postgres 构建的简单消息队列](https://postgresweekly.com/link/143645/web)
想象一下 AWS SQS，但在您的 Postgres 数据库中运行。PGMQ 用 Rust 编写，并在可见性超时内提供“恰好一次”传递语义。


`Adam Hendel (Tembo) `
## [更快的 Postgres](https://postgresweekly.com/link/143642/web)
PolyScale.ai 是一个完全自主的边缘分布式数据库缓存。支持 TCP 和 HTTP，可在任何平台上加速读取并降低全局延迟。只需几分钟即可部署，无需编写代码。


`PolyScale.ai `
## [Hydra 1.0 Beta：面向列的 Postgres](https://postgresweekly.com/link/143646/web)
宣传很简单： “您可以在 Postgres 上立即查询数十亿行，而无需更改代码。只需几分钟（而不是几周）即可完成并行分析。” 1.0 beta 引入了列优化清理、向量存储和相似性搜索（自然），以及用于更优化 JOIN 的新列缓存。它构建在 Citus Columnar 之上，Citus Columnar 本身是cstore_fdw扩展的现代化版本。GitHub 存储库。


`Joseph Sciarrino / Hydra `
## [使用 pgvector，维度越少越好](https://postgresweekly.com/link/143650/web)
目前使用pgvector在 Postgres 中存储 LLM 嵌入非常流行（其他向量用例确实存在，老实说），但如果你有来自 OpenAI 的数百万个 1536 维向量，那么这加起来就是一个很多字节。使用维度更少的嵌入有好处吗？


`Ricahrdson, Rice and Romanov (Supabase) `
## [为什么我的 pg_wal 不断增长？](https://postgresweekly.com/link/143652/web)
该pg_wal目录存储 Postgres 服务器的预写日志 (WAL)，如果它不断增长，您可能会责怪一两个配置设置。


`Laurenz Albe `
## [JSON 和 JSONB 之间的区别](https://postgresweekly.com/link/143654/web)
一种底层数据类型 (JSON)，但 Postgres 中有两种类型（JSON 和 JSONB）。弗朗西斯科解释了原因。


`Francesco Tisiot `
## [使用 PostGIS 再现 XKCD 的“不良地图投影”](https://postgresweekly.com/link/143655/web)
流行的网络漫画XKCD有一条展示longitude=abs(longitude)地图的条带（例如，西经 45 度和东经 45 度将位于同一个位置）。为了尊重这个奇怪的概念，Paul 开始欺骗 PostGIS 渲染同样的东西。


`Paul Ramsey `
## [CloudNativePG 主要 Postgres 升级的现状](https://postgresweekly.com/link/143657/web)
CloudNativePG是 EDB 为 Postgres 提供的开源 Kubernetes 操作器。


`Gabriele Bartolini (EDB) `
## [Pigsty 2.2：“包含电池”的 Postgres 发行版](https://postgresweekly.com/link/143660/web)
一个名称奇怪的 Postgres 发行版，自称为“免费 RDS”。本质上有很多预捆绑的扩展、可观察性、自我修复 HA，现在我们投入了大量精力来改进 Pigsty 的仪表板，您可以在这个演示网站上看到。如果您想了解更多信息，还有一个官方网站。


`Feng Ruohang `
## [PGHist：存储表更改的历史记录](https://postgresweekly.com/link/143663/web)
一组有趣且相当史诗般的 PL/pgSQL 过程（不，它不是扩展），它在指定模式中动态创建触发器以审核表更改。GitHub 存储库。


`PGSuite `


`轻松迁移您的 Heroku Postgres 数据库`
## [RisingWave：具有“类似 Postgres”体验的分布式 SQL 流处理](https://postgresweekly.com/link/143666/web)
RisingWave是非Postgres的新数据库之一，但通过有线协议兼容性向 Postgres 生态系统开放。您可以在这篇介绍性文章中了解更多信息。


`RisingWave Labs `
## [SQLedge：在边缘将 Postgres 复制到 SQLite？](https://postgresweekly.com/link/143668/web)
Alpha/实验性 Go 支持的 Postgres 代理，使用本地 SQLite 数据库进行读取并将写入转发到上游 Postgres 服务器。


`Zak Knill `
## [PLV8 3.2](https://postgresweekly.com/link/143669/web)
 -  Postgres 的 JavaScript 语言插件。v3.2 改进了 Postgres 16 支持，但放弃了Windows 支持（至少目前是这样）。


`pgwire 0.16 – Rust 库中的 Postgres 线路协议。`


`Patroni 3.1  -  Postgres 高可用性模板。`


`ORAFCE 4.5  -  Postgres 的 Oracle 兼容性函数。`
## [DBLAB 0.21](https://postgresweekly.com/link/143673/web)
↳Postgres、MySQL 和 SQLite3 的交互式 CLI 客户端。


`pspg 5.8 – 用于表格数据的 Unix 分页器。`


`Psycopg 3 v3.1.10  - 下一代 Python 数据库适配器。`


`psycopg 2 v2.9.7  - 和上一代..😉`


# 💡本周提示


**🗓即将举办的Postgres活动**
