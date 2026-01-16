---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2022-3-30
---
### PostgreSQL每周新闻#448 - 2022年3月30日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/448)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/xbcdz4ircyusbijt34qg.jpg)
## [MERGE 来到 Postgres 15](https://postgresweekly.com/link/121585/web)
在 Postgres 文档中看到一个全新的页面总是很高兴——即使它是在今年晚些时候发布的。 这是一个用于 MERGE（您可能在 SQL Server 或 Oracle 中看到的 SQL 语句）——基本思想是在可定义的条件下将来自查询或源表的数据整体合并到目标表中。


`PostgreSQL Documentation `
## [Citus 11 现在处于 Beta 版](https://postgresweekly.com/link/121586/web)
Citus 是一个开源 Postgres 扩展，它“将 Postgres 转换为分布式数据库”，11 中的重大更新是模式和元数据同步，因此始终可以从集群中的任何节点查询分布式表。


`Citus Data / Microsoft `
## [Studio 3T 管理您的数据，同时让您的应用程序成形](https://postgresweekly.com/link/121587/web)
Studio 3T 的全套 MongoDB 工具可让您更快地查询，更快地使用数据进行开发，并自动将查询转换为代码。 免费试用 30 天 - 无需信用卡。


`Studio 3T `
## [Citus Con 终极指南：Postgres 活动](https://postgresweekly.com/link/121591/web)
还有不到两周的时间，Citus / Microsoft 团队非常、非常、非常渴望让您享受他们的免费活动，无论是现场直播还是稍后点播观看会议。 这篇文章深入探讨了会谈将在哪些地方进行。


`Citus Data `
## [如何毫无问题地删除角色或删除用户](https://postgresweekly.com/link/121592/web)
通常情况下，我们设置了我们的数据库，很少考虑删除对他们有权力的用户和角色。 然而，考虑到依赖关系的潜在问题，它并不像你想象的那么简单。


`Laurenz Albe `
## [在 EKS 上安装 Crunchy Postgres Operator v5](https://postgresweekly.com/link/121593/web)

`BO PENG`
## [Postgres.js 3.0：适用于 Node 和 Deno 的快速、全功能 Postgres 客户端](https://postgresweekly.com/link/121594/web)
现在对于 Deno 和 Node.js，这个高性能 Postgres 库提供实时更改订阅、通过特殊模板文字构建动态查询、大对象、高可用性 通过多主机连接 URL、异步游标等。 Slonik 也是在这个领域考虑的另一个选择。


`Rasmus Porsager `
## [pg_plan_guarantee：保持你的计划到位](https://postgresweekly.com/link/121596/web)
微调查询以从 Postgres 的计划器中获取正确的执行计划是围绕这些部分的常见爱好，但是当事情发生变化并且突然 Postgres 的计划器决定单方面改变路径时怎么办？ 这个扩展的承诺是“将你的执行计划一成不变”，考虑到你的用例，这可能是一个好主意，也可能不是一个好主意。 请注意，这是一个处于 alpha 阶段的新项目，可能会产生意想不到的后果！


`Gurjeet Singh `
## [Lyft 的移动团队如何大规模实施移动 CI](https://postgresweekly.com/link/121597/web)


`Buildkite `
## [PgBouncer 1.17.0 发布：轻量级连接池](https://postgresweekly.com/link/121598/web)
新功能和一些修复。 数据库定义现在可以指定主机列表。 密码的最大长度已增加。 已修复对 OpenSSL 3 的支持。


`PgBouncer Authors `
## [Quickgres 0.4.2：纯 JavaScript Postgres 客户端库](https://postgresweekly.com/link/121599/web)
有趣的是看到一个 Postgres 客户端库直接与有线协议通信，没有外部依赖。 如果你想看看它是如何工作的，它也几乎都在一个 JS 文件中。


`Ilmari Heikkinen `
## [ETL Helper：一个用于数据库到数据库传输的 Python 库](https://postgresweekly.com/link/121601/web)
一个为 Pythonistas 准备的。 与 Postgres、SQLite、SQL Server 和 Oracle 一起使用，我很喜欢它来自英国地质调查局。

`British Geological Survey `
## [usql 0.10.0：用于数据库的通用 CLI 工具](https://postgresweekly.com/link/121603/web)
它的灵感来自 psql，但添加了更多功能并支持大量数据库，包括关系数据库和 NoSQL。


`Kenneth Shaw `

