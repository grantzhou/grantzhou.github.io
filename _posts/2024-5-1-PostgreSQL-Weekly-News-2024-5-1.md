---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-5-1
---
### PostgreSQL每周新闻#553 - 2024年5月1日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/553)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/s3diq7eox8hkpfsn0jgj.jpg)
## [Crunchy Bridge分析：Your Data Lake in Postgres? ](https://postgresweekly.com/link/154439/web)
Marco Ponders：“如果您可以使用 PostgreSQL 轻松查询具有最先进分析性能的 Data Lake，会怎么样？”Crunchy Bridge用于分析是Crunchy Data的Postgres平台提供S3集成，CSV/Parquet查询支持以及双向数据湖↔Postgres进口/导出的新部分。


`Marco Slot (Crunchy Data) `
## [150 倍 pgvector 加速：年度回顾](https://postgresweekly.com/link/154501/web)
pgvector为 Postgres 提供了额外的数据类型、索引和查询功能，以处理高维向量（例如 LLM 和嵌入中常见的向量）。过去一年，其功能和性能有了巨大的飞跃。


`Jonathan Katz `
## [使用 OtterTune 提高 Postgres 性能并降低成本](https://postgresweekly.com/link/154438/web)
 在 AWS 上花费更多并不等于获得更好的性能。OtterTune 通过优化旋钮获得比标准 RDS 设置高 146% 的吞吐量，并提供索引和查询建议以及表和自动清理见解。免费试用 30 天。


`OtterTune `
## [Postgres膨胀最小化](https://postgresweekly.com/link/154441/web)
表占用的空间比预期的多是引起抱怨的常见原因，但您可以采用多种策略来更有效地利用空间。


`Pavel Borisov `
**本周摘要：**
*   Peter Eisentraut 回顾了Postgres 一直以来支持的平台。


*   Timescale 的首席执行官认为 Postgres 是“数据未来的基石”，并利用社区情绪和调查数据来证明这一点。


*   📅如果您想了解 David Wheeler 对 Postgres 扩展打包和分发生态系统提出的改进的最新进展，几个小时后将举行一次虚拟“迷你峰会” （5 月 15 日还将举行另一场）。


*   看起来PG Day芝加哥2024进展顺利！


## [Papa 有了一个全新的 RAG](https://postgresweekly.com/link/154445/web)
RAG（检索增强生成）是一种与大型语言模型一起使用的技术，您可以在其中获取数据以包含在提示中以改进 LLM 给出的响应。Shaun 演示了如何将所有部分组合在一起，以在 Python 中构建一个简单的基于 RAG 的查询系统，其中pg_vectorize在 Postgres 端完成繁重的工作。


`Shaun M. Thomas `
## [📄 通过 GitHub Actions 进行夜间 Postgres 备份 ](https://postgresweekly.com/link/154447/web)
JOSH STRANGE


## [📄 何时以及为何忽略 Postgres 索引 ](https://postgresweekly.com/link/154448/web)
CLUSTERITY SRO

## [📄 基准测试连接池：PgBouncer、PgCat 和 Supavisor ](https://postgresweekly.com/link/154449/web)
BINIDXABA (TEMBO)

## [📄 使用 pgxn-tools 测试和发布 pgrx 扩展 ](https://postgresweekly.com/link/154450/web)
DAVID WHEELER

## [📄 通过 PAM 在 PgBouncer 中进行 LDAP 身份验证 ](https://postgresweekly.com/link/154451/web)
JOBIN AUGUSTINE


## [PeerDB：一种在其他地方复制 Postgres 数据的简单、快速方法](https://postgresweekly.com/link/154452/web)
由前 Microsoft 和 Citus Data 员工构建的数据复制系统，针对需要将数据从 Postgres 流式传输到数据仓库、队列和其他存储引擎的用例。本周的v0.13.0 版本引入了 Elasticsearch 连接器。GitHub存储库。


`PeerDB `
## [pg_tier：将数据分层到外部 Amazon S3 存储](https://postgresweekly.com/link/154456/web)
一旦数据变旧或访问频率降低，将其存储在其他地方可能会更具成本效益。pg_tier 可以更轻松地将表推送到 S3，同时仍保持查询它的能力（当然，会增加一些延迟）。


`Tembo `
## [Squawk：用于 Postgres 迁移的 Linter](https://postgresweekly.com/link/154457/web)
防止数据库迁移导致的意外停机并鼓励围绕模式和 SQL 的最佳实践。


`Steve Dignam `
## [Hypopg 1.4.1](https://postgresweekly.com/link/154458/web)
 - Postgres 的假设索引。现在支持 Postgres 17。


## [pgmoneta 0.11](https://postgresweekly.com/link/154459/web)
 - 备份/恢复解决方案。现在支持 macOS 并添加磁盘和网络速率限制功能。


## [Orafce 4.10.0](https://postgresweekly.com/link/154460/web)
 - 模拟 Oracle 数据库的函数和包子集以帮助迁移。


## [Lantern 0.2.5](https://postgresweekly.com/link/154461/web)
 - Postgres 的 HNSW/ usesearch矢量扩展。


## [pgwire 0.22 ](https://postgresweekly.com/link/154463/web)
 - Rust 库中的 Postgres 线路协议。



# 💡本周提示


**🗓即将举办的Postgres活动**
