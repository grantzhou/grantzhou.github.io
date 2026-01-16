---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-12-11
---
### PostgreSQL每周新闻#581 - 2024年12月11日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/580)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/qetnbvmsxtbxsosfq2zc.jpg)
## [Electric：Postgres 同步引擎，现处于测试阶段](https://postgresweekly.com/link/163305/web)
看到一年前我们偶然提到的新项目取得成果总是令人欣慰的，这个用于在 Postgres 和众多其他服务（通过 HTTP）之间同步数据的实时引擎自那时起已经取得了长足的进步。GitHub 存储库。

`Kyle Mathews`

💡 如果您觉得 Electric 很熟悉，同一支团队创建了 [PGlite](https://postgresweekly.com/link/163307/web)，这是一种通过 WebAssembly 运行完整 Postgres 数据库的方法。（是的，您可以在浏览器中运行 Postgres。）

## [使用 DBOS 在 Postgres 中运行持久工作流](https://postgresweekly.com/link/163308/web)
了解 [DBOS](https://postgresweekly.com/link/163309/web)，这是一个由包括 Postgres 项目创始人之一在内的团队构建的“持久工作流”引擎。


`Paul Copplestone (Supabase) `
## [在 Postgres 上构建 AI 应用程序？](https://postgresweekly.com/link/163304/web)
从 pgai 开始 — pgai 是 PostgreSQL 的扩展，它为 PostgreSQL 带来了更多 AI 工作流，例如嵌入创建和模型完成。pgai 为开发人员提供 AI 超能力，使他们更容易构建搜索和检索增强生成 (RAG) 应用程序。


`Timescale `
## [▶ 700 多万张 Postgres 表](https://postgresweekly.com/link/163310/web)
一位工程师分享了一种有趣的大规模分析方法，该方法涉及创建大量的表（Postgres 对此没有问题），他坚定地站在“你可能不想这样做，但这肯定很有趣”的立场上。


`Kailash Nadh `

### 本周摘要：

* Peter Eisentraut 想知道 [Postgres 的所有用户都在哪里？](https://postgresweekly.com/link/163311/web)Postgres 显然有很多用户，但他们都在哪里闲逛，社区是否足够好？

* 🎤 微软 Postgres 工程副总裁 Affan Dar 在 [Talking Postgres 播客](https://postgresweekly.com/link/163312/web)上谈到了他的背景以及微软投资 Postgres 背后的策略。

* Cary Huang 分享了上个月在[西雅图](https://postgresweekly.com/link/163314/web)举行的 [2024 年 Postgres 大会](https://postgresweekly.com/link/163313/web)的亮点。

* DevClass 博客与 [Amazon Aurora DSQL](https://postgresweekly.com/link/163315/web) 团队讨论了[为什么 DSQL 目前缺少这么多核心 Postgres 功能](https://postgresweekly.com/link/163316/web)。最终，这是一项正在进行的工作。

* 🇫🇷 第 9 届[巴黎 pgDay](https://postgresweekly.com/link/163319/web) 将于明年 3 月在法国举行，他们的[征文活动](https://postgresweekly.com/link/163320/web)现已开放（截止至 12 月 31 日）。其他开放的 CFP 包括 [PGConf.dev 2025](https://postgresweekly.com/link/163321/web) 和 [Nordic PgDay 2025](https://postgresweekly.com/link/163322/web)。

* [Ben Nadel](https://postgresweekly.com/link/163323/web) 回顾了 Aaron Francis 的新 [Mastering Postgres](https://postgresweekly.com/link/163324/web) 课程。

* 🎄 如果解决 SQL 中的[ ]Advent of Code 挑战](https://postgresweekly.com/link/163317/web)不适合您，那么尝试一下 [Advent of SQL](https://postgresweekly.com/link/163318/web) 怎么样？


## [🤯 解释 Postgres 17.1 中的 ABI 破坏](https://postgresweekly.com/link/163325/web)
几周前，Postgres 17.1 发布，一些更改导致一些流行扩展出现问题。Postgres 17.2 迅速发布以解决该问题，但在这里我们可以了解更多事情背后的故事和技术细节。如果您是扩展开发人员，这肯定是需要注意的事情。


`Pavan Deolasee (EDB)`
## [具有检索增强生成的更智能的 Postgres LLM](https://postgresweekly.com/link/163327/web)
快速、易于理解的“RAG”概念介绍，其中通过提供来自额外数据源的附加上下文来改进大型语言模型的结果。


`Paul Ramsey (Crunchy Data)`


📄 [实现零停机时间 Postgres 主要版本升级](https://postgresweekly.com/link/163328/web) - Matt Long (Medplum)

📄[ ]冰山在前！分析 Postgres 中的运输数据](https://postgresweekly.com/link/163329/web) - Marco Slot (Crunchy Data)

📄 [使用 DOMAIN 执行 ELT 操作](https://postgresweekly.com/link/163330/web) - Robert Bernier (Percona)

📄 [了解 Postgres 中的等待事件](https://postgresweekly.com/link/163331/web) - Umair Shahid (Stormatics)

📄 [在 Postgres 中实现时间旅行](https://postgresweekly.com/link/163332/web) - Stefanie Janine Stölting



### 🛠 代码和工具

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/lv21byqtzyutb2ojpadl.jpg)

## [pgBadger 13.0：Postgres 日志分析工具](https://postgresweekly.com/link/163333/web)
一款注重性能的日志分析器，可生成详细的使用情况报告。这里有一个示例报告供您参考。


`Gilles Darold`
## [pg_worker_pool：创建后台工作进程池的扩展](https://postgresweekly.com/link/163333/web)
一个简单的扩展，依赖于 Postgres 的后台工作进程机制，可以轻松地在多个工作进程之间分配查询。


`Krzysztof Leśniak`

[pgtt-rsl 2.0](https://postgresweekly.com/link/163338/web) – 创建和管理 Oracle / DB2 样式的全局临时表。

[pgRoll 0.8](https://postgresweekly.com/link/163339/web) – 零停机时间、可逆的 Postgres 模式迁移。

[pgwire 0.28](https://postgresweekly.com/link/163340/web) – 在 Rust 库中实现的 Postgres 线路协议。

[pgai 0.3](https://postgresweekly.com/link/163304/web) – Timescale 的工具，用于处理 Postgres 中的 RAG 和 LLM。

[bb8 0.9](https://postgresweekly.com/link/163341/web) – 功能齐全的 Rust 异步 Postgres 连接池。

[DoltgreSQL 0.15](https://postgresweekly.com/link/163342/web) – 版本控制的 Postgres 类似程序。