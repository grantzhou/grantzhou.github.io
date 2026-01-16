---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-9-5
---
### PostgreSQL每周新闻#614 - 2025年9月5日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/614)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/ae8g3cl11hcrttbzf870.jpg)
## [🗓️ pgcalendar：用于循环计划的“无限”日历功能](https://postgresweekly.com/link/173746/web)
如果您需要存储事件的计划，并且可能存在例外情况（例如假期或取消），此扩展程序提供了一种方法来模拟这些概念。示例。

`Huseyin Akbas`

## [分区表统计的怪癖](https://postgresweekly.com/link/173748/web)
Postgres 依靠分区表统计来估计连接行数，但自动清理不会收集它们，这意味着您需要明确运行 ANALYZE 才能获得好的计划。

`Laurenz Albe  `

## [安心监控 PostgreSQL](https://postgresweekly.com/link/173749/web)
Redgate Monitor 为您的 PostgreSQL 数据库提供实时洞察、智能警报和深度诊断。提前预防性能问题，保障系统平稳运行。探索 Redgate Monitor。

`Redgate `

### **本周摘要**

* ⭐ 就在我们即将点击“发送”按钮之际，[Postgres 18 候选版本 1](https://postgresweekly.com/link/173828/web) 终于发布了 :-) 趁着这个话题，Ahsan Hadi [回顾了 Postgres 18 的精彩内容](https://postgresweekly.com/link/173751/web)。

* 🇱🇻 [PostgreSQL 欧洲大会 2025 将于 10 月 21 日至 24 日在拉脱维亚里加](https://postgresweekly.com/link/173752/web)举行，[完整演讲日程](https://postgresweekly.com/link/173753/web)现已上线。

* 🎤 [PG Down Under](https://postgresweekly.com/link/173754/web) 是一个刚刚出现在我们关注范围内的 Postgres 播客。最新一期节目邀请了 RedGate 的 Grant Fritchey 讲述他在 pgNow 工具上的工作。

* PgDog Postgres 分片器/路由层新增了对[基于 Rust 的插件的支持](https://postgresweekly.com/link/173757/web)。


## [优化 Postgres 中的冷页面读取](https://postgresweekly.com/link/173458/web)
如果您的应用程序具有无法从缓存中受益的非传统访问模式，则有用的调整技巧。


`Tej Kashi`

📄 [Postgres 恢复中的隐藏瓶颈及其解决方案](https://postgresweekly.com/link/173759/web) Warda Bibi

📄 [Docker 中的 Postgres 自动备份：使用 pg_dump 的完整指南](https://postgresweekly.com/link/173760/web) Servers Inc. 

📄 [混合环境中 Postgres 安全最佳实践](https://postgresweekly.com/link/173761/web) Sebastian Insausti (Severalnines)

## [PostgreSQL 内部原理：简介](https://postgresweekly.com/link/173459/web)
如果您的应用程序具有无法从缓存中受益的非传统访问模式，则有用的调整技巧。


### **发布**


## [🌐 PostGIS 3.6.0 发布](https://postgresweekly.com/link/173762/web)
这个流行的扩展为 Postgres 添加强大的地理空间数据处理支持，现在针对 Postgres 18（目前为 RC1）。

`PostGIS PSC and OSGeo`

## [E-Maj 4.7：细粒度写入日志和时间旅行扩展](https://postgresweekly.com/link/173763/web)
该扩展可跟踪对表执行的更新，然后可用于对数据库的子集执行“时间旅行”。v4.7 带来了 Postgres 18 支持，包括对虚拟生成列的支持。（TIL E-Maj 代表“Enregistrement des Mises à Jour”，即“记录更新”。）

`Philippe Beaudoin`

## [pg_csv：灵活的 CSV 处理扩展](https://postgresweekly.com/link/173764/web)
旨在解决 COPY 的 CSV 支持的一些问题。

`PostgREST Team`

## [Jailer 16.9：数据库子集和关系数据浏览工具](https://postgresweekly.com/link/173765/web)
通过基于外键或用户定义的关系在数据库中进行双向导航。基于 Java 构建，并通过 JDBC 支持大多数关系数据库。

`Wisser`


[VectorChord 0.5.1](https://postgresweekly.com/link/173766/web) – Postgres 中可扩展、快速且磁盘友好的向量搜索。

[TimescaleDB 2.22](https://postgresweekly.com/link/173767/web) – Postgres 扩展中的时间序列功能。

[PostgREST 13.0.6](https://postgresweekly.com/link/173768/web) – 适用于任何 Postgres 数据库的 REST API。

[sqlc 1.30](https://postgresweekly.com/link/173769/web) – 从 SQL 生成类型安全的 Go 代码。