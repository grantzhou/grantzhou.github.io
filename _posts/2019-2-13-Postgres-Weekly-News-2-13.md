---
layout: post
title: PostgreSQL 每周新闻 2019-02-13
---

### PostgreSQL每周新闻#292 - 2019年2月13日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/292)

![pg_img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/ochjwlkwxnggjvhl94sk.jpg)

## [将TB级的数据从Postgres加载到BigQuery中](https://dzone.com/articles/loading-terabytes-of-data-from-postgres-into-bigqu)
快速了解如何将大量数据从Postgres数据库传输到Google的[BigQuery](https://cloud.google.com/bigquery/)，这项功能可用于分析工作，或许可以向公众开放。

`PAVEL TIUNOV`

## [因为数据是您的业务](https://pgexperts.com/)
![pgx_img](https://copm.s3.amazonaws.com/27676a9c.png)
PGX的开源专家提供解决数据库问题，加速现有应用程序，重构基础架构和开发新应用程序所需的数据库和应用程序的相关技能。

`POSTGRESQL EXPERTS, INC.` **赞助商**

## [Postgres如何错误地使用fsync二十年](https://fosdem.org/2019/schedule/event/postgresql_fsync/)
这是一篇有趣的文章，文章关注的问题不仅是Postgres面临的而是很多系统都存在的问题，许多系统认为fsync（将文件缓冲区刷新进最终提交/持久状态的系统调用）的工作方式与它实际的工作方式不一致。“数据持久性/一致性带来灾难性后果”，如果您喜欢深挖，这是一个值得学习的有趣领域。不喜欢视频？[这个Postgres wiki条目](https://wiki.postgresql.org/wiki/Fsync_Errors)中有更多信息。

`TOMAS VONDRA`

## [SortSupport：Postgres如何快速排序](https://brandur.org/sortsupport)
这篇文章非常具有技术性，但如果您想了解SortSupport（Postgres中用于提高排序性能的系统之一),这是一篇很好的文章。“对已实施Sortsupport的类型进行排序通常会获得两倍或更多的速度，这种加速直接影响到常见的数据库操作，如ORDER BY，DISTINCT和CREATE INDEX。”

`BRANDUR LEACH`

## [Postgres11索引变化概述](https://severalnines.com/blog/overview-index-changes-postgresql-11)
PostgreSQL 11对处理数据库索引的方式进行了几处更改。这篇文章提供了概述，以及如何使用它们。

`AMIT JAIN`

## ▶[破坏大规模Postgres](https://fosdem.org/2019/schedule/event/breaking_postgresql_on_scale/)
这是一段50分钟的谈话，FOSDEM探讨了Postgres中的一些Scale“不连续性”以及如何减轻它们。 如果您不希望数据库在Scale时以奇怪的方式失败，这是一个有价值的谈话。

`CHRISTOPHE PETTUS`

## [pgDash最大化PostgreSQL性能](https://pgdash.io/)
pgDash提供时间序列仪表板，诊断，分析等，以帮助您最大限度地提高Postgres部署的性能。

`PGDASH BY RAPIDLOOP` **赞助商**

## [pg_stat_statements是最有用的Postgres扩展？](https://www.citusdata.com/blog/2019/02/08/the-most-useful-postgres-extension-pg-stat-statements/)
文章的灵感来自FOSDEM的PostgreSQL devroom的一个演讲，关于pg_stat_statements扩展的有用性以及为什么每个Postgres开发人员都应该在他们的toolbox中使用它。

`CRAIG KERSTIENS`

## [连接池，在Azure Database上使用PostgreSQL的最佳性能实践](https://azure.microsoft.com/en-us/blog/performance-best-practices-for-using-azure-database-for-postgresql-connection-pooling/)
关于改进Azure平台上数据库性能和Scale的一系列文章中的最新内容。

`PARIKSHIT SAVJANI`

## [快速推进和迁移：我们如何在Postgres中自动迁移](https://benchling.engineering/move-fast-and-migrate-things-how-we-automated-migrations-in-postgres-d60aba0fc3d4)
Benchling是一个生命科学数据管理平台，这意味着他们需要处理大量数据，就像上周的Braintree / PayPal一样，这篇文章可以很好地了解他们如何进行迁移。

# ![_config.yml]({{ site.baseurl }}/images/Tips-icon.png)   本周提示
如何在psql中查看查询所用的时间
来自 `Peter Cooper`

出于某种原因，我特别想知道事情花费的时间。我甚至在我的shell上有一个设置，在我的prompt中包含[最后一个命令的运行时间](https://jakemccrary.com/blog/2015/05/03/put-the-last-commands-run-time-in-your-bash-prompt/)。但是在使用psql时我们怎么能得到类似的东西呢？
这比你想象的要容易！ 只需输入：

`\timing` 

psql以“Timing is on”响应。如果您想要明确，也可以在最后添加on或off。

现在我们在运行查询时获得基本时间：

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/qhneibej28rs6gl3vilr.jpg)

如果你希望它是永久性的，那么在你的主目录中创建一个.psqlrc文件并将"\timing"置于其中，每次加载psql时它都会自动运行。

当然，这个提示仅用于改善您的日常psql体验。 如果您想真正深入挖掘查询时间，请使用EXPLAIN ANALYZE替换您的查询，然后您将更深入地了解其中的原因。但那是另一个提示了...... :-)

> 本周的技巧由[strongDM](https://postgresweekly.com/link/58601/web)赞助，这是保护您访问服务器/数据库的最佳方式。 [安排10分钟的演示](https://postgresweekly.com/link/58601/web)
