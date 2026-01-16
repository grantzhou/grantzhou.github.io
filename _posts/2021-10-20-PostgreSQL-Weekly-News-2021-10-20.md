---
layout: post
title: PostgreSQL 每周新闻 2021-10-20
---
### PostgreSQL每周新闻#427 - 2021年10月20日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/427)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/kraydsj5otbilupwhdvl.jpg)
## [函数管道：将函数式编程构建到 Postgres 中？](https://postgresweekly.com/link/115100/web)
Timescale 人员（他们支持以时间序列为重点的 TimescaleDB 扩展）的最新版本提供了一种编写更多功能 SQL 以通过将函数组合在一起来分析数据的方法。 给出的第一个例子很好地展示了这个想法。


`David Kohn (Timescale) `
## [Postgres 文本搜索：平衡查询时间和相关性](https://postgresweekly.com/link/115102/web)
Postgres 的 pg_trgm 提供了查询和搜索特定字符串的文本的方法（与更面向单词的 FTS 相反）。 Stephen 演示了特别是使用 pg_trgm 时的一些性能问题以及为什么需要权衡。


`Stephen Gutekanst (Sourcegraph) `
## [为 Postgres 数据库编制索引的更好方法：pganalyze 索引顾问](https://postgresweekly.com/link/115104/web)
我们都喜欢 Explain.depesz.com 分享 EXPLAIN 计划。 所以我们想：为什么不制作一个类似的免费工具，专门用于获取查询的索引建议？ 查看我们的免费 pganalyze 索引顾问并了解最适合您查询的索引。


`pganalyze `
## [OtterTune：RDS Postgres 的自动数据库调优服务](https://postgresweekly.com/link/115105/web)
我已提供一个链接到 Hacker News 的帖子，因为它有更多内容，但如果您愿意，可以直接访问 OtterTune 的主页。 OtterTune 是一种基于 2017 年论文中解释的概念构建的数据库优化服务，现在可供公众试用（仅限 RDS 部署）。 这是一个五分钟的解释。


`Andy Pavlo et al. `
## [升级 Amazon RDS 和 Aurora Postgres v9.6 数据库](https://postgresweekly.com/link/115109/web)
如果您使用 AWS 的任一托管 Postgres 服务并且正在使用 Postgres 9.6，您希望尽快继续您的升级故事。 否则，AWS 将在 2022 年初自动升级，如果您没有做好准备，这可能会导致问题。


`Chandra sekhar Pathivada (Amazon Web Services) `
## [在 Postgres 中预测每月收入运行率](https://postgresweekly.com/link/115110/web)
如果你曾经经营过一家公司或做过报告，你就会知道每个月的常规收入 (MRR) 和年常规收入 (ARR) 率有多重要，你可以计算它们 使用正确的 SQL 查询从 Postgres 存储的数据中提取。


`Jonathan S. Katz `
## [📈 如何使用 Postgres 和 TimescaleDB 执行数据评估任务](https://postgresweekly.com/link/115111/web)


`Timescale `
## [WITH HOLD 游标和事务](https://postgresweekly.com/link/115112/web)
本文描述了游标和事务如何交互，WITH HOLD 如何克服这些限制，以及一些注意事项和技巧。


`Laurenz Albe `
## [QGIS 是否可与 Postgres 14 一起使用？](https://postgresweekly.com/link/115113/web)
简而言之，是的。


`Elephant Tamer `
### 工具和代码
## [pgmetrics 1.12：从正在运行的 Postgres 服务器收集和显示统计信息](https://postgresweekly.com/link/115114/web)
用 Go 编写，这是其输出的示例。 v1.12 添加了 Postgres 14 和 PgBouncer 1.16 支持，包括收集新的 PG14 特定统计数据。 GitHub 存储库。


`RapidLoop `
## [pg_timetable 4.2 发布：Postgres 的高级作业调度](https://postgresweekly.com/link/115117/web)
最新的 4.2.0 版本修复了日志功能中的一个错误，鼓励任何用户立即升级。


`CYBERTEC PostgreSQL International GmbH `
## [可视化 Postgres Vacuum 进度](https://postgresweekly.com/link/115119/web)
这是一篇我想再次强调的“黄金”帖子！ 如果您的数据库的真空过程需要大量时间（就像这里一样），那么能够可视化其进度肯定是可取的，在这种情况下，一张图片真的值一千字。


`Dave Pacheco `

