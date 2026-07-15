---
layout: post
title: PostgreSQL 每周新闻 2026-7-15
---
### PostgreSQL每周新闻#657 - 2026年7月15日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/657)

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/kaeijwub8qefrcin2rpn.jpg)

## [导致数千次 Postgres 宕机的四大祸首](https://postgresweekly.com/link/187904/rss)

两周前我们提到了 [pgrust](https://postgresweekly.com/link/187905/rss)，一个 AI 辅助的 Postgres Rust 重写版本（现在已通过 100% 的 Postgres 回归测试）。在这篇文章中，其创建者概述了他在重写过程中着手解决的 Postgres 最大痛点。

`Michael Malis`

🗣️ 与此同时，[Hacker News 发现了 `pgrust`](https://postgresweekly.com/link/187906/rss) 并进行了深入讨论，Michael 回答了关于其创建和目标的众多问题。

## [无需第二系统的搜索](https://postgresweekly.com/link/187903/rss)

一个 Postgres 满足您的应用数据、全文搜索、向量检索和聚合需求。ParadeDB 是一个开源 Postgres 扩展，性能可媲美 Elasticsearch。

`ParadeDB` **赞助商**

## [如何在按非分区列查询时实现分区修剪](https://postgresweekly.com/link/187907/rss)

如果非分区键列与分区键强相关（例如时间分区数据中的连续会话 ID），`CHECK` 约束可以实现对该列的分区修剪。包含一个处理异常值的 BRIN 启发式方法。

`Haki Benita`

**简讯：**

- 🎂 [Pigsty](https://postgresweekly.com/link/187908/rss) 创建者 Ruohang Feng [庆祝 Postgres 30 周年](https://postgresweekly.com/link/187909/rss)，以 1996 年 7 月 8 日首个公开 Postgres CVS 服务器上线为起点。

- 📘 Dimitri Fontaine 的 [*The Art of PostgreSQL* 一书](https://postgresweekly.com/link/187910/rss)已更新至 2026 年版，这是一次重大更新，*"将文本从 PostgreSQL 11 现代化到 17/18 版本"*。

- 🏴󠁧󠁢󠁳󠁣󠁴󠁿 Jimmy Angelakos 分享了[最近在苏格兰爱丁堡举行的 PostgresEDI 聚会摘要](https://postgresweekly.com/link/187911/rss)，并邀请大家[参加 8 月 13 日的下一次聚会](https://postgresweekly.com/link/187912/rss)。

- Google Cloud 团队分享了[其最近参与多个 Postgres 活动的更新](https://postgresweekly.com/link/187913/rss)。

## [SQL/PGQ 如何在 Postgres 19 中重写为连接](https://postgresweekly.com/link/187914/rss)

深入了解 Postgres 19 对[图查询](https://postgresweekly.com/link/187915/rss)的支持，以及图查询语法如何编译为普通连接。

`Hans-Jürgen Schönig`

## [▶ 与 Jimmy Angelakos 一起修复 Postgres 中的糟糕 SQL](https://postgresweekly.com/link/187916/rss)

一场 55 分钟的演讲，简明扼要地解释了常见的 SQL 反模式，并配有实时 `psql` 演示。

`Jimmy Angelakos`

📄 [版本号并非领域本身](https://postgresweekly.com/link/187917/rss) – 一个服务器声称是 Postgres 14 却输出了 Postgres 14 根本没有的错误的故事。`Christophe Pettus`

📄 [等待 Postgres 20：`min()` 和 `max()` 聚合支持 `uuid`](https://postgresweekly.com/link/187918/rss) `Hubert depesz Lubaczewski`

📄 [`JOIN` 后的 `COUNT(*)` 统计的是行数，而不是事物数](https://postgresweekly.com/link/187919/rss) `Dimitri Fontaine`

📄 [我们如何在 ClickHouse 托管 Postgres 中扩展 PgBouncer](https://postgresweekly.com/link/187920/rss) `Kaushik Iska (ClickHouse)`

---

## 分类广告：

您已经在运行 Postgres。[TimescaleDB 为时间序列扩展了它](https://postgresweekly.com/link/187921/rss)：超表、原生列式压缩、更快的查询。

🔁 [Spock](https://postgresweekly.com/link/187922/rss)：开源多主 Postgres 复制，支持主主写入、冲突解决、逻辑槽故障转移。

🐘 [PostgreSQL 19 预览](https://postgresweekly.com/link/187923/rss)：PGQ 图工作负载、REPACK CONCURRENTLY、pg_plan_advice 等。EDB 黑客讲述今秋即将推出的功能。

---

## 🛠 代码和工具

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/fcelvvlazbal99bf5wap.jpg)

## [plx：用 PHP、JavaScript、Python 等编写存储函数](https://postgresweekly.com/link/187924/rss)

紧随上周的 [PL/Ruby](https://postgresweekly.com/link/187925/rss)，这是一个更通用的扩展，可将 JavaScript、PHP、Python、Ruby 甚至 *COBOL* 转译为 PL/pgSQL！

`Command Prompt Inc.`

## [pg_re2：Postgres 中快速、基于 RE2 的正则表达式](https://postgresweekly.com/link/187926/rss)

Google 的 [re2](https://postgresweekly.com/link/187927/rss) 在正则表达式执行时间上比传统的回溯方法更可预测。ClickHouse 在这里展示了它在 Postgres 中的使用。

`David Wheeler and Philip Dubé`

## [`@neon/sdk`：Neon 的新 TypeScript 客户端库](https://postgresweekly.com/link/187928/rss)

为想要使用 Postgres 平台特定功能来管理项目、分支和数据库的 [Neon](https://postgresweekly.com/link/187929/rss) 用户提供。

`Andre Landgraf (Neon)`

## [pgsavvy：用于数据库的 Vim 风格 TUI](https://postgresweekly.com/link/187930/rss)

一个基于 Go 的 TUI 应用程序，用于从终端浏览和查询 Postgres 数据库，具有 Vim 风格的导航、SQL 自动完成和交互式 `EXPLAIN` 计划导航。

`Dave Savic`

- [Pigsty 4.4](https://postgresweekly.com/link/187931/rss) – 一个"应有尽有"的 Postgres 发行版，现在基于 Postgres 18.4，并提供可试用的 Postgres 19 beta 模板。现在包含 531 个扩展可供使用。

- [plpgsql_check 2.10](https://postgresweekly.com/link/187932/rss) – PL/pgSQL 代码检查器，使用 Postgres 自己的解析器/评估器来检测错误并提高代码质量。

- [pgCodeKeeper 15.0](https://postgresweekly.com/link/187933/rss) – 基于 Java 的 Eclipse IDE 插件，用于比较数据库模式并生成迁移脚本。

- [PostgREST 14.15](https://postgresweekly.com/link/187934/rss) – 从任何 Postgres 数据库提供完全 RESTful 的 API。