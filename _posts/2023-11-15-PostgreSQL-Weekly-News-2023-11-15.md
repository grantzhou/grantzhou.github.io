---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2023-11-15
---
### PostgreSQL每周新闻#530 - 2023年11月15日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/530)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/knva7pu6zhv8xiyp2f8j.jpg)
## [Postgres 16.1、15.5、14.10、13.13、12.17 和 11.22 已发布](https://postgresweekly.com/link/147767/web)
Postgres 11 到 16 的每个版本系列都进行了更新以修复三个安全问题，但 Postgres 16 在第一个小更新中还修复了许多错误。该团队指出，这是 Postgres 11 的最终版本，自五年前首次发布以来，现在被认为是“生命终结”


`PostgreSQL Global Development Group `
## [改进 NULL 处理的两个令人兴奋的 Postgres 功能](https://postgresweekly.com/link/147769/web)
覆盖UNIQUE NULLS NOT DISTINCT（在 Postgres 15 中引入）以及创建确保一组列中只有一个非 NULL 值的约束的能力。


`Paul Gross `
## [免费电子书：使用 Rails 和 Postgres 进行高级数据库编程](https://postgresweekly.com/link/147766/web)
了解 Postgres 和 Rails 中的子查询、物化视图和自定义数据类型。我们将介绍现实生活中的实际示例，首先将其转换为 SQL，然后转换为 Rails 代码。每个示例都附带源代码，因此您可以继续操作。


`pganalyze `
## [值得了解的 8 个最值得了解的 Postgres 扩展](https://postgresweekly.com/link/147770/web)
Timescale 工程师分享了他们使用的、令人兴奋的一系列扩展，涵盖了从 PostGIS 等大型流行扩展到不太常见的扩展pgpcre。


`Sewrathan and Clark (Timescale) `
**本周摘要：**
*   📅 PgConf.Dev 2024将于明年 5 月在加拿大温哥华举行 - 他们的论文征集截止到 1 月 15 日。注册即将开始。


*   在最近的AI 工程师峰会上，Supabase 的 Paul Copplestone 发表了关于 Supabase Vector及其pgvector基础的演讲。


*   RRedgate 的 Ryan Booz 和 Grant Fritchey 举办了一个长达一小时的▶️ 会议，主题是如何充分利用 Postgres 的文档和其他社区资源。他们忘了提到我们，但除此之外，一切都很好！😅


*   Bruce Momjian 表示，SCRAM 身份验证首次在 Postgres 10 中引入，并将继续存在。


## [Postgres 浮点、定位和排序带来的乐趣](https://postgresweekly.com/link/147777/web)
Greg 继续为 2022 年代码来临的基于 PL/pgSQL 的解决方案带来惊喜。这次郊游巧妙地将多项功能整合到一个地方。


`Greg Mullane `
## [PostgreSQL 迎来新的转机](https://postgresweekly.com/link/147778/web)
▶Alex Williams（ The New Stack 的）和 Jonathan Katz（Postgres 的核心贡献者）之间的 20 分钟聊天。他们讨论了 Postgres 16、某些功能为何需要如此长时间才能开发以及 Jonathan 的社区工作。


`The New Stack `


`EPIO`
## [kill -9Postgres 的解释](https://postgresweekly.com/link/147780/web)
如果您想以最突然的方式终止 Postgres 进程，请保持这种想法，直到您了解kill -9正常进程终止的工作原理以及 Postgres 如何处理它。


`Hans-Jürgen Schönig `
## [WiltonDB：Windows 上的 SQL Server 插件，由 Postgres 提供支持](https://postgresweekly.com/link/147782/web)
Babelfish是一个 Amazon 项目，可让 Postgres 理解 SQL Server 有线协议和 T-SQL 语言。WiltonDB 将 Babelfish 与 Postgres 打包在一起，并在 Windows 本身上提供它作为 SQL Server 的直接替代品。


`WiltonDB Software `
## [PGMQ：Postgres 上没有后台工作程序的轻量级消息队列-](https://postgresweekly.com/link/147785/web)
三个月前，Adam首次介绍了 PGMQ ，但现在解释了 PGMQ 如何在没有任何外部观察者的情况下保持消息队列干净地工作，这一切都归功于FOR UPDATE和SKIP LOCKED。


`Adam Hendel `
## [RisingWave 1.4：“类似 Postgres”的分布式 SQL 流处理](https://postgresweekly.com/link/147787/web)
不是Postgres，而是一个向具有有线协议兼容性的 Postgres 生态系统开放的项目。


`RisingWave Labs `
## [pg_stat_monitor 2.0.3](https://postgresweekly.com/link/147788/web)
 - 查询性能监控工具


## [temBoard 8.2](https://postgresweekly.com/link/147789/web)
 - 从 Web 界面管理 Postgres。


## [usql 0.16](https://postgresweekly.com/link/147790/web)
 - 用于 SQL 数据库的通用 CLI。


## [pspg 5.8.1 ](https://postgresweekly.com/link/147791/web)
 - 用于表格数据的 Unix 终端寻呼机


## [Hydra 1.0.2](https://postgresweekly.com/link/147792/web)
 - 面向列的 Postgres。


## [plpgsql_check 2.6.1 ](https://postgresweekly.com/link/147793/web)
 - PL/pgSQL linter。



# 💡本周提示


**🗓即将举办的Postgres活动**
