---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-8-28
---
### PostgreSQL每周新闻#567 - 2024年8月28日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/567)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/mwnjazjyigfrdpwdwtcj.jpg)
## [凯文·贝肯的六度空间 - Postgres 风格](https://postgresweekly.com/link/158955/web)
给定两个随机演员，您能否在六步之内通过其他曾一起出演电影的演员将这两位演员联系起来？这就是凯文·贝肯的六度空间游戏，Paul 着手看看 Postgres 能否解决寻找此类联系的任务。

`Paul Ramsey `

## [为什么我总是在所有事情上使用 Postgres 函数](https://postgresweekly.com/link/158957/web)
关于函数在生产数据库中的作用，有许多学派的观点，因此很多人可能不同意作者的观点。尽管如此，他解释了为什么他欣赏用户定义函数提供的封装和抽象。


`Vedran Bilopavlović `
## [免费指南：将 Postgres 性能提高 3 倍](https://postgresweekly.com/link/158954/web)
通过对数千个数据库进行调整，经过验证的实践，我们将引导您完成整个过程，使 Postgres 数据库的性能提高 3 倍，同时将磁盘数据负载减少 500 倍。


`pganalyze  `

### 本周摘要：

* 🔒 Aqua Security 的 Assaf Morag 研究了他们发现的 [Postgres 恶意软件](https://postgresweekly.com/link/158958/web)。

* [Neon](https://postgresweekly.com/link/158959/web) 无服务器 Postgres 平台已宣布其[自动缩放功能](https://postgresweekly.com/link/158960/web)全面可用。

* [Tembo](https://postgresweekly.com/link/158961/web) 推出了自己的 [Tembo AI 平台 alpha 版本](https://postgresweekly.com/link/158962/web)，该平台提供了一种通过 SQL 和 HTTP 调用 LLM 模型的方法。

## [如何使用 WebAssembly 创建 Postgres FDW](https://postgresweekly.com/link/158963/web)
外部数据包装器 (FDW) 提供了一种方法，让 Postgres 能够像查询本地表一样查询外部数据源。使用基于 Rust 的 Wrappers FDW 框架，您可以创建由 WebAssembly 提供支持的 FDW，这些 FDW 可以在运行时动态部署。


`Supabase `
## [带有 pgstream 的 Postgres Webhooks](https://postgresweekly.com/link/158965/web)
查看 pgstream 更改数据捕获工具的用例：根据 Postgres 数据和架构更改调用 webhook。


`Tudor Golubenco`
## [了解 pgvector 的 HNSW 索引存储](https://postgresweekly.com/link/158967/web)
pgvector 广泛用于在 Postgres 中实现向量相似性搜索功能，但它的索引在底层是如何存储的？


`Varik Matevosyan`

📄 [为什么 Postgres 是 Oracle 的可行替代方案](https://postgresweekly.com/link/158969/web) - 我怀疑任何 Postgres Weekly 读者都不需要说服这一点，但如果你认识任何需要的人……Umair Shahid

📄 [Ruby on Rails 应用程序中容易被忽视的 Postgres 性能问题](https://postgresweekly.com/link/158970/web) - Paweł Urbanek

📄 [为什么 Postgres 17 的增量备份功能会改变游戏规则](https://postgresweekly.com/link/158971/web) - David Wagoner 和 Tim Boutin

📄 [使用 Postgres、Mistral 和 Ollama 构建完全本地的 RAG 应用程序](https://postgresweekly.com/link/158972/web) - Haziqa Sajid (Timescale)

### 机密：

2024 年 11 月 4 日至 8 日，在西雅图举行的 PASS 数据社区峰会上，您可以了解 PostgreSQL [会议和演讲](https://postgresweekly.com/link/158973/web)。

[Dragonfly（25000 个 GitHub 星）](https://postgresweekly.com/link/158974/web) 是现代 Redis 的替代品。改用 Dragonfly 的组织可以将基础设施成本降低 80%。

### 🛠 代码和工具

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/xozxp0pigqwsvbw14z8v.jpg)

[Prisma 5.19.0：JS ORM 现在具有“类型化 SQL”](https://postgresweekly.com/link/158975/web) 
Prisma 是 Node.js/TypeScript 世界中流行的声明式驱动 ORM，其新版本可以以类型安全的方式编写原始 SQL 查询。


`Nikolas Burk`
## [pgMonitor：一个开源监控扩展](https://postgresweekly.com/link/158978/web)
pgMonitor 是 Crunchy Data 多年来一直维护的 Postgres 指标跟踪工具的名称，但它现在也可以作为开源扩展使用。


`Keith Fiske (Crunchy Data)`

[Barman 3.11.0](https://postgresweekly.com/link/158979/web) – 备份和灾难恢复工具。现在支持 Postgres 17 的增量备份。

[Pongo 0.13](https://postgresweekly.com/link/158980/web) – Node.js 的 Postgres 驱动程序，以 MongoDB 样式 API 的形式呈现。

[pg-boss 10.0](https://postgresweekly.com/link/158981/web) – 基于 Postgres 的 Node.js 作业排队系统。

[postgres-meta 0.84](https://postgresweekly.com/link/158982/web) – 用于管理 Postgres 的 RESTful API。

[pgrx 0.12](https://postgresweekly.com/link/158983/web) – 一种使用 Rust 构建 Postgres 扩展的方法。

[pgModeler 1.1.4](https://postgresweekly.com/link/158984/web) – 可视化数据建模工具。

[pgAdmin 4 v8.11](https://postgresweekly.com/link/158985/web)