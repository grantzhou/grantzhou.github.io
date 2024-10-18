---
layout: post
title: PostgreSQL 每周新闻 2024-10-9
---
### PostgreSQL每周新闻#572 - 2024年10月9日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/573)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/oryz3jythgmfegnhmxay.jpg)
## [优化 Postgres 表布局以实现最高效率](https://postgresweekly.com/link/160787/web)
数据在更广泛的数据结构中的对齐长期以来一直是低级编程优化的重要因素，但它也会影响您的 Postgres 表。Renato 研究了表布局如何影响存储效率和查询性能，因为数据在磁盘上的排列和填充方式。

`Renato's Runtime Reflections`
## [“VALUE -> ANY”转换的价值？](https://postgresweekly.com/link/160788/web)
作者思考 RDBMS 是否应该在尝试制定计划之前优化查询，特别是在我们运行的手动查询比以往更少的情况下。


`Lepikhov and Rybakina `
## [在 Postgres 上构建 AI 应用程序？](https://postgresweekly.com/link/160786/web)
从 pgai 开始 — pgai 是 PostgreSQL 的扩展，它为 PostgreSQL 带来了更多 AI 工作流，例如嵌入创建和模型完成。pgai 为开发人员提供 AI 超能力，使他们更容易构建搜索和检索增强生成 (RAG) 应用程序。


`Timescale   `
## [▶ 亲身体验 Postgres 17：新功能及其对性能的影响](https://postgresweekly.com/link/160789/web)
一个小时的网络研讨会，从性能的角度介绍了 Postgres 17 的众多增强功能（还有很多！）


`Lukas Fittl (pganalyze) `

### 本周摘要：

* 您知道 Postgres 17 支持[触发登录事件吗](https://postgresweekly.com/link/160790/web)？

* [Omnigres 创始人 Yurii Rashkovskii](https://postgresweekly.com/link/160791/web) 是本周的 PostgreSQL 人物采访对象。

* 📺 [Aaron Francis 采访了 Postgres 平台 Xata.io 的 Monica Sarbu 和 Tudor Golubenco](https://postgresweekly.com/link/160792/web)，讨论了 Xata 是什么，以及运行 Postgres 平台需要做什么。

* 上周，我们提到 Postgres 18 获得了对[时间主键/唯一键的支持](https://postgresweekly.com/link/160794/web)，现在外键也得到了时间约束。

* Grant Fritchey [哀叹敏感的 ISP 端口阻止和过滤如何阻碍在路上与 RDS 的连接](https://postgresweekly.com/link/160796/web)。

* Tembo 宣布了[由 ParadeDB 的搜索和数据湖扩展提供支持的两个新堆栈](https://postgresweekly.com/link/160797/web)。


## [如何使用 Pgai 和 Pgvectorscale 构建内容推荐系统](https://postgresweekly.com/link/160798/web) 
pgvectorscale 是 pgvector 的扩展，它添加了 StreamingDiskANN 索引支持和改进的量化。


`Andreas Nigg (Timescale)`
## [▶ 使用 Llama 3、Ollama 和 Postgres 构建私有 RAG 系统](https://postgresweekly.com/link/160801/web)
依赖 OpenAI 或 Anthropic 等外部提供商可能无法满足您的数据保护政策，但幸运的是，您可以通过本地开放模型取得很大进展。


`Hervé Ishimwe (Timescale)`

📄 [Postgres 17 中的故障转移槽：通过逻辑复制确保高可用性](https://postgresweekly.com/link/160802/web) - Amit Kapila

📄 [人工智能辅助实验：分区数量与规划时间](https://postgresweekly.com/link/160803/web) - Nikolay Samokhvalov（Postgres AI）



### 📰 分类广告

✨ [宣布 MongoDB 8.0](https://postgresweekly.com/link/160804/web) - 比以前快 30% 以上。了解 MongoDB 8.0 如何构建以超越最严格的安全性、可用性和性能要求。

[Flyway Pipelines 已为 PostgreSQL 推出](https://postgresweekly.com/link/160805/web)！立即登录以免费收集有关数据库更改的健康和历史记录的见解。🚀


### 🛠 代码和工具

## [TimescaleDB 2.17.0：Postgres 的时间序列扩展](https://postgresweekly.com/link/160806/web)
这款流行的扩展实现了处理大规模时间序列数据的功能和优化，并在此版本中引入了对 Postgres 17 的完整支持。新的额外 SIMD 优化还提高了对压缩超表进行实时分析查询的性能。


`Timescale`
## [🤖 dbx：即将推出的 AI 驱动的 SQL 编辑器和数据库客户端](https://postgresweekly.com/link/160807/web)
我们很少链接到未公开的工具，但正如我们的一位读者所问的那样，他们的登陆页面当然值得一看，如果您喜欢，可以注册以获得早期访问权限。


`Jordi Hermoso`

[IvorySQL 3.4：开源 Oracle 兼容 Postgres](https://postgresweekly.com/link/160808/web)
从 Oracle 迁移到 Postgres 的方法有很多，而 IvorySQL 的方法是向 Postgres 添加兼容元素，例如对 Oracle 的 PL/SQL 语法和 Oracle XML 函数的支持。


`IvorySQL`


[rsql 0.14](https://postgresweekly.com/link/160810/web) – 基于 Rust 的现代 psql 式 CLI，可用于处理 Postgres、DuckDB、MySQL、Redshift、SQLite3、SQL Server 和其他数据库。

[Ruby PG Extras 5.4 和 Rails PG Extras](https://postgresweekly.com/link/160811/web) – 从 Ruby 和 Rails 应用程序深入了解 Postgres 实例。

[QuestDB 8.1.2](https://postgresweekly.com/link/160812/web) – Java 驱动的时间序列数据库，兼容 Postgres 有线协议。

[River 0.13](https://postgresweekly.com/link/160813/web) – 快速可靠的 Postgres 驱动的 Go 后台作业。

[Good Job 4.4](https://postgresweekly.com/link/160814/web) – Postgres 支持的 Ruby on Rails 作业队列。