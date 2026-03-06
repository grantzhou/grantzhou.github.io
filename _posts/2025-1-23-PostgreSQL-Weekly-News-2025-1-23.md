---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-1-23
---
### PostgreSQL每周新闻#583 - 2025年1月23日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/585)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/mk5bzh3up1xchq0gse6b.jpg)
## [2024 年谁为 Postgres 发展做出了贡献？](https://postgresweekly.com/link/164673/web)
每年，罗伯特都会编制一份名单，列出过去一年对 Postgres 发展贡献最大的人。229 人是至少一次提交的主要作者，66% 的新代码行来自前 18 位贡献者。

`Robert Haas`

## [表级锁的剖析：减少锁定影响](https://postgresweekly.com/link/164674/web)
执行操作时很容易锁定整个表，但性能和正常运行时间的影响应该很快促使您使用限制较少的方法。Gulcin 解释了一些选项。


`Gulcin Yildirim Jelinek `
## [VeilStream – 适用于 Postgres 的简单数据访问管理](https://postgresweekly.com/link/164672/web)
VeilStream 是一种安全、自托管的 Postgres 过滤器，位于生产数据库的前面，提供强大而简单的 GUI 和 API 来设置数据编辑和匿名化规则。立即免费试用。


`VeilStream `
## [GROUP BY 和修复优化器估计](https://postgresweekly.com/link/164675/web)
您是否知道 GROUP BY 包含的列越多，优化器高估行数的可能性就越大？Postgres 为每列维护单独的统计数据，并通过将它们相乘来创建组估计。创建扩展统计数据可以帮助整理事情。


`Hans-Jürgen Schönig `

### 本周摘要：

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/up6tlxtjaevrp6q1hrqn.jpg)

* 在通过 TLS 对 Neon 进行真正的 Postgres 查询时，请查看网络上[传输的每个字节](https://postgresweekly.com/link/164676/web)（见上文）。所有内容都带有注释，以帮助您了解复杂性。

* [Clickbench](https://postgresweekly.com/link/164677/web) 是实时分析数据库的基准，多亏了 [pg_mooncake](https://postgresweekly.com/link/164678/web)，Postgres 现在已成为基准测试中排名前 10 的数据库。

* 🗓️ 2025 年[北欧 PGDay](https://postgresweekly.com/link/164680/web) 和 2025 年[巴黎 pgDay](https://postgresweekly.com/link/164681/web) 的时间表现已发布。

* 🇧🇪 如果您下个月要参加或想要参加 FOSDEM PGDay，Andreas Scherbaum 在这里有[很多有用的建议和信息](https://postgresweekly.com/link/164682/web)。


## [在 Postgres 中实现线程安全的扫描器和解析器](https://postgresweekly.com/link/164683/web)
除非您是 Postgres 实现者（例如此处的前 5 名贡献者 Peter Eisentraut），否则这可能不会直接对您有用，但了解将 Postgres 的扫描器和解析器转变为线程安全所涉及的内容很有趣。剧透：内容很多。


`Peter Eisentraut `
## [不要忘记Parallel Leader Participation设置](https://postgresweekly.com/link/164685/web)
Kaarel 有他自己的 TLDR：“如果您正在处理更大的缓存外数据集，拥有大量核心，尤其是当表被分区时，您实际上应该考虑禁用 parallel_leader_participation。”


`Kaarel Moppel `

📄 [使用 JSONB 取消透视数据](https://postgresweekly.com/link/164686/web) – 非常实用的技巧 - Leo Hsu 和 Regina Obe

📄 [谁的优化更好？](https://postgresweekly.com/link/164687/web) – 关于比较 SQL 查询计划质量的想法 - Andrei Lepikhov

📄 [Postgres UUIDv7](https://postgresweekly.com/link/164688/web) + 每个后端单调性 - Brandur Leach

📄 [Postgres 中的逻辑复制：基础知识](https://postgresweekly.com/link/164689/web) - Phil Eaton

### 📰 分类广告
🐘 [POSETTE：Postgres](https://postgresweekly.com/link/164690/web) 活动将于 6 月 10 日至 12 日举行。征集提案将于 2 月 9 日结束。鼓励新手和经验丰富的演讲者提交提案！

实现 Postgres 的最佳性能。[参加 pganalyze 之旅](https://postgresweekly.com/link/164691/web)。

### 代码和工具：

## [DBOS Transact v2：TypeScript 中的轻量级持久执行](https://postgresweekly.com/link/164692/web)
基于 Postgres 构建的轻量级持久执行开源库。持久执行意味着在程序运行时保持其执行状态，因此如果程序中断或崩溃，它会从中断处恢复，非常适合长期运行或业务关键型工作流程。文档。

`DBOS, Inc.`

## [HeidiSQL 12.10](https://postgresweekly.com/link/164694/web)
一款用于数据库工作的原生 Windows 应用程序 — 一款方便的开源数据库管理工具。支持 Postgres、MySQL、SQL Server 和 SQLite。使用 Delphi 编写，开源。

`Ansgar Becker`

[PostgresML 2.10](https://postgresweekly.com/link/164696/web) – 从 SQL 进行机器学习。现在支持 Postgres 17。

[pgai 0.7](https://postgresweekly.com/link/164697/web) – Timescale 的工具，用于在 Postgres 中与 RAG 和 LLM 配合使用。

[pg-diff 3.0](https://postgresweekly.com/link/164698/web) – PostgreSQL 模式和数据比较工具。

[tbls 1.80](https://postgresweekly.com/link/164699/web) – 自动以 Markdown 格式记录数据库。

[Bob 0.30](https://postgresweekly.com/link/164700/web) – Go 的 SQL 查询生成器和 ORM/Factory 生成器。

[PostgreSQL JDBC 驱动程序 42.7.5](https://postgresweekly.com/link/164701/web)

[PostGIS 3.5.2](https://postgresweekly.com/link/164702/web)