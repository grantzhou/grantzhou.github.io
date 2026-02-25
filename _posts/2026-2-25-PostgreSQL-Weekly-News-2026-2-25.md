---
layout: post
title: PostgreSQL 每周新闻 2026-2-25
---
### PostgreSQL每周新闻#637 - 2026年2月25日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/637)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/j0rsq6gvmpu39cchsm3z.jpg)

## [带连接的行锁如何产生令人惊讶的结果](https://postgresweekly.com/link/181198/rss)

非空外键和有效约束应该保证内连接总是返回一行..对吧？这篇文章介绍了一个真实的边缘情况，在这种情况下可能*什么都不返回*（由于一个容易被忽视的并发和锁定问题），解释了原因，并提供了几种解决方案。

Haki Benita


## [企业级 Postgres 用于 Agentic AI、高可用性等](https://postgresweekly.com/link/181199/rss)

pgEdge 为 Agentic AI 和需要高可用性、可靠性和数据主权的企业应用提供开源、100% Postgres 基础设施。我们让大规模构建、部署和管理企业级 Postgres 应用变得简单。

pgEdge **赞助商**


## 本周摘要：

- ⚠️ [Postgres 的"非周期发布"预计将于明天发布。](https://postgresweekly.com/link/181200/rss)它旨在解决[最近发布的 Postgres 18.2、17.8、16.12、15.16 和 14.21](https://postgresweekly.com/link/181201/rss) 中引入的回归问题。

- 🇨🇦 [PGConf.dev 的日程安排](https://postgresweekly.com/link/181202/rss)现已上线，会议将于今年 5 月 19-22 日在温哥华举行。

- 🇩🇪 [PGConf.DE 2026 的日程安排](https://postgresweekly.com/link/181203/rss)现已上线。它将于 4 月 21-22 日在德国埃森举行。


## [利用 Postgres 竞态条件](https://postgresweekly.com/link/181204/rss)

解释了同步屏障如何让您在测试中按需制造竞态条件，以及如何验证您的锁实际上在做您认为它们在做的事情。

Mikael Lirbank


## [为什么 C 排序规则是集群的最佳选择](https://postgresweekly.com/link/181205/rss)

如何通过使用简单的 C 排序规则而不是自然语言排序规则来避免 OS 升级后可能出现的索引损坏陷阱。但如果您*想要*在日常使用中使用自然语言排序规则怎么办？Laurenz 展示了如何两全其美。

Laurenz Albe


## [▶ 为什么攻克 Postgres 性能问题很有趣](https://postgresweekly.com/link/181206/rss)

Microsoft 的 Tomas Vondra 是一位长期的 Postgres 贡献者，以性能工作而闻名。在这个 80 分钟的采访中，他解释了为什么性能攻克很难但很有趣，演示了他贡献的哈希连接优化，并分享了为什么 Postgres 的"社区氛围"让他不断回归。

Talking Postgres Podcast **podcast**


📄 [我希望早点知道的 9 个 Postgres 特性](https://postgresweekly.com/link/181207/rss) – 包括 `EXCLUDE` 和 `CHECK` 约束、`DISTINCT ON`、`FILTER` 和递归 CTE。*Thiery Michel*

📄 [`INSERT 0 1` 实际上告诉您什么？](https://postgresweekly.com/link/181208/rss) – 简短而优雅地看一下您以前见过但可能从未想过的东西。*Lætitia Avrot*

📄 [Postgres 19 即将推出：`%i` 提示转义以指示热备份状态](https://postgresweekly.com/link/181209/rss) – 在您的 `psql` 提示中使用 `%i` 将让您一目了然地看到您是连接到主服务器还是备用服务器。*Hubert Lubaczewski*

📄 [使大型 Postgres 迁移切实可行：使用 PeerDB 在两小时内迁移 1TB](https://postgresweekly.com/link/181210/rss) *Amogh Bharadwaj (ClickHouse)*


## 🛠 代码和工具

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/vvy3kjykzsd7atoie8og.jpg)

## [sabiql: 用于 Postgres 的无驱动 TUI](https://postgresweekly.com/link/181211/rss)

一个基于 Rust 的 Postgres 终端 UI，它包装了 `psql`，所以不涉及驱动程序。然而，与 `psql` 不同，您可以获得 ER 图生成、内联单元格编辑、将值快速复制到剪贴板、模糊搜索等功能。

riii111


## [pg_ash: Postgres 的活动会话历史](https://postgresweekly.com/link/181212/rss)

一种纯 SQL 和 PL/pgSQL 方法（因此它甚至可以在托管平台上工作）。它每秒对 `pg_stat_activity` 进行采样，并以紧凑格式存储结果，您稍后可以使用 SQL 查询这些结果，以深入了解您没有实时捕获的问题。

Nikolay Samokhvalov