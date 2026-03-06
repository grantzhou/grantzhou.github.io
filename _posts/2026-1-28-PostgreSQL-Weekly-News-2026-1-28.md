---
layout: post
title: PostgreSQL 每周新闻 2026-1-28
---
### PostgreSQL每周新闻#633 - 2026年1月28日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/633)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/bdupmx0qonlmqfbgsmwl.jpg)

## [OpenAI 如何扩展 Postgres 以支持 8 亿 ChatGPT 用户](https://postgresweekly.com/link/179887/rss)

你知道 Postgres 是 ChatGPT 的核心吗？OpenAI 分享了他们如何通过读副本让 Postgres 支持每秒数百万次查询，**仅使用单个主节点**（无需分片！）的故事。这篇文章基于 [Bohan 去年在 PGConf․dev 上的一场流行演讲](https://postgresweekly.com/link/179888/rss)。

**Bohan Zhang (OpenAI)**


💡 如果 Bohan 的名字看起来很熟悉，他是 [OtterTune](https://postgresweekly.com/link/179889/rss) 的联合创始人之一（与 Andy Pavlo 和 Dana Van Aken 一起）。OtterTune 是一个 AI 驱动的数据库调优系统，所以他在 OpenAI 表现出色也就不足为奇了！😁


## [面向时序数据规模的 Postgres 扩展](https://postgresweekly.com/link/179886/rss)

TimescaleDB 通过超表扩展了 Postgres，实现了自动分区、95% 压缩率以及实时刷新的连续聚合。无需管理新数据库，无需学习新查询语言。它就是 Postgres，但更快。[免费开始构建](https://postgresweekly.com/link/179886/rss)。

**Tiger Data** 赞助商


## [🔎 当用户输入 'beatles abbey rd' 时找到 'Abbey Road'](https://postgresweekly.com/link/179890/rss)

介绍如何使用 `pg_trgm` 进行模糊搜索以及使用 `pgvector` 进行语义搜索，以超过 100,000 首歌曲的数据集为例。

**Daniel Guzman Burgos**


**简讯：**

- ClickHouse 已进入 Postgres 托管领域，推出了[与 ClickHouse 原生集成的新托管 Postgres 服务](https://postgresweekly.com/link/179891/rss)。

- 🇫🇮 将于 3 月 24 日在赫尔辛基举行的 [Nordic PGDay 2026](https://postgresweekly.com/link/179893/rss) 的[日程](https://postgresweekly.com/link/179892/rss)现已公布... 🇫🇷 两天后（3 月 26 日）在巴黎举行的 [pgDay Paris 的日程](https://postgresweekly.com/link/179894/rss)也已公布。

- Damien Clochard 探讨了[哪些 Postgres 平台支持 PostgreSQL Anonymizer](https://postgresweekly.com/link/179895/rss)。

- 云平台 [*Neon* 进行了品牌重塑，推出了新设计](https://postgresweekly.com/link/179896/rss)，并从 `.tech` 迁移到 `.com`。


## [Postgres 中的 Buffers 简介](https://postgresweekly.com/link/179897/rss)

Buffers 是 Postgres 内部运作的基础部分，但在教程中经常被忽视，除了为性能调整几个配置设置。Radim 解释了它们实际在做什么。

**Radim Marek**


## [为什么你的高可用架构是个谎言（但这没关系）](https://postgresweekly.com/link/179898/rss)

*"停止追求完美。为现实建模你的架构"*，Lætitia 在对高可用性常见误解的简短探讨中说道。

**Lætitia Avrot**


## [`WITHOUT OVERLAPS` 约束，现已在 Postgres 18 中可用](https://postgresweekly.com/link/179899/rss)

时态功能在 SQL:2011 中出现，在 SQL:2023 中被标准化为可选功能。`WITHOUT OVERLAPS` 在 Db2 和 MariaDB 中早已可用，现已登陆 Postgres 18，允许拒绝具有重叠时间范围的插入。

**Neon**


## [Postgres 索引简介](https://postgresweekly.com/link/179900/rss)

面向在高层次上熟悉索引但想要更好地了解底层运作的开发者的基础概述。

**Dalto Curvelano**


📄 [如何渲染与当前时区不同的时间戳](https://postgresweekly.com/link/179901/rss) – Hubert 已经完成了所有实验，所以你不必这样做。*Hubert depesz Lubaczewski*

📄 [MySQL 的未来是 PostgreSQL（或 MariaDB，或 TiDB，或...）吗？](https://postgresweekly.com/link/179902/rss) – 以充满希望的开场白开始：*"我无意用这篇博文惹恼任何人"*。*Dave Stokes*

📄 [将 Postgres 用作事件驱动系统的死信队列](https://postgresweekly.com/link/179903/rss)  *Diljit PR*

📄 [将 Sybase/SAP ASE 迁移到 Postgres](https://postgresweekly.com/link/179904/rss)  *Avinash Vallarapu (HexaCluster)*


## 📰 分类广告

📌 获取功能齐全、由 Postgres 专家支持并与标准 Postgres 兼容的 MCP 服务器：[github.com/pgEdge/pgedge-postgres-mcp](https://postgresweekly.com/link/179905/rss)。

🐘 **CFP** 将于 **2 月 1 日**截止，面向 [POSETTE: An Event for Postgres](https://postgresweekly.com/link/179906/rss)。在我们的网站上找到所需的所有资源。不要拖延 - [立即开始](https://postgresweekly.com/link/179906/rss)。


## 🛠 代码和工具

## [🤖 为编码代理提供的 Postgres 最佳实践](https://postgresweekly.com/link/179907/rss)

一系列可以轻松安装的 Postgres 最佳实践，为 Claude Code 或 Codex 等编码代理提供额外优势，考虑了 RLS、连接管理和 Postgres 特定的 SQL 功能等 Postgres 细节。即使你*不*使用 AI，你也可以[在这里以 Markdown 形式阅读所有指南](https://postgresweekly.com/link/179908/rss)。

**Pedro Rodrigues (Supabase)**


💡 类似地，[Neon 发布了一套代理技能](https://postgresweekly.com/link/179909/rss)，专门用于与 Neon Serverless Postgres 配合使用。


## [RegreSQL 1.5：SQL 查询的回归测试](https://postgresweekly.com/link/179910/rss)

这个想法很简单：获取你的查询，运行它们，捕获预期结果，然后在未来运行时比较它们的成本、I/O 或其他特征何时发生变化。*"当查询结果意外变化时，你会立即知道。"* [GitHub 仓库。](https://postgresweekly.com/link/179911/rss)

**boringSQL**


## [✉️ pg_utl_smtp 1.0：适用于 Postgres 的 Oracle UTL_SMTP 兼容扩展](https://postgresweekly.com/link/179912/rss)

[UTL_SMTP](https://postgresweekly.com/link/179913/rss) 是一个 Oracle Database 包，用于直接从数据库过程通过 SMTP 发送电子邮件。这个扩展将相同的 API 带到了 Postgres。

**HexaCluster**


- [Pigsty 4.0](https://postgresweekly.com/link/179914/rss) – "自带电池"的 Postgres 发行版，加强了安全性，添加了 Docker 支持，并从 AGPL-3.0 切换到 Apache-2.0。

- [DbGate v7.0](https://postgresweekly.com/link/179915/rss) – 支持多种数据库的跨平台数据库工具。编写查询、处理模式、可视化数据等。

- [DBOS Transact 2.10.0](https://postgresweekly.com/link/179916/rss) – 在 Python 中的持久化执行，由 Postgres 支持。

- [pg-boss 12.7.0](https://postgresweekly.com/link/179917/rss) – 基于 Postgres 构建的 Node.js 作业队列。

- [PGXN Tools v1.7](https://postgresweekly.com/link/179918/rss)