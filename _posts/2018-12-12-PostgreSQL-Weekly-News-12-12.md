---
layout: post
title: PostgreSQL 每周新闻 2018-12-12
---

### PostgreSQL每周新闻 #285 - 2018年12月12日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
![_config.yml](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/vwffcnrvp1sqpwocqman.jpg)

备注：[英文原文地址](https://postgresweekly.com/issues/285)

## [如何零停机时间将Postgres 10升级到11](https://severalnines.com/blog/how-upgrade-postgresql10-postgresql11-zero-downtime)
在PostgreSQL上完成升级的旧方法是使用pg_upgrade，转储和恢复，或使用一些第三方工具，但逻辑复制现在开启了一个相当轻松的零停机时间方法。

`SEBASTIAN INSAUSTI`

## [如何使用Postgres上的GraphQL订阅构建实时应用程序](https://www.smashingmagazine.com/2018/12/real-time-app-graphql-subscriptions-postgres/)
使用Postgres，GraphQL和React构建实时轮询应用程序，没有特定的后端代码（它使用在Heroku上运行的Hasura的GraphQL服务-全部免费）。

`SANDIP DEVARKONDA`

## [使用Telegraf和InfluxDB监控PostgreSQL数据库](https://www.influxdata.com/blog/monitoring-your-postgresql-database-with-telegraf-and-influxdb/)
![INFLUXDATA](https://copm.s3.amazonaws.com/8c2dd309.jpg)
了解如何使用InfluxDB监控Postgres，这是一个发展最快的时间序列数据库，专为指标和事件而构建。

`INFLUXDATA` *赞助商*

## [使用分区保持Postgres整洁](https://blog.dataegret.com/2018/12/keeping-postgres-tidy-with-partitioning.html)
“如果你怀疑分区是否是这个例子的有用工具，我希望你不会再怀疑了。”

`ALEXEY LESOVSKY`

## [Postgres实际如何工作？](https://www.youtube.com/watch?v=zkEhX0yOL3k)
已经有一年了，但不知怎的，我们错过了Postgres核心团队成员的这个简洁的谈话，他们以一种非常容易理解的方式深入探讨了很多Postgres技术（特别是关于查询解析和规划）。

`PETER EISENTRAUT`

## [Amazon RDS支持将Postgres日志发布到Amazon CloudWatch日志](https://aws.amazon.com/cn/about-aws/whats-new/2018/12/amazon-rds-supports-postgresql-logfiles-publish-to-amazon-cloudwatch-logs/)

`AMAZON WEB SERVICES, INC.`

## [如何在macOS上本地测试Postgres](https://www.peterbe.com/plog/how-i-performance-test-postgresql-locally-on-macos)
Mozilla工程师分享如何使用pghero和Docker在本地测试PG

`PETER BENGTSSON`

## [PREPARE TRANSACTION及其危险](https://www.cybertec-postgresql.com/en/prepared-transactions/)
你几乎肯定不需要使用PREPARE TRANSACTION，除非你正在建立一个事务管理器，但如果你很好奇...

`LAURENZ ALBE`

## [在会话中分配work_mem](https://momjian.us/main/blogs/pgblog/2018.html#December_10_2018)
work_mem允许你在内存中执行更大的排序，如果你有内存，它将胜过基于磁盘的等价物。

`BRUCE MOMJIAN`

## [评估TimescaleDB和Postgres的高可用性解决方案](https://blog.timescale.com/high-availability-timescaledb-postgresql-patroni-a4572264a831)
“我们如何评估几种第三方工具，并最终选择Patroni作为我们的首选方法。”

`LEE HAMPTON`

## [数据库与加密](https://blog.2ndquadrant.com/databases-vs-encryption/)
将加密分离为单独的可信组件的方法，该组件作为自定义数据类型实现，与更常见的全盘加密或使用pgcrypto相比，它具有一些优势。

`TOMAS VONDRA`

## [阅读我们对PostgreSQL 11中新功能的看法](https://severalnines.com/blog/whats-new-postgresql-11?utm_campaign=Momentum_Campaign_DEC_2018&utm_content=pgweekly&utm_medium=Paid_Search&utm_source=banner)
Somenines为PostgreSQL数据库提供部署，监控和管理

`SEVERALNINES` *赞助商*

## [Orafce：Postgres的Oracle兼容功能](https://github.com/orafce/orafce)
Orafce实现了Oracle数据库中的一些功能，这些功能可能对迁移到Postgres的用户有用。 上周发布的新版本增加了对Postgres 11的支持。

`ORAFCE`

# 活动
## [FOSDEM PGDay 2019](https://2019.fosdempgday.org/)
2019年2月1日(布鲁塞尔，比利时)

FOSDEM常规PostgreSQL活动的扩展

## [PostgreSQL Conference Europe](https://2019.pgconf.eu/)
2019年10月15日至18日(米兰，意大利)

第十一届PostgreSQL欧洲年会，一天的讲师指导培训，随后三天的世界级PostgreSQL演讲和一流的交流平台。
