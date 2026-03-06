---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2021-3-31
---
### PostgreSQL每周新闻#399 - 2021年3月31日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/399)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/nve3nh9rfpzmx2xmipvm.jpg)
## [Postgres Optimizer如何工作并加快查询速度](https://postgresweekly.com/link/105452/web)
上周，我们看到了如何使用EXPLAIN分析查询并查看执行计划者的决定是什么，但是这篇文章深入探讨了后面进行的优化过程。


`Hans-Jürgen Schönig `
## [在Postgres 14中加快恢复和VACUUM的速度](https://postgresweekly.com/link/105454/web)
Postgres 14目前还未发布，但是许多开发人员正在为此而努力实现新功能，包括David Rowley一直在对crash recovery性能进行重大改进。 在这里，他解释了它是如何工作的。


`David Rowley `
## [🌍CYBERTEC空间服务🌎您的数据库GIS准备好了吗？](https://postgresweekly.com/link/105455/web)
使用易于理解的地图和仪表板显示庞大的数据集，并从地理角度分析数据。 我们可以帮助您实施空间基础架构，GIS培训和数据库优化以及空间分析。


`CYBERTEC `
## [用UNION加快SQL查询的效率](https://postgresweekly.com/link/105456/web)
SQL的UNION操作通常不被认为是优化查询性能的一种方法，但是在许多情况下，它可以用来大幅提高速度。


`Ben Levy and Christian Charukiewicz `
## [何时使用表空间](https://postgresweekly.com/link/105457/web)
表空间本质上是文件系统中可以存储代表数据库对象的数据的位置，它们使定义不同的位置来存储不同的数据库，索引和其他对象。


`Laurenz Albe `
## [迁移到Amazon RDS和Amazon Aurora数据库的Graviton2（ARM）的关键注意事项](https://postgresweekly.com/link/105458/web)
开发了自己基于ARM的芯片，这些芯片可保证以较低的价格提供更高的性能，AWS非常希望将您的数据库工作负载转移给他们- 这里提到他们对用户采取的流程的期望。


`Reagan Rosario and Tyler Lynch (AWS) `
## [如何加快Postgres查询的最佳实践。 免费电子书](https://postgresweekly.com/link/105459/web)
我们分享了帮助Atlassian，CounterPath等公司加快查询速度的经验教训。


`pganalyze `
## [探索PL / Python：将Postgres表数据转换为NumPy数组](https://postgresweekly.com/link/105460/web)


`Kat Batuigas `
## [使用Raku的Postgres](https://postgresweekly.com/link/105461/web)
Raku是最初称为Perl 6的语言。


### 🔧工具和代码

`Luca Ferrari `
## [首先看一下pg_repack](https://postgresweekly.com/link/105462/web)
pg_repack是一个扩展，用于从表和索引中删除膨胀，但在处理过程中不对它们进行排他锁定。


`Luca Ferrari `
## [pg_timetable 3.7.0：Postgres的高级作业调度](https://postgresweekly.com/link/105464/web)


`CYBERTEC PostgreSQL International GmbH `
## [pgAdmin 5.1：流行的Postgres Admin仪表板](https://postgresweekly.com/link/105465/web)
您现在可以在界面内更轻松地放大和缩小。


`pgAdmin Development Team `
## [pg_auto_failover 1.5：自动故障转移和高可用性扩展](https://postgresweekly.com/link/105466/web)
监视和管理Postgres集群的自动故障转移。


`Citus Data `