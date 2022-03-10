---
layout: post
title: PostgreSQL 每周新闻 2022-3-2
---
### PostgreSQL每周新闻#444 - 2022年3月2日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/444)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/ueeegngjrj7ibpbgtzqs.jpg)
## [OrioleDB：Postgres 的新云原生存储引擎？](https://postgresweekly.com/link/120322/web)
这个项目还处于早期阶段，但 OrioleDB 是一个 Postgres 扩展，旨在为表的访问方式带来一些现代理念，包括撤消日志、写时复制检查点、行级 WAL 和无锁页面读取。 它处于 alpha 版本（仅限 Postgres 14），但这是一种值得关注的方法。

`Alexander Korotkov et al. `
## [停止浪费时间重写代码。 简化代码重用](https://postgresweekly.com/link/120323/web)
使用 Sourcegraph，您可以找到现有的代码库以进行重用，并避免将时间花在您知道队友已经解决的问题上。 这意味着更安全和连贯的代码库以及更多时间让您花在更有趣的工作上。


`Sourcegraph `
## [pgwatch2 v1.9 Beta 发布](https://postgresweekly.com/link/120324/web)
pgwatch2 是一个流行的 Postgres 监控和仪表板系统。 v1.9 带来了新的维护者、改进的开发过程、改进的性能和更好的连接池。 现在可以进行测试了。 


`Pavlo Golub `
## [SQL 中的字符串处理，艰难的方式](https://postgresweekly.com/link/120329/web)
我认为我以前从未见过与悬崖攀爬相比的字符串操作，但 Josh 向我们展示了一些类似的冒险地形，当涉及到使用 SQL 准确拆分和处理字符串时，regexp_split_to_table， 和 concat_ws。


`Josh Tolley `
## [Migra：就像 diff 但是对于 Postgres Schemas](https://postgresweekly.com/link/120330/web)
当然，您可以获取两个 SQL 文件并在它们之间运行 diff，但是 Migra 将事情提升到一个新的水平，并且“神奇地”计算出从 A 到 B 所需的 SQL，这可能很有用 . GitHub 存储库。


`djrobstep `
## [pg_back 2.1.0: A Simple and Thorough Backup Tool for Postgres](https://postgresweekly.com/link/120332/web)
一种工具（用 Go 编写），用于以您选择的格式将数据库转储到文件中，包括角色、服务器参数等。 在幕后使用 pg_dumpall 和 pg_dump 来获取您需要的所有数据。


`Nicolas Thauvin `
## [Studio 3T 管理您的数据，同时让您的应用程序成形](https://postgresweekly.com/link/120333/web)


`Studio 3T `
## [Postgres 13 和 14 中的逻辑复制/解码改进](https://postgresweekly.com/link/120334/web)
作者建议过去放弃逻辑复制的用户应该重新考虑，因为 PG 13+ 引入了重大改进。


`Jobin Augustine `
## [如何使用 SSIS 和 Babelfish 从 SQL Server 迁移到 Aurora PostgreSQL](https://postgresweekly.com/link/120335/web)
Babelfish 是 Amazon 的 T-SQL 到 Postgres 的兼容层，本文演示了使用它与 SQL Server Integration Services (SSIS) 一起从 SQL Server 迁移到 AWS 的 Aurora PostgreSQL 产品，如果 您有 SQL Server 工作负载。


`Barot and Venkatraman (AWS) `


