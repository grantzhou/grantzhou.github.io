---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2021-3-10
---
### PostgreSQL每周新闻#396 - 2021年3月10日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/396)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/rhxyooxeqhxygitungyv.jpg)
## [Citus 10发布：Postgres 12和13的分布式“超级大国”吗？](https://postgresweekly.com/link/104328/web)
Citus是长期存在的Postgres扩展（开源，但现在由Microsoft团队广泛开发），使Postgres更具分布式和水平可扩展性。v10最重要的是，它为Postgres引入了列式存储支持，以减少存储量并提高分析查询的性能。 


`Marco Slot (Microsoft) `
## [使用Python和Pandas在Postgres中构建推荐引擎](https://postgresweekly.com/link/104329/web)
了解如何直接在Postgres内部利用Python和Pandas（一种流行的数据分析工具）来构建自己的推荐引擎。


`Craig Kerstiens `
## [[网络研讨会]一切都失败了-如何挽救数据库灾难](https://postgresweekly.com/link/104331/web)
所有应用程序都失败了。这是不可避免的。在本演讲中，我们将介绍基于分布式系统基本原理的主动-主动，始终在线数据库的概念。


`Cockroach Labs `
## [迁移到Aurora：简单，除了账单？](https://postgresweekly.com/link/104332/web)
“将我们的生产数据库从Postgres迁移到Aurora很容易，直到我们注意到我们的每日数据库成本增加了一倍以上。” 幸运的是，尽管他们对这一举动似乎有些矛盾，但他们继续减轻了这一负担。


`Kimberly Nicholls `
## [Citus 10如何将柱状压缩带到Postgres](https://postgresweekly.com/link/104333/web)
我们已经提到了上面的Citus 10版本，但是新的柱状存储机制如何工作？这是对Postgres的相当新颖的补充，但是这篇文章很好地解释了包括利弊在内的事情。


`Jeff Davis (Microsoft) `
## [使用pg_notify了实时仪表盘](https://postgresweekly.com/link/104334/web)
现在，这可能是有用的。pg_notify是Postgres函数，可用于在Postgres客户端之间发送通知，以及触发器，NOTIFY和LISTEN命令可用于实时仪表板应用程序。 


`Daniel Lifflander `
## [适用于AWS RDS的Postgres主要版本升级和副本的最佳实践](https://postgresweekly.com/link/104336/web)
使用类似于AWS RDS提供的托管服务的好处之一是，升级也得到了一定程度的管理。但是仍然有一些事情要考虑，特别是在主要级别（例如12-> 13）升级中。


`Divya Sharma and Anisha Cherodian (AWS) `
## [沿堆栈其余部分可视化关键的Postgres度量标准](https://postgresweekly.com/link/104338/web)
收集OOTB和自定义的Postgres度量标准，并将它们与相关的跟踪和日志相关联。从今天开始免费试用。


`Datadog `
## [清理Postgres数据库](https://postgresweekly.com/link/104340/web)
Craig分享了一些有关如何提高Postgres数据库性能的可行步骤。


`Craig Kerstiens `
## [用全文搜索解决方案替换列搜索](https://postgresweekly.com/link/104342/web)
“磁盘很便宜。时间很贵。” 因此，如果您确实需要全文搜索的灵活性，请不要担心留出一定的存储空间以妥善处理它。这里也有一些有趣的查询示例。


`Dan Langille `
## [在哪里可以设置postgres配置参数？](https://postgresweekly.com/link/104344/web)
证明它不仅在中postgresql.conf。


`Hubert depesz Lubaczewski `
## [加快pgbench使用速度COPY FREEZE](https://postgresweekly.com/link/104346/web)
pgbench是Postgres随附的基准测试工具，由该文章的作者于1999年编写。在这里，他研究了由于即将推出的Postgres 14增强而为加快基准测试过程而进行的优化。


`Tatsuo Ishii `
## [pg_activity 2.1：-top类似Postgres活动监视工具](https://postgresweekly.com/link/104350/web)
与您可能top在服务器上监视进程和CPU使用情况一样，pg_activity它提供了一种类似的方法来检查PostgreSQL。建立在Python 3.6上。


`Dalibo `
## [Postgres服务器导出器：Prometheus的Postgres指标导出器](https://postgresweekly.com/link/104352/web)
l,null,"en


`Prometheus Monitoring Community `
# 💡本周提示


**🗓即将举办的Postgres活动**
