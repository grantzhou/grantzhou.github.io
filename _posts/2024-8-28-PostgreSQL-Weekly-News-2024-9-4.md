---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-9-4
---
### PostgreSQL每周新闻#568 - 2024年9月4日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/568)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/wymc982loxcwpkjvzxv1.jpg)
## [Postgres 17 中的三大功能](https://postgresweekly.com/link/158955/web)
随着我们继续最终接近 Postgres 17（可能于本月晚些时候推出），Neon 反思了对 MERGE 的改进、改进的 JSON 函数和性能改进。EDB 也列出了[自己的 Postgres 17 增强功能列表](https://postgresweekly.com/link/159300/web)，其中[增量备份支持](https://postgresweekly.com/link/159301/web)位居榜首。

`Anastasia Lubennikova (Neon) `

💡 说到 Postgres 17，[Postgres 17 的候选版本 1](https://postgresweekly.com/link/159302/web) 似乎将于本周发布。尚未公布，但请关注。

## [掌握 PostgreSQL 扩展：Pgvector、Citus、TimescaleDB](https://postgresweekly.com/link/159298/web)
通过我们由专家主导的 Pgvector、Citus 和 TimescaleDB 网络研讨会系列释放 PostgreSQL 的全部潜力。了解集成、扩展和最佳实践，以优化数据库性能。立即观看以提升您的 PostgreSQL 技能！


`Percona `
## [2024 年 PostgreSQL 状态问卷调查现已开放](https://postgresweekly.com/link/159303/web)
Timescale 广受欢迎的年度社区调查再次开放。您可以在[此处](https://postgresweekly.com/link/159304/web)参加，截止日期为 9 月 30 日星期一。如果您现在急需一些统计数据，可以在[此处](https://postgresweekly.com/link/159305/web)查看 2023 年调查的结果。


`Timescale  `

### 本周摘要：

* MongoDB 的首席执行官声称，[MongoDB 在业务工作负载方面取得了一些“胜利”，甚至超过了 Postgres](https://postgresweekly.com/link/159306/web)。他还提出了其他主张，包括 MongoDB“更有利于提高开发人员的工作效率”。

* [EDB 的 Amul Sul](https://postgresweekly.com/link/159307/web) 是本周 PostgreSQL 人物的受访者。

* 📊 Redgate 正在进行 [2024 年数据库格局问卷调查](https://postgresweekly.com/link/159308/web)。

* 🇦🇹 Xata 将于 9 月 18 日参加维也纳的欧洲开源峰会，并希望在那里与您讨论 Postgres 的所有事宜。他们还将举办 [Postgres“欢乐时光”](https://postgresweekly.com/link/159309/web)，即使那些没有参加峰会的人也可以参加。

* 📄 [如何在 Kubernetes 中测试 PostgreSQL Commitfest 补丁](https://postgresweekly.com/link/159310/web) - Gabriele Bartolini

* 📄 [VACUUM：管理和检测膨胀](https://postgresweekly.com/link/159311/web) - Hans-Jürgen Schönig

### 🛠 代码和工具

[pg_stat_monitor 2.1：查询性能监控工具](https://postgresweekly.com/link/158975/web) 
与 pg_stat_statements 类似，但有望成为“更高级的替代品”。一个特别巧妙的功能是按时间对统计数据进行分组，从而可以更精细地使用收集的数据。[GitHub 存储库](https://postgresweekly.com/link/159313/web)。


`Percona`
## [Pigsty v3.0：一款扩展功能丰富的 Postgres 发行版](https://postgresweekly.com/link/159314/web)
Pigsty 是一款 Postgres 发行版，承诺“功能齐全”。它提供了一个类似 RDS 的平台，但可以根据您的需要进行部署。现在，它还允许您轻松安装 336 个其他扩展。


`Ruohang Feng`
## [pg_hint_plan 1.7：使用“提示”调整查询执行计划](https://postgresweekly.com/link/159314/web)
Postgres 的查询规划器通常能够很好地找出如何最好地针对您的数据执行查询，但是当它需要在正确的方向上稍微推动一下时，这可以让您放弃一些提示。在 v1.7 中，添加了对 Postgres 17 的支持。


`NTT OSS Center DBMS Development and Support Team`

📰 分类广告
索引拖累了你？报名参加 Redgate 9 月 10 日的网络研讨会 [PostgreSQL 101：索引](https://postgresweekly.com/link/159318/web)，了解技巧、窍门和最佳实践。

[Blacksmith](https://postgresweekly.com/link/159319/web) 只需更改一行代码，即可将 GitHub Actions 的运行速度提高 2 倍，成本降低一半。受到 Ashby 和 Slope 等 100 多家公司的信赖。

## [PgCat 1.2：现代 Postgres 池和代理](https://postgresweekly.com/link/159320/web)
基于 Rust 构建，PgCat 提供分片支持（包括基于 SQL 语法的实验性分片）、负载平衡和故障转移支持。


`PostgresML`
## [pg_easy_replicate 现在支持逻辑复制期间的架构更改跟踪](https://postgresweekly.com/link/159321/web)
pg_easy_replicate 可以轻松设置逻辑复制并在主数据库服务器之间执行最少的停机时间切换。它现在还支持 DDL 更改跟踪。


`Shayon Mukherjee`


[Patroni 4.0](https://postgresweekly.com/link/159323/web) – PostgreSQL HA 的流行模板。

[FerretDB 1.24](https://postgresweekly.com/link/159324/web) – 一个类似于 MongoDB 的数据库，但使用 Postgres 进行存储。

[PgParty 1.8](https://postgresweekly.com/link/159325/web) – 使用 Ruby 从 Active Record 创建 Postgres 分区。

[DBeaver 24.2](https://postgresweekly.com/link/159326/web) – 跨平台数据库 GUI 工具和 SQL 客户端。

[pg_failover_slots 1.1](https://postgresweekly.com/link/159327/web)