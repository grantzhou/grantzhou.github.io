---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2023-12-6
---
### PostgreSQL每周新闻#533 - 2023年12月6日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/533)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/abbflozzmeokknncagpr.jpg)
## [使用 Postgres 的提示和技巧代码的出现](https://postgresweekly.com/link/148647/web)
年度会议 编程竞赛又回来了！ Greg 是使用 SQL 和 PL/pgSQL 来解决挑战的老手，所以如果您也想尝试一下，他在这里解释了如何开始以及一些 Postgres 特定的提示和技巧（这对于其他任务很有用）也是！）


`Greg Sabino Mullane `
## [降低 AWS 上的云支出并提高 Postgres 性能](https://postgresweekly.com/link/148646/web)
如果您正在努力应对 AWS RDS 或 Aurora 成本增加和性能下降的问题，那么是时候考虑 EDB Postgres 了。优势包括：高可用性选项、随时可用的 Postgres 专家、Oracle 兼容性和透明定价。 AWS+EDB Postgres 结合起来效果更好。


`EDB Postgres `
## [每个人的 Postgres 活动体验](https://postgresweekly.com/link/148649/web)
作为最新 PGSQL Phriday 博客活动的一部分，许多 Postgres 用户写下了他们参加各种 Postgres 聚会和会议的经历。如果您从未去过任何地方，您可能会发现这些文章很有启发性。 Michael Christofides 分享了他的想法，Claire Giordano 在 2023 年 PASS 数据峰会上制作了史诗般的 Postgres 图解指南可以享受。很多，还有更多。这里有▶️ 长达一小时的活动节目，Postgres.fm 做了


`Pavlo Golub et al. `
**本周摘要：**
*   ⭐️我还没有找到关于它的大文章还但它似乎Heroku正在将其 Postgres 平台迁移为在后台使用 Amazon Aurora – 这是一个巨大的进步。


*   PowerSync 是一个新的 Postgres 到 SQLite 双向同步层。


*   Richard Hipp 坚持使用 SQLite，推出了SQLite 中 JSON 支持的巨大发展 因此，现在 SQLite 与 Postgres 一样，同时具有 JSON 和JSONB..😄


## [您可以从WAL中提取SQL吗？](https://postgresweekly.com/link/148656/web)
给定 wal_level 的“副本”，是否有可能从此类 WAL 中提取 SQL ？ Julien 在系列文章的第一篇中表示，通常情况下不会，但如果您深入挖掘，您可以提取出许多有用的东西 。


`Julien Rouhaud `
## [One Team 的 Postgres 数据库优化故事](https://postgresweekly.com/link/148657/web)
这是一个古老的故事：您启动一个应用程序，它变得流行，数据库开始出现压力。这就是一个团队监控正在发生的情况并推出一些修复措施的方式。


`Miroslav Bajtoš `
## [关闭光标](https://postgresweekly.com/link/148658/web)
Ora2Pg 等工具可以将 Oracle 数据、过程和函数移植到Postgres，但随着任何重大的架构变化，细微的差异可能会导致奇怪的结果，如下所示。


`Pavel Stěhule `
## [使用物化视图创建快速时间序列图](https://postgresweekly.com/link/148661/web)
从 Postgres 方法开始，然后再转向 Timescale 的连续聚合。一个>


`Dylan Paulus (Timescale) `
## [pgxman：就像 npm 对于 Postgres](https://postgresweekly.com/link/148662/web)
Postgres 拥有丰富的扩展生态系统 (PGXN 提供了一种遵循它们的方法），但安装它们可能很棘手。已经有很多清理工作的尝试，例如 Supabase 的 dbdev，而 Hydra 正在尝试 pgxman （“Postgres 扩展管理器”）采用了更像 npm 的方法。


`Joe Sciarrino (Hydra) `


`Redgate`
## [pguint：无符号整数类型扩展](https://postgresweekly.com/link/148667/web)
将有符号 8 位整数和无符号 8、16、32 和 64 位整数类型引入 Postgres 9.1+（仅限 64 位平台） .


`Peter Eisentraut `
## [check_pgactivity 2.7：适用于 Nagios 的 Postgres 插件](https://postgresweekly.com/link/148668/web)
如果您使用 Nagios 进行监控，请使用它来监控 Postgres。 v2.7 添加了 Postgres 15/16 支持。


`OPM Development Group `
## [PLV8ify：将 JavaScript 文件转换为 PLV8 函数](https://postgresweekly.com/link/148669/web)
捆绑 TS/JS 输入并使用 PLV8 扩展编写包含 Postgres 函数的 SQL。似乎还处于早期阶段。


`Divyendu Singh `
## [无状态 Postgres 查询路由器 1.0](https://postgresweekly.com/link/148670/web)
 -  Yandex 的水平分片方法。 (GitHub 存储库。)


## [适用于 Kubernetes 5.5 的 Crunchy Postgres](https://postgresweekly.com/link/148672/web)
 -  


## [ScalikeJDBC 4.1](https://postgresweekly.com/link/148673/web)
 -  用于 Scala 的基于 SQL 的数据库访问库。


## [Schemalint 1.0.5](https://postgresweekly.com/link/148674/web)
 -  架构 linter。  



# 💡本周提示


**🗓即将举办的Postgres活动**
