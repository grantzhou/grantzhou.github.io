---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-3-13
---
### PostgreSQL每周新闻#591 - 2025年3月13日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/592)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/ba1jmrccnqs6j7qcmuxk.jpg)
## [Citus 中的 1 万亿行？](https://postgresweekly.com/link/166811/web)
“Postgres 可扩展”，但到底能达到多大程度？Hans-Jürgen 决定一探究竟，他进行了一个小实验（或者说大实验？），看看是否可以实现 1 万亿行的表。

`Hans-Jürgen Schönig`

## [❌ 在 Postgres 中取消查询的方法](https://postgresweekly.com/link/166812/web)
如果您有一个或两个查询占用了 Postgres 的资源，那么终止它们是一种选择，并且有几种方法可以解决它。


`Petr Kada`
## [▶ 不要让 Postgres 维护出现漏洞](https://postgresweekly.com/link/166810/web)
确保您能够学习主动维护实践，以便在隐藏的数据库性能风险（如慢速查询、检查点行为和连接问题）升级之前发现它们。


`pganalyze `

### 本周摘要：

* 🤔 微软的 Postgres 团队回顾了他们[在 2024 年取得的成就](https://postgresweekly.com/link/166813/web)。如果你想知道他们的团队里都有谁以及他们做什么，这是一个很好的介绍。

* 🗣️ 经过几个月的休整，PostgreSQL 本周人物访谈又回来了，[Doug Ortiz](https://postgresweekly.com/link/166814/web) 为本周人物。

* 🎤 EDB 的 Jeremy Kellway 在 Stack Overflow 播客上解释了 [Postgres 如何非常适合 AI 用例](https://postgresweekly.com/link/166815/web)。

* ⛓️‍💥 Neon Postgres 平台已经实现了一个[“中断模拟器”](https://postgresweekly.com/link/166816/web)来演示其“即时恢复”功能。

* 🇨🇦 如果您想在 [2025 年蒙特利尔 Postgres 扩展日](https://postgresweekly.com/link/166817/web)上发言，其演讲者征集截止日期为 4 月 1 日。


## [Postgres 获得自连接消除优化](https://postgresweekly.com/link/166818/web)
几年前，有人提出了一种连接优化，即在某些条件下可以删除冗余的内部自连接（通常由 ORM 添加）。这种所谓的自连接消除 (SJE) 优化现已提交给 Postgres，并在 GitHub 提交中进行了说明。


`Postgres Repo`

* 📄 [等待 Postgres 18：允许并行创建 GIN 索引](https://postgresweekly.com/link/166820/web) Hubert depesz Lubaczewski

* 📄 [等待 Postgres 18：允许 json{b}_strip_nulls 删除空数组元素](https://postgresweekly.com/link/166821/web) Hubert depesz Lubaczewski

* 📄 [当 HASH 分区比 RANGE 效果更好时](https://postgresweekly.com/link/166822/web) Umair Shahid

### 代码和工具：

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/lxbnd2wqyl7rdcsqp0sq.jpg)

## [介绍 pgNow：一种时间点诊断工具](https://postgresweekly.com/link/166543/web)
Redgate 创建的免费（但不开放 - 预览版在电子邮件墙后面）跨平台桌面工具，用于突出显示和分析有关查询、索引、配置设置和 Postgres 集群操作的其他重要元素的实时数据。即使您没有使用它，Ryan 也会在此处全面概述它提供的功能。

`Ryan Booz`


[PGSync 4.0](https://postgresweekly.com/link/166824/web) – 用于将数据从 Postgres 同步到 Elasticsearch 或 OpenSearch 的中间件。

[📊 PEV2 v1.14](https://postgresweekly.com/link/166825/web) – 用于可视化 Postgres 执行计划的 Vue 组件。

[DoltgreSQL 0.18](https://postgresweekly.com/link/166826/web) – 具有 Git 风格功能的版本控制 Postgres 类。

[pgenv 1.4](https://postgresweekly.com/link/166827/web) – Postgres 二进制管理器。