---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2022-5-4
---
### PostgreSQL每周新闻#453 - 2022年5月4日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/453)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/lljednvtgyp6bvwqzpyw.jpg)
## [看看（未来）并行服务器端备份压缩](https://postgresweekly.com/link/122999/web)
Postgres 15 将支持服务器端备份压缩，Robert 做了一些研究以了解它的工作情况（在速度和节省的磁盘空间方面） ) 使用不同的压缩算法。很有前途！


`Robert Haas `
## [Postgres 中的 IO：过去、现在和未来](https://postgresweekly.com/link/123000/web)
▶两天前的一次技术演讲，深入探讨了 Postgres 的 IO 故事，包括当前的限制、如何解决这些限制以及在改进方面取得的进展。（1 小时 6 分钟。）


`Andres Freund `
## [你的分布式数据库真的兼容 PostgreSQL 吗？](https://postgresweekly.com/link/123001/web)
您如何评价云原生数据库的 PostgreSQL 兼容性？该视频提供了一个框架来比较现代数据库的 PostgreSQL 兼容性，包括 Google Spanner、Amazon Aurora、CockroachDB 和 YugabyteDB


`YugabyteDB `
## [使用大型 Postgres 数据库](https://postgresweekly.com/link/123002/web)
当 Postgres 可以处理无限大小（尽管表限制为 32TB）时，什么是小型、中型或大型数据库？Robert 说，通过预测未来情况来解决“大型”数据库的潜在问题是每个 DBA 的目标。


`Robert Bernier `
## [Apache AGE 1.0：Postgres的图表扩展](https://postgresweekly.com/link/123003/web)
为 Postgres 提供图形数据库功能（通过 openCypher）的扩展，其灵感来自 AgensGraph。有关发布的更多信息。


`Apache Foundation `
## [使用MobilityDB分析历史飞行数据](https://postgresweekly.com/link/123007/web)
MobilityDB 位于 Postgres 和 PostGIS 之上，用于提供地理空间轨迹分析。所以它非常适合分析历史空中交通数据，如此处所示。


`Florian Nadler `
## [MERGE在 Postgres 15 中使用 SQL](https://postgresweekly.com/link/123009/web)
上个月，我们提到Postgres 15 即将支持MERGE ，这篇文章展示了它的基本使用示例。


`Hans-Jürgen Schönig `
## [高级Postgres模式设计](https://postgresweekly.com/link/123011/web)
▶PGConf NYC 2021 上关于“超越功能索引、排除约束、数组类型、事务 DDL 等CREATE TABLE”的演讲。CREATE VIEW


`Sehrope Sarkuni `
## [在 Amazon RDS 或 Aurora 上自动化间隔分区维护](https://postgresweekly.com/link/123012/web)
非常特定于 AWS，但这里有很多将想法结合在一起来创建强大的分区数据库


`Shetty, Gudivada, et al. (AWS) `
## [调整 Auto-Vacuuming 参数](https://postgresweekly.com/link/123013/web)
也许是 Postgres 最常被提及的话题。


`Michael Aboagye `
## [PGWatch2 v1.9 发布](https://postgresweekly.com/link/123015/web)
pgwatch2是一个 Postgres 监控系统，使用 Grafana 仪表板来可视化各种 Postgres 指标。


`Pavlo Golub `
## [自定义仪表板、管理面板、CRUD 应用程序](https://postgresweekly.com/link/123017/web)
l,null,"en


`Retool `
## [pg_ivm 1.0：IVM（增量视图维护）扩展](https://postgresweekly.com/link/123018/web)
增量视图维护（IVM）以计算和应用增量更改而不是重新计算所有内容的方式使物化视图保持最新。pg_ivm 提供了一种“即时维护”，其中物化视图在基表被修改后立即更新。


`SRA OSS, Inc. Japan `
# 💡本周提示


**🗓即将举办的Postgres活动**
