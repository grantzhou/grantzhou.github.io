---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2021-9-22
---
### PostgreSQL每周新闻#423 - 2021年9月22日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/423)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/firsue8ggtdc2jitz45a.jpg)
## [百分比近似的工作原理（以及为什么它比平均值更有用）](https://postgresweekly.com/link/113932/web)
分解平均值与百分比的基础知识，并通过真实场景（API 监控）展示依赖大型时间序列数据集平均值的“危险”。 最后看看百分比在 Postgres 中是如何工作的。


`David Kohn (Timescale) `
## [Postgres 14：一些小事情](https://postgresweekly.com/link/113933/web)
Postgres 14 即将推出，但虽然许多版本都有 Craig 所说的“大支柱”或主要功能，但版本 14 更像是一个小但并非不重要的改进的集合，Craig 选择了一个 这里有几个他最喜欢的。


`Craig Kerstiens `

## [Postgres 14 中的逻辑复制改进](http://amitkapila16.blogspot.com/2021/09/logical-replication-improvements-in.html)

`Amit Kapila `

## [Pggnalyze Index Advisor：理想的Postgres索引建议](https://postgresweekly.com/link/113935/web)
我们的免费索引顾问根据您的数据库架构和统计数据以及您的查询工作负载以及每次表扫描的其他见解提供索引建议。 如果要使用推荐的理想索引，只需复制 CREATE INDEX 命令。


`pganalyze `
## [Postgres 调度器的比较表](https://postgresweekly.com/link/113936/web)
pg_timetable 的开发者之一，Postgres 的调度扩展，自称为“调度器瘾君子”，给出了 pg_timetable、pg_cron、pgAgent、jpgAgent 和 pgbucket 的快速比较。


`Pavlo Golub `
## [Citus 10.2 对 Postgres 扩展的新功能](https://postgresweekly.com/link/113938/web)
来自 Microsoft 流行的开源 Postgres 水平扩展系统的最新消息。 它现在“支持 Postgres 14”，简化了分区维护，并改进了对列表索引的支持。


`Onder Kalaci (Citus Data) `
## [Amazon RDS 现在支持用于 Postgres 数据库的 X2g 实例](https://postgresweekly.com/link/113939/web)
X2g 实例是基于 Gravton2 的大量内存实例，起始容量为 32GB，如果您有钱，可以使用高达 1TB 的 RAM。


`Amazon Web Services `
## [如何自动化 Amazon Aurora PostgreSQL 的基准测试](https://postgresweekly.com/link/113940/web)
解释如何为 AWS Aurora 上的 Postgres 数据库设置自动化但实际的基准测试系统。


`Andrew Love (AWS) `
## [处理 Linux 升级后损坏的索引](https://postgresweekly.com/link/113941/web)
升级运行 Postgres 集群的操作系统并涉及 glibc 库版本更新，或将数据库迁移到运行另一个操作系统（和 glibc）版本的另一台机器会带来鲜为人知但非常显着的风险...


`Michał Mackiewicz `
## [如何使用 pglogical 和数据库迁移服务 (DMS) 升级 Postgres](https://postgresweekly.com/link/113942/web)
即使您尚未使用 Google 的 Cloud SQL 服务，您仍然可以使用他们的数据库迁移服务来帮助升级。


`Shubha Rajan (Google Cloud) `
## [实时识别慢速 PostgreSQL 查询并优化性能](https://postgresweekly.com/link/113943/web)


`Datadog `
## [将 JPA 应用程序从 Oracle 迁移到 Postgres](https://postgresweekly.com/link/113944/web)
Java Persistence API (JPA) 本质上是一组使用关系数据库来存储 Java 对象的标准。


`Tim Zöller `

# 工具和代码

## [pglog：灵活且简单的日志分析器](https://postgresweekly.com/link/113945/web)
如果您使用大量数据库并希望通过分析日志（在本地，而不是在生产中）快速解决任何问题，pglog 是您需要的拓展。


`Lætitia Avrot `
## [node-pg-migrate 6.0：节点支持的 Postgres 数据库迁移管理](https://postgresweekly.com/link/113947/web)


`Salsita Software `
## [ErrorPush：兼容 Rollbar 客户端的极简错误收集服务](https://postgresweekly.com/link/113946/web)
一个开源的错误收集服务，将日志存储在单个 Postgres 表中。 用 Python 编写。


`Haukur Rósinkranz `

