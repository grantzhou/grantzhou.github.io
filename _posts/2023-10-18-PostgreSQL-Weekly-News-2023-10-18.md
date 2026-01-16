---
layout: post
title: PostgreSQL 每周新闻 2023-10-18
---
### PostgreSQL每周新闻#526 - 2023年10月18日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/526)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/ipt6vr1vss3fj89nfjkk.jpg)
## [在 Postgres 中使用 Money](https://postgresweekly.com/link/146461/web)
您知道 Postgres 有一种money类型吗？但伊丽莎白并不推荐这样做，而是考虑了一些替代方法。如果您想在浏览器中尝试帖子中提出的想法，还有一个实时环境。


`Elizabeth Christensen (Crunchy Data) `
## [PostgresqlCO.NF：Postgres 人类配置设置](https://postgresweekly.com/link/146464/web)
一份有用的在线参考指南，介绍 Postgres 的各种参数，从基础知识（如 和 ）log_statement到application_name最近在 v16 中添加的内容（如createrole_self_grant和 ）debug_parallel_query。


`OnGres, Inc. `
## [强类型和⛅：认识 EdgeDB 4.0](https://postgresweekly.com/link/146460/web)
EdgeDB 是一个专注于开发人员体验的开源数据库。它具有高级、现代数据模型、集成模式迁移和 TypeScript 查询生成器，可以轻松编写高级、快速查询，让 ORM 相形见绌。


`EdgeDB `
## [如何减少 Postgres 数据库大小](https://postgresweekly.com/link/146469/web)
在 Timescale 博客上，本文确实在一些地方倾向于特定于 Timescale 的功能，但也解释了广泛的一般概念，例如页面、元组、死元组和表膨胀，以及缓解措施一些常见的数据库大小问题。


`Paulus and Soto (Timescale) `
**本周摘要：**
*   Bruce Momjian称赞 Postgres 的多模式特性，并将其与花生酱和巧克力进行比较。


*   云平台 Vercel 已普遍提供其Vercel Postgres产品，并降低了测试期的价格。该服务由Neon在幕后提供支持。


*   如果您是 Ruby on Rails 开发人员，您应该了解上周发布的Rails 7.1 中的所有新 Postgres 功能。


*   Amazon RDS支持新的 M6in、M6idn、R6in 和 R6idn网络优化实例，吞吐量高达 200Gbps。


*   Supabase 添加了FDW，用于将数据从 Airtable 加载到 Supabase Postgres 数据库中。


*   📅 2023 年 PASS 数据社区峰会将于下个月在西雅图举行。有许多 Postgres 会议，演讲者 Ryan Lambert在日程表上有关于使用 PostGIS 的演讲，希望在那里见到您。


*   📅 2024 年巴黎 pgDay正在寻找赞助商。


## [终止长时间运行的查询](https://postgresweekly.com/link/146480/web)
长时间运行的查询很少受到欢迎，但可以检测并终止它们。statement_timeout也可用于在一段时间后自动删除它们。


`Hans-Jürgen Schönig `
## [使用 Vim 作为我的 Postgres 客户端](https://postgresweekly.com/link/146481/web)
通过管道将文件传输到psql.


`Thomas Stringer `


`pganalyze`
## [Postgres.js 3.4：适用于 JavaScript 平台的快速、功能齐全的 Postgres 客户端](https://postgresweekly.com/link/146484/web)
现在可与多个 JavaScript 平台（Node、Deno、Bun 以及截至此版本的Cloudflare）配合使用，这个高性能 Postgres 库提供实时更改订阅、动态通过特殊模板文字构建查询，通过多主机连接 URL、异步游标等提供高可用性支持。


`Rasmus Porsager `
## [PgBouncer：Postgres 的轻量级连接池](https://postgresweekly.com/link/146486/web)
尽管是 v1.21.0，但这是一个重要的版本，因为它增加了对协议级命名准备语句的支持（更多关于其工作原理。）。


`PgBouncer `
## [pg_yregress：TAP 兼容的测试执行](https://postgresweekly.com/link/146488/web)
TAP 兼容的测试执行器，可以实现更好的测试组织和工具标准化（相对于运行会话并通过比较标准输出上的预期输出和实际输出来实现测试）pg_regress。


`Omnigres `
## [适用于 Postgres v2.4 的 SQLite 外部数据包装器](https://postgresweekly.com/link/146489/web)
需要 Linux 或 POSIX 兼容系统，但现在支持 Postgres 16 并可与SQLite 3.42.0配合使用。


`PGSpider `
## [GatewayD：类似于 API 网关，但针对数据库](https://postgresweekly.com/link/146491/web)
SQL数据库和客户端的L4代理，因此您可以使用插件（提供的自写或社区），可观察性和连接池进行扩展。Postgres仅在目前，内置GO和AGPL许可。


`GatewayD Labs `
## [JSONb Accessor 1.4](https://postgresweekly.com/link/146492/web)
 - 将类型化 JSONB 支持的字段添加到 Ruby on Rails 中的 ActiveRecord 模型。


## [pgRoll 0.3](https://postgresweekly.com/link/146493/web)
 - 零停机迁移使 Postgres 14+ 变得容易。


## [Que 2.3](https://postgresweekly.com/link/146494/web)
 - 使用 Postgres 咨询锁的 Ruby 作业队列。


## [pgrx 0.11](https://postgresweekly.com/link/146495/web)
 - 一种使用 Rust 构建 Postgres 扩展的方法。  



# 💡本周提示


**🗓即将举办的Postgres活动**
