---
layout: post
title: PostgreSQL 每周新闻 2026-5-27
---
### PostgreSQL每周新闻#650 - 2026年5月27日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/650)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/f47ypjpnxyepnyzpd6sy.jpg)

## [PGConf.dev 2026：为什么它仍然是我最喜欢的 Postgres 会议](https://postgresweekly.com/link/185714/rss)

上周在温哥华举行的 [PGConf.dev](https://postgresweekly.com/link/185715/rss) 活动的精彩旅行报告。Cary 除了分享许多有趣的照片，还详细总结了他参加的演讲、非正式会议上提出的话题，甚至 Postgres 30 周年生日派对上发生的事情，还有蛋糕！

💡 [Jeremy Schneider](https://postgresweekly.com/link/185716/rss) 和 [Ashutosh Bapat](https://postgresweekly.com/link/185717/rss) 也有详细的旅行报告。*"我很高兴我决定参加，"* Jeremy 说。

`Cary Huang (High Go)`


## [赞助商：您的 Agent 需要更好的上下文，而不是更大的提示](https://postgresweekly.com/link/185713/rss)

Memory Engine 将工程事实、决策和指令存储在 PostgreSQL 中，以便 Agent 在每个任务前提取相关内容。不再需要加载整个代码库。语义、关键字、时间搜索。可检查，MCP 原生。[免费开始使用](https://postgresweekly.com/link/185713/rss)。

`Memory Engine` **赞助商**


## [🕒 now() 有多快？](https://postgresweekly.com/link/185718/rss)

你知道 `now()` *不是*'当前时间'而是事务开始时的时间吗？当这种区别很重要时，就像 Oskar 遇到的重试循环一直看到相同的冻结时间戳而永远无法取得进展时，改用 `clock_timestamp()` 吧。

💡 `now()` 相当于 `transaction_timestamp()`。更多信息请参见[文档](https://postgresweekly.com/link/185719/rss)。

`Oskar Dudycz`


## [5 个让人困惑的 Postgres 锁行为](https://postgresweekly.com/link/185720/rss)

Postgres 的锁管理器在设计上是正确的，但这种正确性仍然可能让你感到惊讶。一位 Postgres 工程师介绍了五种反直觉的锁行为，这些行为曾导致实际的生产中断，以及如何避免它们。

`Shinya Kato`


## [XID Wraparound 的同样邪恶的孪生兄弟](https://postgresweekly.com/link/185721/rss)

监控事务 ID 回绕是 Postgres 管理员的家常便饭，但*MultiXact IDs*（由并发行锁和外键检查消耗）可能完全被忽视。Richard 解释了 MXID 如何累积、为什么它们也需要冻结，并分享了监控它们的查询。

💡 要深入了解 MultiXact 内部机制和调优，AWS 有[深度指南](https://postgresweekly.com/link/185722/rss)。

`Richard Yen`


## 📄 文章和故事

[TOAST：Postgres 隐藏大值的地方](https://postgresweekly.com/link/185723/rss) – 更多 Postgres 基础知识。但更脆。*Radim Marek*

[我如何在没有混乱的情况下管理持久多人游戏状态](https://postgresweekly.com/link/185724/rss) – 使用*"PostgreSQL 保存真相，Redis 做快速工作"*保持多人游戏的一致性。*Julien Singler*

[如何为基于 pgrx 的 Postgres 扩展进行性能分析](https://postgresweekly.com/link/185725/rss) – [pgrx](https://postgresweekly.com/link/185726/rss) 是一个用 Rust 构建 Postgres 扩展的框架。*Raynor Elgie*


## 分类广告：

🐘 没有足够的时间观看 44 场 Postgres 演讲？使用[《POSETTE 终极指南：Postgres 活动》](https://postgresweekly.com/link/185728/rss)并挑选你的最爱。*Microsoft | AMD。*

🚀 [现场加入我们](https://postgresweekly.com/link/185729/rss)：pgEdge AI DBA Workbench 与 Postgres 核心团队成员 Dave Page 的演示。[立即注册](https://postgresweekly.com/link/185729/rss)。

🔎 [介绍 pg_search](https://postgresweekly.com/link/185730/rss)，一个在 Postgres 中实现 Elasticsearch 质量全文、向量和混合搜索的 Postgres 扩展。


## 🛠 代码和工具

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/nulzao0zyadpzdb8afpe.jpg)

## [pgGraph：为普通 Postgres 表添加图数据库功能](https://postgresweekly.com/link/185731/rss)

一个'早期 alpha'扩展，为普通关系表添加图查询层，无需单独的数据库或新查询语言（无需学习 Cypher）。虽然还处于早期阶段，但有一些有趣的想法。[GitHub 仓库](https://postgresweekly.com/link/185732/rss)。

`Evokoa`


## [🔎 plpgsql_check 2.9：PL/pgSQL 代码检查器](https://postgresweekly.com/link/185733/rss)

一个专门的工具，用于查找隐藏在 PL/pgSQL 函数中的错误。

`Pavel Stehule`


## [pg_parse：Rust 的 Postgres 兼容 SQL 解析器](https://postgresweekly.com/link/185734/rss)

依赖于 `libpg_query`，因此你可以获得与 Postgres 本身相同的 SQL 查询内部解析树。

`Paul Mason`


**其他版本：**

- [PgQue 0.2](https://postgresweekly.com/link/185735/rss) – 零膨胀 Postgres 队列。一个 SQL 文件即可安装，使用 `pg_cron` 或 `pg_timetable` 来计时。v0.2 引入了 Python、Go 和 TypeScript 的第一方客户端、协作消费者、pg_tle 打包等。

- 📊 [pg_statviz 1.1](https://postgresweekly.com/link/185736/rss) – 用于 Postgres 内部统计时间序列分析和可视化的极简扩展和实用程序。*（我们喜欢新的 logo！）*