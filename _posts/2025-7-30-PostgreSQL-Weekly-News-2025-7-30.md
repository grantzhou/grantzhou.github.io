---
layout: post
title: PostgreSQL 每周新闻 2025-7-24
---
### PostgreSQL每周新闻#608 - 2025年7月24日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/609)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/khrspmmtn99ujhlnerps.jpg)
## [让 Postgres 慢 42,000 倍（因为我失业了）](https://postgresweekly.com/link/172500/web)
我们做了很多关于如何最大限度地利用 Postgres 并使其运行得尽可能快速顺畅的项目，但是你能从另一个角度尝试让 Postgres 尽可能慢来学到一些东西吗？这看似毫无意义的练习，但却是一个了解 Postgres 某些配置选项实际作用的好方法。

`Jacob Jackson`

💡 如果您更喜欢更直接可用的东西，Jacob 还编写了一个关于[调优 Postgres 的快速介绍](https://postgresweekly.com/link/172501/web)。

## [使用 pganalyze 查询顾问加速 Postgres 查询](https://postgresweekly.com/link/172499/web)
了解我们全新的查询顾问功能如何检测计划问题，并将 Postgres 查询速度提升 1000 倍以上。观看网络研讨会，了解如何识别低效查询、获取重写建议并跟踪改进。


`pganalyze  `

### **本周摘要**

📊 [Stack Overflow 2025 年调查结果已出炉](https://postgresweekly.com/link/172503/web)，Postgres 稳居最常用[数据库榜首](https://postgresweekly.com/link/172504/web)，这对 Postgres 来说是个好消息，尽管 MySQL 在学习者中占据领先地位。

EDB 博客分享了 Bruce Momjian [在全球各地谈论 Postgres 的最新动态](https://postgresweekly.com/link/172505/web)。

[Polina Bungina](https://postgresweekly.com/link/172506/web) 是本周 PostgreSQL 人物的受访者。

🤖 Postgres AI 正在开发一个[开源的“自动驾驶 Postgres”项目](https://postgresweekly.com/link/172502/web)。


## [以网络速度对 Postgres 进行分片](https://postgresweekly.com/link/172507/web)
PgDog 事务池/Postgres 分片工具的首席开发人员分享了 PgDog 新的基于高速逻辑复制的重新分片功能的技术细节。


`Lev Kokotov `


📄 [Postgres 为何需要更好的连接安全默认值](https://postgresweekly.com/link/172509/web)——了解 sslmode=require 和 sslmode=verify-full 之间的区别至关重要。George MacKerron (Neon)

📄 [CERN 如何利用 TimescaleDB 助力突破性物理学研究——一个案例研究](https://postgresweekly.com/link/172510/web)，其中包含一些来自欧洲科学产业核心的有趣技术花絮。TigerData

📄 [迁移和升级：在 Postgres 中实现近乎零停机](https://postgresweekly.com/link/172511/web) Sebastian Insausti

📄 [从 Postgres CDC 到 Iceberg](https://postgresweekly.com/link/172512/web)：从实际数据管道中汲取的经验教训 Yingjun Wu (RisingWave)


### **📰 分类广告**

🐘 [Atlas](https://postgresweekly.com/link/172513/web) 管理 Postgres，就像 Terraform 管理基础设施一样。将模式定义为代码，并安全地规划和应用迁移。了解更多。

💌 您知道我们有一系列新闻简报吗？查看 [JavaScript 周刊](https://postgresweekly.com/link/172514/web)、[Go 周刊](https://postgresweekly.com/link/172515/web)和 [Ruby 周刊](https://postgresweekly.com/link/172516/web)，更全面地了解我们的工作。


### **发布**

## [pg_meminfo：适用于 Linux 的 Postgres 内存使用情况统计工具](https://postgresweekly.com/link/172517/web)
一个仅限 Linux 的扩展程序，可使用简单的 SQL 查询检查每个后端的详细内存使用情况。它会显示每个后端进程的 pss 等指标，从而更轻松地诊断内存问题或调查泄漏。Shaun 还建议，这段代码可以作为其他希望构建类似扩展程序的学习练习。

`Shaun Thomas`

## [pgsql-http 1.7：Postgres 的 HTTP 客户端](https://postgresweekly.com/link/172518/web)
如果能编写一个触发器来调用 Web 服务，那岂不是很棒？要么返回结果，要么让 Web 服务根据数据库的新状态进行自我刷新？

`Shaun Thomas`


[Mathesar 0.4](https://postgresweekly.com/link/172519/web) – 类似电子表格的 Postgres 表界面。

[DbGate 6.6](https://postgresweekly.com/link/172520/web) – 适用于 SQL 和 NoSQL 数据库的数据库管理应用。

[Supavisor 2.6](https://postgresweekly.com/link/172521/web) – Supabase 的多租户 Postgres 连接池。

[RisingWave 2.5](https://postgresweekly.com/link/172522/web) – 兼容 Postgres 的流式数据库。

[Bob 0.39](https://postgresweekly.com/link/172523/web) – 适用于 Go 语言的 SQL 查询构建器和 ORM/Factory 生成器。

[Piccolo 1.28](https://postgresweekly.com/link/172524/web) – 用户友好的 Python ORM 和查询构建器。

[Prisma 6.13](https://postgresweekly.com/link/172525/web) – 下一代 Node.js + TypeScript ORM。

[pgAdmin 4 v9.6](https://postgresweekly.com/link/172526/web) – 流行的 Postgres 管理工具。