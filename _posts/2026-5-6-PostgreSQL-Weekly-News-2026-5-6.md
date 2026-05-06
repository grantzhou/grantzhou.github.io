---
layout: post
title: PostgreSQL 每周新闻 2026-5-6
---
### PostgreSQL每周新闻#647 - 2026年5月6日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/647)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/kypnkxj6cc4bjtcfewgt.jpg)

## [我对 Postgres 19 感兴趣的特性](https://postgresweekly.com/link/184808/rss)

对 v19 部分亮点的主观评述，包括 `pg_plan_advice`、DDL 提取函数、在线 `REPACK`/`REPACK CONCURRENTLY` 以及可观测性改进。

**Tianzhou (Bytebase)**


## [将 Postgres 用作作业队列的潜在后果](https://postgresweekly.com/link/184809/rss)

在"小规模"下没问题，但何时会出现问题，有哪些替代方案？Richard 提供了一些实用的建议。

**Richard Yen**


## [POSETTE 上的 Azure HorizonDB：2026 年 Postgres 活动](https://postgresweekly.com/link/184807/rss)

在 POSETTE 2026（一个免费的虚拟开发者活动，将于 6 月 16-18 日举行）上探索 44 场关于 Azure HorizonDB、基于 PostgreSQL 的应用开发、Postgres 性能与 AI、Postgres 19 等主题的演讲。不要错过您喜欢的内容 - 使用[添加到日历](https://postgresweekly.com/link/184807/rss)功能。

**Microsoft | AMD sponsor**


## PGBACKREST 插曲：

- 上周，[pgBackRest "死了"](https://postgresweekly.com/link/184810/rss)，但在 Postgres 世界一周是很长的时间，维护者 David Steele 收到了大量支持，以至于*["几乎可以确定[他]将能够获得足够的资金来继续该项目。"](https://postgresweekly.com/link/184811/rss)* 🎉

- 即使 Steele 的资金落空，[PGX Inc.](https://postgresweekly.com/link/184832/rss) 也已介入[提供 `pgxbackup` 的"连续性支持"](https://postgresweekly.com/link/184812/rss)，这是 pgBackRest 的一个分支。

- Vibhor Kumar 利用 pgBackRest 的故事[反思开源的角色](https://postgresweekly.com/link/184813/rss)，当它超越仅仅是一个项目而成为*基础设施*时。


## [Figma 如何为 Postgres 构建所需的连接池管理器](https://postgresweekly.com/link/184814/rss)

Figma 的规模超出了 PgBouncer 的能力，评估了 PGCat，最终使用 Go 和 [PGX](https://postgresweekly.com/link/184815/rss) 构建了自己的连接池管理器（PGKeeper）。它不是公开的，但他们深入探讨了设计：它向客户端公开 gRPC 而不是充当 PG 线协议池管理器，因此每个查询都有元数据用于基于优先级的准入控制、负载削减和公平共享。

**He, Goh, and Baid (Figma)**


## [212 项内容](https://postgresweekly.com/link/184816/rss)

[Postgres 19 草稿发布说明](https://postgresweekly.com/link/184817/rss)中的 212 个条目可能令人不知所措，Christophe 将其归纳为*"关键"*项目，同时解释说虽然 v19 没有单一的*"标志性用户功能"*，但它*"正是一个良好的数据库版本应该有的样子。"*

**Christophe Pettus**


## [Postgres 提交者是如何选择的？](https://postgresweekly.com/link/184818/rss)

一位 Postgres 提交者解释了人们如何被选入[这个杰出的群体](https://postgresweekly.com/link/184819/rss)。

**Tomas Vondra**


## [这取决于：在 Postgres 中使用会话变量](https://postgresweekly.com/link/184820/rss)

您可能使用过 [`SET`](https://postgresweekly.com/link/184821/rss) 来调整配置参数，但您知道可以用它来存储自己的会话变量吗？

**Shaun Thomas**


📄 [使用 Postgres 构建 MCP 服务器](https://postgresweekly.com/link/184822/rss) – Bruce 的另一个优秀演示幻灯片。*Bruce Momjian*

📄 [为什么要向雇主推销为 Postgres 做贡献的想法](https://postgresweekly.com/link/184823/rss) *Valeria Kaplan*


## 分类广告：

🔎 [为 Postgres 提供 Elastic 级别的搜索扩展](https://postgresweekly.com/link/184839/rss)。BM25、分析和向量 — 无需 Elasticsearch。

🐘 [AppSignal](https://postgresweekly.com/link/184824/rss) 精确定位慢速 Postgres 查询、破坏它的部署以及修复方法。[免费 30 天试用。2 分钟安装](https://postgresweekly.com/link/184824/rss)。

🤖 [认识 Ellie](https://postgresweekly.com/link/184825/rss) — 您的 24x7 Postgres AI 助手。监控、检测并修复任何 Postgres 数据库上的问题。[免费且开源](https://postgresweekly.com/link/184825/rss)。


## 🛠 代码和工具

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/stbujlcgrkxmtd8gjbt5.jpg)

## [pg_column_tetris：强制执行最佳列对齐以最小化行填充浪费](https://postgresweekly.com/link/184826/rss)

Postgres 为了效率将列对齐到特定的字节边界，插入"填充"来填补空隙。此扩展可以显示现有表中有多少字节浪费在填充上，或者可以警告/阻止创建列顺序低效的表。

**Roger Welin**

💡 如果您正在寻找最佳实践，[在 PostgreSQL 中排序表列](https://postgresweekly.com/link/184827/rss)提供了 GitLab 如何设计表以避免浪费填充的指南。

- [pg_graphql 1.6](https://postgresweekly.com/link/184830/rss) – 为 Postgres 数据库添加 GraphQL 支持。值得注意的是，GraphQL 内省[现在默认禁用](https://postgresweekly.com/link/184831/rss)以减少 API 枚举的可能性。

- [PostgREST 14.11](https://postgresweekly.com/link/184828/rss) – 从 Postgres 数据库提供完全 RESTful 的 API。

- [postgresparser 1.2](https://postgresweekly.com/link/184829/rss) – 基于 ANTLR 的 PostgreSQL 查询解析器，用于 Go。