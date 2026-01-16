---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2022-6-1
---
### PostgreSQL每周新闻#457 - 2022年6月1日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/457)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/zusgmvmazvtcrp1lw9bx.jpg)
## [Neon：AWS Aurora Postgres 的开源无服务器替代方案？](https://postgresweekly.com/link/124164/web)
这是一家同名公司（由 Nikita Shamgunov 创立，他是 MemSQL 的共同创始人）背后的代码库，该公司构建了一个多云无服务器 Postgres 平台，现在为我们提供了强大的PlanetScale氛围，但有额外的资源


`Neon `
## [关于视图权限和行级安全性](https://postgresweekly.com/link/124167/web)
视图提供了一种方便的方式来访问预定义的 SQL 查询，并且它们还可以通过限制对视图基础表的访问同时仍然允许使用视图来用作额外的安全层。这篇文章涵盖了基础知识，同时也介绍了 Postgres 15 即将推出的security_invoker选项。


`Laurenz Albe `
## [P弹性规模的 Postgres 可能性？这就是 CockroachDB](https://postgresweekly.com/link/124169/web)
与来自 AWS 和 GCP 的 Postgres 托管服务不同，自动扩展 CockroachDB 让您可以使用熟悉的语法快速构建、最小化操作并按需付费。再加上云的自由度，可以随心所欲地部署您的工作负载。


`Cockroach Labs `
## [深入了解 AlloyDB 的 Columnar Engine](https://postgresweekly.com/link/124170/web)
 两周前，我们提到了 Google 发布的AlloyDB，这是它与 Aurora-a 类似的 Postgres 兼容的可扩展托管数据库。这篇文章更深入地探讨了它的独特功能以及列式引擎如何在某些类型的查询上实现（显着）更快的性能。


`Sheshadri Ranganath (Google Cloud) `
## [来自 Aurora PostgreSQL 的近实时通知，带有触发器、Lambda 和 SNS](https://postgresweekly.com/link/124172/web)
这是 AWS 非常适合的那种管道工作。本教程介绍了启用 Postgres 兼容 Aurora 数据库上的数据更改通知的过程，该通知通过无服务器功能发送，然后通过 SNS 发送到其他地方。请注意不要在每次表格添加新行时向自己发送电子邮件.. ;-)


`Wajid Ali Mir and Anjan Mukherjee `
## [pgAdmin 4 的架构](https://postgresweekly.com/link/124173/web)
pgAdmin是一个流行的基于浏览器的 Postgres 仪表板和管理工具，如果您想知道它有哪些活动部分，这些图表适合您。您是否意识到 pgAdmin 有一个不是Postgres 核心的数据库......？


`Yogesh Mahajan (EDB) `
## [Compose Transporter 1.1：在持久性引擎之间同步数据](https://postgresweekly.com/link/124175/web)
我喜欢它如何自我标榜“就像 ETL 一样，只是不乏味”。这个由 Go 驱动的工具可让您将各种数据库（MongoDB、Postgres、MySQL、Elasticsearch 等）、文件和其他资源连接在一起，运行一些基本转换（可选），然后将数据发送到其他地方。所以，是的，基本上是 ETL。


`Compose `
## [如何使用PG_RMAN备份和还原数据](https://postgresweekly.com/link/124176/web)
pg_rman是我们之前没有提到的 Postgres 备份和恢复工具，但它已经存在很多年了，并且支持到 Postgres 15 beta。它的目标是像pg_dump在线备份一样简单易用。


`David Zhang `
## [从 DuckDB 查询 SQLite 和 Postgres 数据](https://postgresweekly.com/link/124178/web)
PostgresScanner提供了DuckDB、流行的进程内 SQL OLAP DBMS（想象 SQLite，但用于 OLAP）和 Postgres之间的 FDW 样式集成


`Cupper `
## [只需 5 分钟即可了解最新的初创公司、技术和编程](https://postgresweekly.com/link/124181/web)
l,null,"en


`TLDR Newsletter `
## [Exporter2Perfdata：连接 Postgres 监控工具](https://postgresweekly.com/link/124182/web)
exporter2perfdata是一个新的开源工具（用 Go 编写），它从 Prometheus 导出器收集指标并将其转换为 Icinga 2 / Nagios 的 perfdata 格式。


`Crunchy Data `
## [托管PostgreSQL服务指南](https://postgresweekly.com/link/124184/web)
一个基本但有用的列表和一系列注意事项。


`Dan Townsend `
# 💡本周提示


**🗓即将举办的Postgres活动**
