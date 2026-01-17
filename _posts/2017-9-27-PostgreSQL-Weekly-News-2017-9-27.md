---
layout: post
title: PostgreSQL 每周新闻 2017-9-27
categories: [PostgreSQL]
tags: [PGWeekly]
---
### PostgreSQL每周新闻#226 - 2017年9月27日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/226)

## [PostgreSQL 的哈希索引现在变酷了](http://rhaas.blogspot.co.uk/2017/09/postgresqls-hash-indexes-are-now-cool.html)
在 Postgres 10 之前，哈希索引存在严重缺陷，但正如 Robert 在这里解释的那样，情况正在迅速好转。

`Robert Haas`

## [PostgreSQL 10 RC1 发布](https://www.postgresql.org/about/news/1783/)
版本 10 的第一个候选版本现已可供下载。

`PostgreSQL.org`

## [pglogical 2.0 - 来自 2ndQuadrant 的下一代逻辑复制](https://www.2ndquadrant.com/en/resources/pglogical/)
![](https://copm.s3.amazonaws.com/5016eca7.jpg)

pglogical 是一个完全作为 PostgreSQL 扩展实现的逻辑复制系统。完全集成，不需要触发器或外部程序。使用这种物理复制的替代方案复制您的数据并实现零停机。

`2ndQuadrant PostgreSQL Products` **赞助商**

## ["我在 Postgres 中达到 1600 列限制的那一天"](https://rosenfeld.herokuapp.com/en/articles/programming/2017-09-26-the-day-i-reached-the-1600-columns-limit-in-postgresql)
Postgres 在删除列时不会回收空间，这在创建和删除许多临时列的情况下可能会成为问题。一个有趣的故事。

`Rodrigo Rosenfeld Rosas`

## [Postgres 10 的新特性](https://wiki.postgresql.org/wiki/New_in_postgres_10)
即将发布的 Postgres 主要新版本中的变更清单。

`PostgreSQL Wiki`

## [使用 pgTAP 框架对 Postgres 进行单元测试](https://medium.com/engineering-on-the-incline/unit-testing-postgres-with-pgtap-af09ec42795)

`Simon McClive`

## [从单节点 Postgres 迁移到 Citus](https://www.citusdata.com/blog/2017/09/20/migrating-from-single-node-postgres-to-citus/)
迁移到 Citus 需要遵循的一些步骤。

`Craig Kerstiens`

## [使用 PostGIS、GeoServer 和 Google Earth 创建多维分级统计图](https://medium.com/@aliasmrchips/multi-dimensional-choropleth-maps-using-postgis-geoserver-and-google-earth-557a03608c99)

`Mark Mathis`

## [驯服 Postgres 自动清理](https://developer.s24.com/blog/taming-postgresql-autovacuum.html)
在调优自动清理时，"从默认设置开始，并定期检查表膨胀"。

`Torsten Bøgh Köster`

## [Postgres 中的事务暂存作业排空](https://brandur.org/job-drain)
构建一个强大的后台工作系统，利用事务隔离确保永远不会过早处理作业，并利用事务持久性确保永远不会丢失作业。

`Brandur Leach`

## [跨越 PostgreSQL 鸿沟](https://www.commandprompt.com/blog/postgres%20chasm/)
"我认为 PostgreSQL 整体上缺少的是有效的沟通和外展活动，以吸引和引导新用户和开发人员。"

`Debbie Cerda`

## [使用 SelectStar 深入了解您的 Postgres 数据库](https://selectstar.io/blog/postgresql-selectstar-database-performance-platform/)
开始免费试用，了解高级查询如何帮助优化性能。

`SelectStar` **赞助商**

## [Podyn：DynamoDB 到 Postgres 的复制和迁移工具](https://www.citusdata.com/blog/2017/09/22/dynamodb-to-postgres-replication/)

`Marco Slot`