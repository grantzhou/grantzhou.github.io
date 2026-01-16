---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2021-10-6
---
### PostgreSQL每周新闻#425 - 2021年10月6日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/425)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/uap9deydp0do77p0ewus.jpg)
## [🎂 PostgreSQL 14 发布](https://postgresweekly.com/link/114590/web)
距离 Postgres 13 的最终版本仅一年多，下一个主要版本就在这里。 与 13 一样，14 是您可以称之为“进化”版本的版本，没有巨大的新功能（都是关于小事的），而是一长串增强功能和成熟度。 这些包括：
* 能够更轻松地为用户分配表、视图和模式的只读或只写权限。
* 逻辑复制改进。
* 更好的范围类型。
* 改进了查询并行性支持并改进了并行顺序扫描性能。
* 减少索引膨胀。
* 一些 JSON 改进。
* 每列可配置压缩。
* 存储过程现在可以使用 OUT 参数返回数据。


`PostgreSQL Global Development Group `
## [CYBERTEC Migrator 第 3 版现已推出](https://postgresweekly.com/link/114599/web)
我们重建了 GUI 以进一步简化数据库迁移：利用四个简单的阶段指导您完成迁移过程，控制功能有助于重新运行阶段或中止。 您现在可以使用新的日志视图探索迁移的内部工作原理。


`CYBERTEC `
## [Timescale Cloud：用于时间序列工作负载的新的基于 Postgres 的云数据库服务](https://postgresweekly.com/link/114600/web)
Postgres 继续其通过 Timescale 的新产品及其开源时间序列数据库扩展 TimescaleDB Postgres 变体来主导云数据库场景的道路。 这篇发布文章深入探讨了为什么他们认为这是一个引人注目的提议，并鼓励您免费试用。


`Mike Freedman (Timescale) `
## [Azure 如何在Postgres 14发布后一天内发布](https://postgresweekly.com/link/114602/web)
如果您认为升级 Postgres 安装很困难，那么考虑云提供商如何升级整个平台可能会令人难以置信。 微软很自豪在发布后的 24 小时内开始了这个过程，虽然这篇文章没有详细介绍它，但很好地了解了他们如何看待它以及他们如何让 Citus 参与其中。


`Ozgun Erdogan (Microsoft) `
## [使用 Postgres 自动递增的三种方法](https://postgresweekly.com/link/114603/web)
作者着眼于以各种方式重叠的序列、SERIAL 数据类型和标识列。


`Laetitia Avrot `
## [Kubernetes 上的 PostgreSQL 14（附示例）](https://postgresweekly.com/link/114604/web)
Crunchy Data 已经向 PGO（Kubernetes 的开源 Postgres Operator）推出了他们自己独特的 Postgres 14 体验。


`Jonathan S. Katz `
## [从 Postgres 9.6 升级到 Postgres 13](https://postgresweekly.com/link/114605/web)
在您担心升级到 Postgres 14 之前，也许摆脱像 9.6 这样的旧版本是一个更大的问题。 五年前发布的 Postgres 9.6 从 2021 年 11 月起正式处于“生命尽头”。


`Avinash Vallarapu `
## [像查询 Postgres 一样查询 MongoDB - 使用 SQL 使用 Studio 3T](https://postgresweekly.com/link/114606/web)


`Studio 3T `
## [ÖBB（奥地利铁路公司）如何迁移到 Azure 上的 Postgres](https://postgresweekly.com/link/114607/web)
奥地利国家铁路系统如何从基于 Oracle 的本地系统迁移到 Azure Database for PostgreSQL 的案例研究。


`Microsoft `
## [Postgres 还是“少年”？](https://postgresweekly.com/link/114608/web)
在意识到 Postgres 14 的全部内容之前，作者试图找到一个焦点。没有一个焦点，它更多地是关于一个较小但可靠的增强列表。


`Kirk Roybal `
## [为什么关系数据库是标准而不是基于图形的数据库？](https://postgresweekly.com/link/114609/web)
不是 Postgres 特有的，但这个问题在本周 Hacker News 上引发了一些有趣的评论，争论一直追溯到 70 年代。


`Hacker News `
