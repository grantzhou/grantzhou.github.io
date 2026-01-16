---
layout: post
title: PostgreSQL 每周新闻 2019-4-3
---

### PostgreSQL每周新闻#299 - 2019年4月3日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/299)

![pg_img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/ssoylsgxn7il7w6zynuj.jpg)

## [Postgres支持“生成字段（Generated Column）”](https://github.com/postgres/postgres/commit/fc22b6623b6b3bab3cb057ccd282c2bfad1a0b30)
很高兴看到Postgres对SQL标准功能的支持，此提交以一个简单示例开始，该示例说明一种类型的生成字段（Generated Column）将来如何工作。MySQL 5.7引入了[类似的功能](https://gabi.dev/2016/10/17/understanding-generated-columns/)，SQL Server称它们为[计算列(Computed Column)](https://docs.microsoft.com/en-us/sql/relational-databases/tables/specify-computed-columns-in-a-table?view=sql-server-2017)。

`PETER EISENTRAUT`

## [使用pg_dump / pg_restore升级Postgres](https://www.percona.com/blog/2019/03/27/postgresql-upgrade-using-pg_dump-pg_restore/)
上次介绍了[使用pg_dumpall升级Postgres](https://www.percona.com/blog/2019/03/18/postgresql-upgrade-using-pg_dumpall/)，本次介绍使用pg_dump和pg_restore升级Postgres。

`JOBIN AUGUSTINE, VALLARAPU, ET AL.`

## [在PostgreSQL数据库中监视的度量标准](https://www.influxdata.com/blog/metrics-to-monitor-in-your-postgresql-database/?utm_campaign=postgres&utm_medium=newsletter&utm_source=cooperpress)
![img](https://copm.s3.amazonaws.com/2e860b79.jpg)  
在数据库性能方面，您需要跟踪几个关键指标，它们并非都是特定于数据库的。

`INFLUXDATA` **数据库**

## [2019年PostgreSQL趋势报告](https://scalegrid.io/blog/2019-postgresql-trends-report-private-vs-public-cloud-migrations-database-combinations-top-reasons-used/)
一位多云DBaaS提供商在上个月的PostgresConf上对用户进行了调查，并在此处分享了结果。 AWS作为托管Postgres的最受欢迎的云平台，成本是选择Postgres的最大理由。

`SCALEGRID`

## [等待PostgreSQL 12：REINDEX CONCURRENTLY](https://www.depesz.com/2019/03/29/waiting-for-postgresql-12-reindex-concurrently/)
在Postgres 12中，REINDEX命令（从表的当前数据重建索引）有一个选项，让它在后台构建索引并在完成时将其开启。

`HUBERT DEPESZ LUBACZEWSKI`

## [使用适用于Azure上的PostgreSQL的TimescaleDB驱动物联网和时间序列工作负载](https://azure.microsoft.com/en-gb/blog/power-iot-and-time-series-workloads-with-timescaledb-for-azure-database-for-postgresql/)
与Timescale建立新的合作伙伴关系，在Azure上为客户构建的物联网和时间序列工作负载引入了对TimescaleDB（专注于时间序列支持的Postgres扩展）的支持。

`SUNIL KAMATH (MICROSOFT)`

## [我们如何将大规模并行Postgres数据库迁移到Kubernetes上](http://engineering.pivotal.io/post/how_we_moved_a_massively_parallel_postgres_database_onto_kubernetes/)

`OZ BASARIR (PIVOTAL)`

## [Pgpool-II 4.1中的语句级负载平衡](http://pgsqlpgpool.blogspot.com/2019/04/statement-level-load-balancing.html)

`PGPOOL`

## [思考MapReduce,但是使用SQL](https://www.citusdata.com/blog/2019/02/21/thinking-in-mapreduce-but-with-sql/?utm_source=PG_Weekly&utm_medium=email&utm_campaign=sponsor_blog)
了解如何使用MapReduce方法来并行化SQL数据库，就像我们使用Citus和Postgres一样。

`CITUS DATA, NOW PART OF THE MICROSOFT FAMILY` **赞助商**

## [与diff类似但是适用于Postgres Schema](https://github.com/djrobstep/migra)
用Python编写，可以从您自己的Python脚本或命令行使用。

`ROBERT LECHTE`

## [ActiveRecordExtended 1.0：为Ruby的Active Record添加额外的Postgres功能](https://github.com/georgekaraszi/ActiveRecordExtended)
 Active Record，作为Ruby on Rails应用程序中常用的与数据库交互，自然是与数据库无关的，但Postgres有许多额外的查询功能，不能使用它们是一种耻辱。这个gem添加了诸如数组和JSON查询，CTE和联合之类的东西。

`GEORGE PROTACIO-KARASZI`

## [repmgr 4.3发布](https://www.2ndquadrant.com/en/about/news/announcing-release-repmgr-43/)
repmgr是一种流行的复制和故障转移管理工具，此版本中包括一些可用性改进。

`2NDQUADRANT`

🗓  即将举办的Postgres活动  

   * [pgconf.de 2019 (5月10日,莱比锡)](https://2019.pgconf.de/) —— 最成功的德语PostgreSQL会议。  
   * [PGDay.IT 2019 (5月16日,博洛尼亚)](https://2019.pgday.it/en/)  
   * [PGCon 2019(5月28日,渥太华)](https://www.pgcon.org/2019/) —— 供用户和开发人员见面和讨论Postgres的年度会议
   * [Postgres Vision 2019(6月24日,波士顿)](https://postgresvision.com/)  
