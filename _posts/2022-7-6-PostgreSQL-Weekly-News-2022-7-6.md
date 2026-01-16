---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2022-7-6
---
### PostgreSQL每周新闻#462 - 2022年7月6日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/462)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/ruzzofs1h8hvnvx0wqoz.jpg)
## [了解pg_stat_activity](https://postgresweekly.com/link/125812/web)
pg_stat_activity提供了一种简单的方法来查看不同的 Postgres 后端进程在做什么。休伯特深入研究了它的各种价值实际代表什么。


`Hubert depesz Lubaczewski `
## [PostgreSQL 15 Beta 2发布](https://postgresweekly.com/link/125813/web)
Postgres 的巨大功劳在于投入了大量精力以使主要版本恰到好处，因此在第一个 beta 版发布五周后看到第二个 beta 版并进行了大量修复令人欣慰。我们鼓励您继续帮助测试，更新的（测试版）发行说明仍保留在此处。


`PostgreSQL Global Development Group `
## [使用 Retool，您可以将所有来源的数据加入到一个 CRUD 应用程序中](https://postgresweekly.com/link/125815/web)
Retool 在几分钟内连接到您的 PostgreSQL 数据库，并可以轻松地在您的 PostgreSQL 数据之上构建管理面板、仪表板和实用程序。此外，借助 Retool，您可以使用 REST 或 GraphQL API 连接到其他数据源——所有这些都在一个内部应用程序中。


`Retool `
## [如何记录特定表中的选择？](https://postgresweekly.com/link/125816/web)
使用PGAudit 的实用介绍。很高兴能够使用这种功能。


`Hubert depesz Lubaczewski `
## [事务异常与Select for Update](https://postgresweekly.com/link/125818/web)
“我最近遇到了一个很好的例子，说明添加FOR UPDATE到查询中如何引入事务异常。” 幸运的是，Laurenz 有一些处理这种情况的技巧。（如果您不知道，FOR UPDATE锁定选定的行以防止并发更新，就像您可能希望在事务中做的那样。）


`Laurenz Albe `
## [postgresql中的查询：嵌套循环](https://postgresweekly.com/link/125823/web)
Egor 的详细且技术含量高的 Postgres 帖子总是受到欢迎，他继续深入研究连接方法以及 Postgres 14 如何引入一种方便的技术来加速重复循环。


`Egor Rogov `
## [如何推理为您的 Postgres 数据库编制索引（按需网络研讨会）](https://postgresweekly.com/link/125824/web)
l,null,"en


`pganalyze `
## [在 SQL 中处理“奖励程序”](https://postgresweekly.com/link/125825/web)
看看如何将逻辑引入数据库总是很有趣。此示例围绕使用窗口函数来收集跨时间范围的数据，例如公司奖励计划可能使用的数据。


`Hans-Jürgen Schönig `
## [Antares SQL：新（ISH）开源SQL客户端](https://postgresweekly.com/link/125827/web)
一个基于 Electron 的跨平台客户端，具有一些雄心勃勃的目标。到目前为止支持 MySQL/MariaDB、Postgres 和 SQLite，更多的还在路上。看起来很有希望！


`Fabio Di Stasio `
## [OctoSQL：使用 SQL 连接、分析和转换来自多个源的数据](https://postgresweekly.com/link/125828/web)
一种由 Go 驱动的 CLI 工具，用于查询“过多”源（包括 CSV 文件、JSON、MySQL、Postgres、Redis 和 Parquet），甚至在它们之间进行连接。


`Jacob Martin `
## [EverSQL Online SQL 查询优化工具](https://postgresweekly.com/link/125829/web)
这远不是第一个这样的工具，当然也不是最简单的，但这个索引顾问涵盖了许多数据库，包括 Postgres，值得一看。


`EverSQL `
# 💡本周提示


**🗓即将举办的Postgres活动**
