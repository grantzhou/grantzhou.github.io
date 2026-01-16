---
layout: post
title: PostgreSQL 每周新闻 2023-11-22
---
### PostgreSQL每周新闻#531 - 2023年11月22日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/531)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/bfifhr47blxnrnlk1orh.jpg)
## [探索 Postgres 查询计划](https://postgresweekly.com/link/148037/web)
Phil 通过研究如何拦截查询执行过程以及通过这样做可以学到什么，继续深入探讨 Postgres 工作原理的技术细节。 诚然，大多数 Postgres 用户永远不需要深入研究，但如果您想至少了解一下幕后发生的事情，那么值得浏览一下。


`Phil Eaton `
## [通过增量物化视图提高查询性能！](https://postgresweekly.com/link/148036/web)
通过将 Epsio 插入数据库来提高最复杂查询的性能。 每当基础数据发生变化时，Epsio 就会不断为您定义的查询准备和更新结果，而无需重新计算整个数据集。


`Epsio `

**本周摘要：**
*   AWS RDS for PostgreSQL 现在支持 Postgres 16.1。 Postgres 16 也在 Azure Database for PostgreSQL 上正式发布。


*   📗 Luca Ferrari 和 Enrico Pirozzi 推出了由 Packt 出版的《学习 PostgreSQL》一书的第二版。


*   Bruce Momjian 回顾了 2021 年的一个邮件列表主题，该主题思考 SQL 是否是一件好事。 毫不奇怪的剧透：Bruce 喜欢 SQL。


## [为多租户设计数据库](https://postgresweekly.com/link/148038/web)
Craig 深入研究了多租户应用程序、分片以及 Citus 扩展在管理此类情况方面可以发挥的作用。 他提供了几种数据设计方法，以便您在时机成熟时更好地做好扩展准备。


`Craig Kerstiens (Crunchy Data) `
## [在 s390x（即 IBM 大型机）上运行 Postgres](https://postgresweekly.com/link/148044/web)
Postgres 正在获得对一种不太新的架构的支持，这种架构采用 IBM Z 系列大型机架构，在 Debian 中称为 s390x。 Marist College 的 LinuxOne 云提供了构建机器。


`Christoph Berg `
## [如何在 Heroku 上使用 pgvector 进行相似性搜索](https://postgresweekly.com/link/148045/web)
Heroku Postgres 几周前宣布支持 pgvector，这里是强制性的“如何使用它”帖子。


`Valerie Woolard (Heroku) `
## [在 Postgres 中体验 WAL REDO](https://postgresweekly.com/link/148047/web)
从技术角度了解添加一条自定义信息作为 XLOG 记录以供在 WAL REDO 期间使用所涉及的步骤。


`David Zhang `
## [PostgreSQL 101 网络研讨会：数据库监控和优化](https://postgresweekly.com/link/148048/web)


`Redgate`
## [使用 citus_stat_activity 进行 Citus 实时查询检查](https://postgresweekly.com/link/148049/web)
如何使用 citus_stat_activity 一次性获取有关分片的所有信息。


`Hans-Jürgen Schönig `
## [Postgres 新技巧：SIMD 向量化以实现更快的分析查询](https://postgresweekly.com/link/148050/web)


`JAMES BLACKWOOD-SEWELL (TIMESCALE)`
## [在具有两个可读备用服务器的 Amazon RDS 多可用区部署上使用 PgBouncer 进行快速切换](https://postgresweekly.com/link/148051/web)


`KHODORKOVSKIY AND JAIN (AWS)`
## [River：用于 Go 和 Postgres 的快速、稳健的作业队列](https://postgresweekly.com/link/148052/web)
一个新的测试版开源作业队列，“用于构建快速、密封的应用程序”，用 Go 编写。 它使用 pgx 与 Postgres 交互。


`Brandur Leach `
## [pgcopydb：将 Postgres 数据库复制到目标 Postgres 服务器](https://postgresweekly.com/link/148054/web)
自动化并提供围绕 pg_dump 运行的一些结构 | 两个正在运行的 Postgres 服务器之间的 pg_restore。


`Dimitri Fontaine `
## [PGSync 3.0：Postgres 到 Elasticsearch 同步工具](https://postgresweekly.com/link/148055/web)
用于将 Postgres 同步到 Elasticsearch 的中间件，以便您可以在 Elasticsearch 中公开非规范化文档以进行查询。 现在麻省理工学院获得许可。


`Tolu Aina `
## [PostGIS 补丁版本](https://postgresweekly.com/link/148056/web)
即 3.4.1、3.3.5、3.2.6、3.1.10 和 3.0.10。

## [Orafce 4.7](https://postgresweekly.com/link/148057/web)
适用于 Postgres 的 Oracle 数据库兼容性函数和包。

## [pg-mem 2.7.2](https://postgresweekly.com/link/148058/web)
内存中模拟 Postgres，用于 JavaScript 中的单元测试。

## [Pgpool-II 4.5 Beta 1](https://postgresweekly.com/link/148059/web)
连接池和平衡。