---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2023-7-19
---
### PostgreSQL每周新闻#515 - 2023年7月19日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/515)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/pdiatnvihasxcycz1zme.jpg)
## [Citus 12：Postgres 基于Schema的分片](https://postgresweekly.com/link/142723/web)
Citus 多年来一直在做“分布式 Postgres”的事情，但这是一个引入基于schema分片的巨大版本。 基于schema的分片与 Citus 最初的基于行的分片方法形成鲜明对比，它允许您以更广泛的方式进行分片 - 仅举一个例子，这对于多租户 SaaS 应用程序尤其方便。


`Citus Data `
## [使用 Epsio 的增量物化视图即时获得复杂查询的结果](https://postgresweekly.com/link/142722/web)
通过将 Epsio 集成到现有数据库中，将查询延迟和工作负载成本降低几个数量级。


`Epsio `
## [不再有vacuum了吗？ 不再数据膨胀了吗？](https://postgresweekly.com/link/142725/web)
OrioleDB 是一个大胆的扩展，有着大胆的目标，包括最终成为 Postgres 核心的一部分。 它是 Postgres 的替代引擎，可以消除数据膨胀和持续清理表的需要。 这篇文章很好地解释了它是什么、它是如何工作的以及为什么你可以使用它，但请记住它仍然处于实验阶段。


`Oriole DB Inc. `
## [在 Postgres 中使用时间序列](https://postgresweekly.com/link/142726/web)
当然，您可以使用 TimescaleDB 等，但对于适度的用例，Postgres 很可能已经具备了对数据进行临时切片和切块所需的功能。

`Alex Plescan `
**本周摘要：**
*   📅pgday UK是一项新活动，由Postgresql Europe将于9月12日在伦敦，英国举行😁


*   亚马逊奥罗拉（Amazon Aurora）增加了对Postgres 15.3、14.8、13.11、12.15 和 11.20 的支持。它还增加了对PGVECTOR的支持。


*   Supabase 尝试了 pgvector 0.4 的基准测试。


*   Bytebase 尝试比较 Postgres 和 MySQL。


*   Heroku 通过重新支持向公共架构添加扩展来尝试改善他们的 Postgres 扩展体验。


*   📅 2023 年 PASS 数据社区峰会日程现已公布。 通常以 SQL Server 为重点的活动正在扩展，今年 Postgres 的演讲数量惊人。


## [🎧 Citus Con 之路：Postgres podcast](https://postgresweekly.com/link/142734/web)
来自 Microsoft Citus Data 团队的podcast，旨在展示其受欢迎的 Citus Con 活动的演讲者，但现在，它更像是一个通用的 Postgres podcast。 ▶️ 最新一集由 Grant Fritchey 和 Ryan Booz 谈论他们最喜欢的了解 Postgres 的方法。
```
Postgres.fm 也仍然是一场精彩的表演。 他们的最新一集介绍了 PgBouncer 和 PgCat 等连接池。
```

`Citus Data `
## [Instacart 的零停机 Postgres 切换](https://postgresweekly.com/link/142738/web)
解释 Instacart 如何在不停机的情况下保持其庞大的 RDS Postgres 服务器保持最新状态。。


`Nicholson, Tanner, and Montagna (Instacart) `
## [如何创建和运行 Postgres 回归和 TAP 测试](https://postgresweekly.com/link/142739/web)
适合直接在 Postgres 上工作的人员。


`Tristen Raab `
## [Ora2Pg 24.0：不再仅适用于 Oracle](https://postgresweekly.com/link/142740/web)
Ora2Pg 是一个长期存在的工具，用于协助 Oracle 数据库到 Postgres 迁移，但它现在也增加了对从 SQL Server 迁移的支持。


`Gilles Darold `
## [云 PostgreSQL 的开源替代方案。 即可免费开始并获得 300 美元积分](https://postgresweekly.com/link/142742/web)


`EDB BIGANIMAL`
## [pg_cirrus Beta 1：简单的 Postgres 集群设置](https://postgresweekly.com/link/142743/web)
将 Python 和 Ansible 简单地结合在一起，用于设置一个主节点和两个备用节点的三节点集群，并通过此处的基本说明完成流复制和负载平衡。


`Stormatics `
## [PostgREST v11.1 中有哪些新增功能？](https://postgresweekly.com/link/142745/web)
PostgREST 是一个 Haskell 应用程序，可从任何现有的 Postgres 数据库提供 RESTful API。 它不需要 Supabase，但这是类 Supabase 的方案 。


`Steve Chavez (Supabase) `
## [FerretDB 1.6](https://postgresweekly.com/link/142747/web)
↳感觉就像 MongoDB，位于 Postgres 之上。


## [Credcheck 2.1](https://postgresweekly.com/link/142748/web)
↳ 验证 Postgres 用户凭据。


## [PGSpider 3.1.0](https://postgresweekly.com/link/142749/web)
↳ 东芝用于分布式大数据的 SQL 集群引擎。


## [PostGIS 3.4.0 Beta 1](https://postgresweekly.com/link/142750/web)


## [pgmanage 1.0b2](https://postgresweekly.com/link/142751/web)
