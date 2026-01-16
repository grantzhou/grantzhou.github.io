---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-7-24
---
### PostgreSQL每周新闻#608 - 2025年7月24日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/609)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/dtx3obv2bt4zodzr7hzr.jpg)
## [Postgres 18 Beta 2 发布](https://postgresweekly.com/link/172192/web)
Postgres 18 的第二个 Beta 版本现已发布，最终版本将在未来几个月内发布。草稿版本说明仍然是了解最新情况的最佳途径，但本文也涵盖了自 Beta 1 版本以来的一些更改和修复。

`PostgreSQL Global Development Group`

## [将 Postgres 队列扩展到每秒 100K 个事件的经验教训](https://postgresweekly.com/link/172194/web)
RudderStack 决定使用 Postgres 作为其主要排队系统，而不是像 Kafka 这样的系统，他们的团队分享了他们学到的扩展工作的故事，包括解释一些非常具体的 Postgres 配置调整。


`Aris Tzoumas (RudderStack) `

## [Darkhorse Emergency 如何驾驭复杂的 PostgreSQL 模式](https://postgresweekly.com/link/172191/web)
了解 Darkhorse Emergency 如何用 Atlas 的声明式模式管理取代脆弱的 SQL 脚本，从而安全地演进逻辑繁重的 Postgres 系统。更快的迁移、更安全的部署，以及更多开发人员为数据库做出贡献。

`atlasgo.io `

## [Postgres 每秒数十亿条边的计算](https://postgresweekly.com/link/171889/web)
OneSparse 简介，它是 Postgres 的一个扩展，使用 SuiteSparse 的 GraphBLAS 库将表转换为高性能稀疏矩阵，并转换回原形，无需外部图数据库。需要一些解释才能理解，但幸运的是，Michel 对此进行了深入的讲解。

`Michel Pelletier`

### **本周摘要**

* Claire Giordano 分享了她过去一年从 Talking Postgres 播客嘉宾[那里学到的丰富知识](https://postgresweekly.com/link/172195/web)。

* 🇮🇹 [PGDay Napoli](https://postgresweekly.com/link/172196/web) 将于 9 月 25 日在意大利那不勒斯举行。[以下是活动安排，现已开放报名](https://postgresweekly.com/link/172197/web)。

* [Percona 联合创始人 Peter Zaitsev](https://postgresweekly.com/link/172199/web) 是本周 PostgreSQL 人物的采访对象。

* Robert Haas [回顾了一年来举办 Postgres 黑客研讨会的经历](https://postgresweekly.com/link/172200/web)。

* Neon 用户？Neon 现在有一个 [VS Code 扩展](https://postgresweekly.com/link/172201/web)，可以将你的 Neon 数据库连接到本地开发环境。

## [Matrix 如何发现并恢复 Postgres 损坏问题](https://postgresweekly.com/link/172202/web)
Matrix 是一个流行的去中心化通信系统，尽管它确实为系统新手提供了一个“主服务器”。这个由大型 Postgres 实例支持的主服务器最近遇到了索引损坏问题，以下是其背后的详细故事。

`Richard van der Hoff`

📄 [PGDG 是谁？](https://postgresweekly.com/link/172205/web)——对你我来说，就是 PostgreSQL 全球开发小组。Laurenz Albe

📄 在 Postgres 18 中使用 [SQL:2023 属性图查询进行实验](https://postgresweekly.com/link/172206/web) Gavin Ray

📄 [使用 LLM 和 MCP 调试 Ruby on Rails 中的 Postgres 性能](https://postgresweekly.com/link/172207/web) Paweł Urbanek

📄 [在 Postgres 会议上发言的益处](https://postgresweekly.com/link/172208/web) Ashutosh Bapat

### **快速发布**

[PostGIS 3.6.0 Beta 1](https://postgresweekly.com/link/172209/web) – 强大的地理空间数据扩展。

🕒 [pg-when 0.1.9](https://postgresweekly.com/link/172214/web) – 使用自然语言创建时间值。

[Procrastinate 3.4](https://postgresweekly.com/link/172210/web) – 基于 Postgres 的 Python 任务队列。

[DoltgreSQL 0.51](https://postgresweekly.com/link/172211/web) – 类似 Postgres 的版本控制工具，具有 Git 风格的功能。

[Autobase 2.3.0](https://postgresweekly.com/link/172212/web) – 自托管 DBaaS/Postgres 平台。

[ParadeDB 0.17](https://postgresweekly.com/link/172213/web) – 用于搜索和分析的 Postgres。