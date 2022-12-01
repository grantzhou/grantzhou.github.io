---
layout: post
title: PostgreSQL 每周新闻 2022-11-23
---
### PostgreSQL每周新闻#482 - 2022年11月23日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/482)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,w_430,h_100/e_make_transparent/co_white,e_outline:7/xyflkz7n00elwtgja9ne.png)
## [Variadic Unnesting 的力量](https://postgresweekly.com/link/132013/web)
本周没有明显的“大新闻”，所以让我们来看看“整洁的 Postgres 功能！” （从 Postgres 9.4 开始）。 这是对 string_to_array 和 UNNEST 表函数如何帮助规范化杂乱数据（在本例中来自电子表格）的了解。 正如作者所说：“在我使用过的其他数据库中，我做不到这么棒的事情。”


`Leo Hsu and Regina Obe `
## [Timescale 在 S3 之上的“无底”对象存储层](https://postgresweekly.com/link/132014/web)
Timescale 继续通过其云服务进行创新，这次是在 Amazon S3 上构建的（目前仅限私人测试版）对象存储机制。 这个想法是数据可以跨磁盘和 S3 分层，同时保持访问透明。


`Mike Freedman (Timescale) `
## [我们都是为了提供强大的支持](https://postgresweekly.com/link/132012/web)
“我从我提交的@crunchydata 支持票中学到了很多关于@PostgreSQL 的知识。 他们知道他们的 Postgres，这是肯定的！” - @frigidcode


`Crunchy Bridge `
## [使用 pgBadger 分析 Postgres 日志的无服务器架构](https://postgresweekly.com/link/132015/web)
pgBadger 是一种日志分析工具（用 Perl 编写），可生成显示有关数据库流量、锁定、最慢查询等统计信息的报告。 这篇文章的重点是在无服务器架构中部署它，其中 AWS RDS 通过 SQS 和 AWS Lambda 将日志发送到 S3，然后发送到 pgBadger，后者再次将其报告输出到 S3……哇！


`Sarabu, Dave, and Townsend (AWS) `
## [使用 ANY 而不是 IN 来提升查询？](https://postgresweekly.com/link/132018/web)
Matt 提出了在更多可能使用 IN(list) 的情况下使用 = ANY(array)（或 SOME）的案例。


`Matt Hudson `
## [不同的相等谓词会有所不同吗？](https://postgresweekly.com/link/132024/web)
即，IN 与 =。 剧透：不，至少对于 Postgres 13 是这样。 但由于数据库之间的行为差异，始终值得检查。

## [在 psql 中使用 Emacs 作为编辑器](https://postgresweekly.com/link/132025/web)
通过 emacsclient

`LUCA FERRARI`

`Frits Hoogland `
## [Dalibo Postgres 执行计划可视化工具](https://postgresweekly.com/link/132026/web)
提供 EXPLAIN ANALYZE 的输出并更好地了解 Postgres 计划对您的查询执行的操作。 这已经有一段时间了，并且会继续看到频繁的更新，包括本周。 如果您想在本地或应用程序中使用它，它是开源的。


`Dalibo `
## [Squeal：Haskell 中 SQL 的“深度嵌入”](https://postgresweekly.com/link/132028/web)
本质上是一个将 SQL 概念和类型原生引入 Haskell 的客户端库，因此您可以尽可能地在功能上组合查询。


`Morphism Tech `
## [Dynaboard：专为开发人员打造的 Pro-Code Web App Builder](https://postgresweekly.com/link/132029/web)


`Dynaboard `

