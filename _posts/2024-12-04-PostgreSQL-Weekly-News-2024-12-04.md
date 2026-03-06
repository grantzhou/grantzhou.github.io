---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-12-04
---
### PostgreSQL每周新闻#580 - 2024年12月04日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/580)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/fv3u0ffwlfvxgutpwsb1.jpg)
## [Amazon Aurora DSQL：一款新的 Postgres 兼容数据库](https://postgresweekly.com/link/163026/web)
目前处于“预览”阶段，DSQL 承诺具有高可用性和强一致性的“几乎无限的可扩展性”，同时兼容 Postgres（有点……？没有视图、触发器、JSON 或外键约束……）。AWS 英雄 AJ Stuyvenberg 称其为“我最近从 AWS 看到的最令人兴奋的发布”，因此请关注此消息。（[官方新闻稿](https://postgresweekly.com/link/163029/web)。）

`Amazon Web Services`

💡 AWS 的 Marc Brooker 撰写了一篇[关于 DSQL 的个人博客文章](https://postgresweekly.com/link/163030/web)，对 DSQL 进行了更详细的解释，并解释了其架构中的一些选择。

## [Honeybadger 的全栈可观察性](https://postgresweekly.com/link/163025/web)
Honeybadger 的新日志平台有点像 Splunk、DataDog 或 CloudWatch Logs，但只具有优秀的组件和合理的价格。此外，它还易于与 Crunchy Bridge、Journald、AWS 等集成！


`Honeybadger `
## [我希望有人告诉我有关 Postgres 的知识](https://postgresweekly.com/link/163031/web)
各种各样的实用技巧，涵盖从规范化和不同类型的使用到 SQL“怪癖”、锁和 JSONB 的使用等领域。


`Hazel Bachrach `

### 本周摘要：

🌐 PostGIS Day 2024 于两周前举行，▶️ [所有视频现在都在 YouTube 上](https://postgresweekly.com/link/163032/web)。如果您更喜欢活动进展的文字介绍，[Paul Ramsey 在此处提供了摘要](https://postgresweekly.com/link/163033/web)。

🇩🇪 [PostgreSQL 德国会议](https://postgresweekly.com/link/163034/web) 2025 将于明年 5 月 8 日至 9 日在柏林举行。如果您想[发言](https://postgresweekly.com/link/163035/web)，征文截止日期为 2025 年 2 月 1 日。

亚马逊推出了 [Amazon S3 Tables](https://postgresweekly.com/link/163036/web)，这是一种在 S3 上存储和查询 Iceberg 格式表格数据的方法。


## [使用 pg_karnak 跨租户数据库进行事务模式迁移](https://postgresweekly.com/link/163037/web) 
如果您运行的设置中系统的每个租户/用户都有自己的数据库，那么维护它们之间的模式很快就会变得棘手。pg_karnak 是 Nile 的分布式 DDL 层，用于协调租户之间的模式。它尚未开源，但这篇文章深入探讨了它的工作原理。


`Gwen Shapira (Nile)`
## [子字符串函数，正则表达式风格](https://postgresweekly.com/link/163038/web) 
虽然您可以使用 Postgres 的子字符串函数通过数字索引提取字符串的部分，但您是否知道它也支持使用正则表达式？


`Leo Hsu and Regina Obe`
## [优化 Postgres 性能和压缩](https://postgresweekly.com/link/163039/web) 
pglz 与 LZ4 — 您知道可以更改用于压缩 TOAST 数据的算法吗？如果 LZ4 的


`Keyur Panchal (Timescale)`

📄 [使用 Knex 和 pipeline 编写可组合 SQL](https://postgresweekly.com/link/163040/web) – Knex.js 是 JavaScript 领域中流行的 SQL 查询构建器 - Aycan Gulez

📄 [插入期间违反唯一约束可能会导致膨胀](https://postgresweekly.com/link/163042/web) - Josef Machytka


### 📰 分类广告


🚀 [pgai Vectorizer](https://postgresweekly.com/link/163043/web) 使用一个 SQL 命令自动在 Postgres 中创建和同步嵌入 — 保持嵌入更新，无需任何工具。

🚀 想要快速、准确的搜索？使用 [MongoDB Atlas Vector Search](https://postgresweekly.com/link/163044/web) 增强您的查询能力。


### 🛠 代码和工具

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/dlezaivmlaxmsnscjpf6.jpg)

## [Supabase Cron：Postgres 中的作业调度](https://postgresweekly.com/link/163045/web)
使用 pg_cron 扩展来管理 Supabase 平台上的重复作业的模块（通过仪表板或 SQL）。


`Vasilov, Rice, and Sutton (Supabase)`

🤖 [pgai v0.2](https://postgresweekly.com/link/163047/web) – Timescale 的工具，用于处理 Postgres 中的 RAG 和 LLM。在 v0.2 中，其矢量化器现在支持 Ollama。

[pgwire 0.27](https://postgresweekly.com/link/163048/web) – 在 Rust 库中实现的 Postgres 线路协议。

[PgParty 1.9](https://postgresweekly.com/link/163049/web) – 使用 Ruby 从 Active Record 创建 Postgres 分区。