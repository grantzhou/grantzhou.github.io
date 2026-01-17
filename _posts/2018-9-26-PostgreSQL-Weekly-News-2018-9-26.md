---
layout: post
title: PostgreSQL 每周新闻 2018-9-26
categories: [PostgreSQL]
tags: [PGWeekly]
---
### PostgreSQL每周新闻#275 - 2018年9月26日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/275)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/jdpx2najknvtqjchjawm.jpg)

## [在 EC2 上运行 Postgres？您的时钟可能正在拖慢速度](https://heapanalytics.com/blog/engineering/clocksource-aws-ec2-vdso)
一个有趣的故事：一家公司发现运行其 Postgres 集群的 EC2 实例在获取时间时特别慢，这对其 Postgres 分析工作负载产生了性能影响。有趣的是，Heap 的一位工程师还解释了[为什么他们使用 EC2 而不是 RDS](https://news.ycombinator.com/item?id=18043439) 来运行 Postgres。

`Kamal Marhubi (Heap)`

## [PostgreSQL 11 Beta 4 发布](https://www.postgresql.org/about/news/1890/)
您可能已经注意到我们链接了很多关于 Postgres 11 的精彩内容（本期也不例外），随着最新 beta 版的发布，它离最终发布又近了一步。如果您正在进行基准测试，请注意 JIT 编译现在默认禁用，必须显式开启。

`PostgreSQL Global Development Group`

## [Postgres-XL：可横向扩展的 PostgreSQL](https://www.2ndquadrant.com/en/resources/postgres-xl/?utm_source=cp&utm_medium=pgweekly&utm_campaign=xlcppgweekly)
Postgres-XL 是一个大规模并行处理数据库 - 与 PostgreSQL 高度兼容，可横向扩展。它支持商业智能工作负载和在同一平台上的高容量事务写入和读取工作负载。

`2ndQuadrant PostgreSQL Products` **赞助商**

## [PostGIS 2.5.0 发布：PostgreSQL 的空间和地理对象](http://postgis.net/2018/09/23/postgis-2.5.0/)
眼尖的读者会注意到所有 2.5 beta 版本都针对 Postgres 11，虽然 PostGIS 2.5 最适合 Postgres 11，但它也可以在 Postgres 9.4 及更高版本上运行。

`PostGIS Developers`

## [优化 Postgres 列顺序](https://blog.2ndquadrant.com/on-rocks-and-sand/)
深入探讨了一些底层调整，您可以通过内存高效的方式对列进行排序。

`2ndQuadrant`

## [Postgres 11：人人都有收获](https://lwn.net/Articles/764515/)
对 Postgres 11 即将推出的一些新功能的高层次解释 - 我们在过去几个月里大多数都在这里提到过。我们自己的 Craig Kerstiens [也对可用功能进行了初步了解](http://www.craigkerstiens.com/2018/09/20/postgresql-11-a-first-look/)。

`Peter Geoghegan`

## [Amazon Aurora 现在支持停止和启动数据库集群](https://aws.amazon.com/about-aws/whats-new/2018/09/amazon-aurora-stop-and-start/)
Aurora（有 Postgres 兼容版本）集群现在可以停止（最多 7 天）和重新启动，使其对于开发和测试目的更有用且更实惠。

`Amazon Web Services`

## [公告：EDB Postgres 迁移门户 Beta 版](https://www.bit.ly/2QqsNxd)

`EnterpriseDB` **赞助商**

## [如何在 SQL 中编写乘法聚合函数](https://blog.jooq.org/2018/09/21/how-to-write-a-multiplication-aggregate-function-in-sql/)

`Lukas Eder`

## [将 Postgres 作为企业级环境进行安全保护](https://www.percona.com/blog/2018/09/21/securing-postgresql-as-an-enterprise-grade-environment/)
一篇简短的文章，介绍了几个可以提高安全性的 Postgres 功能。

`Avinash Vallarapu`

## [关于行为准则争议的思考](http://ledgersmbdev.blogspot.com/2018/09/thoughts-on-code-of-conduct-controversy.html)
对 PostgreSQL 社区需要[其最近发布的"行为准则"](https://lwn.net/Articles/765332/)的反思，以及应该采取什么流程来达到正确的平衡。

`Chris Travers`

## [pg_terminator：清理会话和查询的工具](https://www.depesz.com/2018/09/25/pg_terminator-released/)
配置后，它可以根据各种规则取消/终止查询和连接。[Git 仓库](https://gitlab.com/depesz/pg_terminator)。

`Hubert depesz Lubaczewski`

## 🗓 活动

## [PostgresConf South Africa 2018](https://postgresconf.org/conferences/SouthAfrica2018)
**10月9-10日（南非约翰内斯堡）** 为数据库管理和开发社区提供交流思想和了解当前功能及即将到来趋势的机会。

## [2Q PGConf 2018](http://www.2qpgconf.com/)
**12月4-5日（芝加哥）** 一个致力于交流 PostgreSQL 知识的会议。

## [PGCONF.ASIA 2018](https://www.pgconf.asia/EN/2018/)
**12月10-12日（日本东京）** PGConf.ASIA 2018 是 PostgreSQL 的国际会议。来参加这个在亚洲举办的最大 PostgreSQL 会议之一。

## [FOSDEM PGDay 2019](https://2019.fosdempgday.org/)
**2019年2月1日（比利时布鲁塞尔）** FOSDEM 常规 PostgreSQL 活动的延伸。