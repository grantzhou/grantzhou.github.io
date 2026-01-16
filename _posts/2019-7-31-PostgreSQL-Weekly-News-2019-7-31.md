---
layout: post
title: PostgreSQL 每周新闻 2019-7-31
---

### PostgreSQL每周新闻#316 - 2019年7月31日

![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/316)

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/avzmg0sjxhowqtx5i0em.jpg)

## [介绍Postgres的并行](https://www.percona.com/blog/2019/07/30/parallelism-in-postgresql/)

介绍了新版本Postgres的并行机制，包括并行顺序扫描、并行聚合和并行B-tree索引扫描和他们加速数据扫描的原理。

`IBRAR AHMED`

## [Postgres的组合索引和独立索引](https://www.cybertec-postgresql.com/en/combined-indexes-vs-separate-indexes-in-postgresql/)

在设计数据库关系时，会遇到一个常见的问题，组合索引和单个索引哪一个更有意义。HANS-JÜRGEN研究了Postgres中的一些场景。

`HANS-JÜRGEN SCHÖNIG`

## [Postgres的sharding](https://www.percona.com/blog/2019/05/24/an-overview-of-sharding-in-postgresql-and-how-it-relates-to-mongodbs/?utm_source=cooperpress&utm_medium=advertisement&utm_campaign=GLQ319COOPERPRESSDG&utm_term=postgresql&utm_content=postgresql-weekly)

学习Postgres的新功能，现在可以完成简单的数据sharding

`PERCONA`**赞助商**

## [Postgres系数据库AWS Aurora](https://www.percona.com/blog/2019/07/16/brin-index-for-postgresql-dont-forget-the-benefits/)

Amazon Aurora提升了Postgres的兼容性，这具体指什么，它是如何使用的，它的限制是什么。Viorel Tabara带你了解所有的这一切。

`SEVERALNINES`



## [在DNA上跑SQL是数据库的下一个发展方向么？](https://www.zdnet.com/article/forget-silicon-sql-on-dna-is-the-next-frontier-for-databases/)

欧盟正在研究一些未来的新兴技术，其中一项是在合成DNA中存储数据。这是一项及其昂贵的研究，它已经有了可喜的进展，而且有人已经准备为这项研究做学术报告。这是一个值得关注的领域。

`GEORGE ANADIOTIS (ZDNET)`



## [jsquery和SQL/JSON在json查询的对比](https://thombrown.blogspot.com/2019/07/jsquery-vs-sqljson.html)

Postgres12将提供对SQL/JSON的本地支持，并将提供一种标准化的方法来查询存储在Postgres JSONB列中的JSON数据。另一方面，JSQuery在Postgres9.4以后的扩展中提供了类似的查询语言。本文对这两种方式进行比较。

`THOM BROWN`



## [你的数据就是你的生命](https://pgexperts.com)

PGX提供完整的PostgreSQL支持，从应急服务到日常运营支持，再到战略规划。我们是为你的数据操作而来的。

`POSTGRESQL EXPERTS, INC`**赞助商**



## [Postgres和Apache Spark大数据](https://severalnines.com/blog/big-data-postgresql-and-apache-spark)

Spark是一个非常流行的开源大数据分析引擎，如果你对这个不是很了解，那么这篇文章通过Postgres带你深入了解它。

`SEBASTIAN INSAUSTI`



## [使用约束排除提升查询性能](https://www.timescale.com/blog/implementing-constraint-exclusion-for-faster-query-performance/)

看 Timescale（PostgreSQL的时间序列集中扩展）如何利用PostgreSQL的基础，并扩展其性能以提高性能。

`SVEN KLEMM`



## [pglogical 2.2.2发布](https://www.postgresql.org/about/news/1956/)

PGLogical是一种基于扩展的逻辑复制系统，它是物理复制的有效替代方案。

`2NDQUADRANT`



# 💡本周提示

###### 一个定制NULL值排序规则的方法

由[Jonathan Reinink](https://postgresweekly.com/link/67572/web)在[Twitter](https://postgresweekly.com/link/67573/web)提供支持



PostgreSQL中我最喜欢的一个小特性是NULL值的排序（NULL值放在开始或者末尾）。只需在方向（asc/desc）后添加nulls last或nulls first。

![image](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/v1564400143/bp6nlnrmv40c2h4uke4c.png)

这允许你随意定义NULL值在排序结果中的位置。



本周提示由[Datadog](https://postgresweekly.com/link/67571/web)赞助。使用datadog在一个地方监控Postgres数据库、云服务、Web服务器、容器和servlet。[Try it free](https://postgresweekly.com/link/67571/web)



🗓  **即将举办的Postgres活动**  

• [PGConf.Brasil 2019](https://www.pgconf.com.br/2019/en/)(8月1-3日，圣保罗)——为期三天的会议，包括讲座，教程，课程和闪电讲座。

• [PGDay Austria 2019](https://pgday.at/en/)（9月6日， 维纳·纽斯塔特，奥地利）

• [PostgreSQL Conference Asia 2019](https://2019.pgconf.asia/)（9月8-11日，巴厘岛，印度尼西亚）

• [PostgresConf South Africa 2019](https://postgresconf.org/conferences/SouthAfrica2019)（10月8-9日，约翰内斯堡）——提供给使用Postgres的数据库管理和开发人员互相了解的机会。

