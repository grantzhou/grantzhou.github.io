---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-9-11
---
### PostgreSQL每周新闻#615 - 2025年9月11日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/615)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/ppthfcm8ahmx87sfbnys.jpg)
## [pg_duckdb 1.0：基于 DuckDB 的 Postgres 高性能分析扩展](https://postgresweekly.com/link/174135/web)
一款官方 Postgres 扩展（与 Hydra 和 MotherDuck 合作开发），将 DuckDB 的列式矢量化分析引擎及其功能嵌入到 Postgres 中。GitHub 仓库。

`DuckDB`

## [亲身体验 Postgres 18：异步 I/O、B 树跳过扫描等](https://postgresweekly.com/link/174103/web)
Postgres 18 将于本月发布，现在是时候了解其以性能为中心的更新了：从异步 I/O 和计划器更改，到 B 树跳过扫描、UUIDv7、VACUUM 更改以及对生产工作负载的增强监控。

`pganalyze `

## [Postgres 18 RC1 版本发布](https://postgresweekly.com/link/174104/web)
就在我们上周即将点击“发送”按钮时，官方发布了一篇关于 RC1 的博客文章，我们悄悄地把它分享了出来。不过，这篇文章只是简短地提及了一下，所以值得再次分享，以防您错过。我们还了解到，最终版本将于两周后的 9 月 25 日发布。

`PostgreSQL Global Development Group `

💡 Umair Shahid 分享了他最期待的 Postgres 18 的三个功能。


## [Supabase 向 Postgres 社区开放 OrioleDB 专利](https://postgresweekly.com/link/174104/web)
OrioleDB 于三年前作为 Postgres 的新存储引擎问世。Supabase 于 2024 年收购了它，现在允许其他人使用该专利中描述的技术。Paul 指出：“我们的目标就是将 Oriole 推向上游，使其成为 Postgres 源代码树的一部分，并与 Postgres 的其他部分一起公开开发和维护（如果社区愿意的话！）”

`Paul Copplestone (Supabase)`


### **本周摘要**

* 🇪🇸 [Postgres Ibiza 2025](https://postgresweekly.com/link/174110/web) 将于今年 10 月 15 日至 17 日在美丽的伊维萨岛举行。感觉如何？Jesús Espino [撰写了他参加去年活动的经历](https://postgresweekly.com/link/174111/web)。

* Neon 无服务器 Postgres 平台宣布，它[不再将高级功能（例如 HIPAA 和 SOC 2 合规性）锁定在更高企业级用户](https://postgresweekly.com/link/174112/web)之后，而是让所有用户都能以“按需付费”的方式使用这些功能。

* Postgres 项目再次参加了 [Google Summer of Code](https://postgresweekly.com/link/174113/web)，一位名叫 Ahmed Gouda 的学生[参与者分享了他专注于 pgwatch 的工作成果](https://postgresweekly.com/link/174114/web)。

* 🇮🇳 [PGConf India 2026 ](https://postgresweekly.com/link/174116/web)将于明年 3 月 11 日至 13 日在班加罗尔举行，其 [CFP](https://postgresweekly.com/link/174117/web) 开放至 10 月 15 日。


## [排序规则可以用于 citext 吗？](https://postgresweekly.com/link/174118/web)
“对于不区分大小写的查询，自定义的非确定性排序规则确实可以作为 citext 的替代方案，而且通常性能损失要低得多。”


`Umut Tekin`

📄 [深入探究 Postgres 内部机制](https://postgresweekly.com/link/174119/web)：流程架构 Srinath Reddy (EDB)

📄 [Postgres 18 着眼于分析能力提升和分布式未来](https://postgresweekly.com/link/174120/web)——The Register 聚焦即将发布的 Postgres 18 版本。Lindsay Clark

📄 [惊喜维也纳之旅](https://postgresweekly.com/link/174121/web)——上周参加奥地利 PGDay 活动的记录。Christoph Berg

📄 [类似“TPC-C”的 pgbench“扩展包”](https://postgresweekly.com/link/174123/web) Kaarel Moppel

## [PostgreSQL 内部原理：简介](https://postgresweekly.com/link/173459/web)
如果您的应用程序具有无法从缓存中受益的非传统访问模式，则有用的调整技巧。


### **发布**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/r2pc9y3ozsj1dupflsum.jpg)


## [pgFormatter 5.7：一款格式化 SQL 代码的工具](https://postgresweekly.com/link/174124/web)
您可以在线测试，也可以从 GitHub 获取源代码（使用 Perl 编写）并自行运行。v5.7 中的新功能。

`Gilles Darold`

## [EpgEdge 开源](https://postgresweekly.com/link/174127/web)
pgEdge 是一个面向企业的 Postgres 发行版，专注于高可用性和支持多主服务器的分布式部署。它之前是一个“源代码可用”的商业产品，但现在已获得 OSI 认可的 PostgreSQL 许可证。

`Dave Page`

## [矢量搜索包装器：通用向量搜索包装器](https://postgresweekly.com/link/174129/web)
如果您是 Python 开发人员，它可以让您在 Postgres、MySQL、SQLite 和 DuckDB 向量后端之间快速切换。

`Mihir Ahuja`

[pREST (PostgreSQL REST) 2.0 RC3](https://postgresweekly.com/link/174130/web) – 在 Postgres 数据库前端部署 RESTful API。

[BemiDB 1.3](https://postgresweekly.com/link/174131/web) – 针对分析优化的单二进制 Postgres 只读副本。

[pgai v0.12](https://postgresweekly.com/link/174132/web) – Timescale 的工具，用于在 Postgres 中使用 RAG 和 LLM。

[pgroll 0.14.2](https://postgresweekly.com/link/174133/web) – 零停机、可逆模式迁移。

[Supavisor 2.7](https://postgresweekly.com/link/174134/web) – Supabase 的多租户连接池。