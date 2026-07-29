---
layout: post
title: PostgreSQL 每周新闻 2026-7-29
---
### PostgreSQL每周新闻#659 - 2026年7月29日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/659)

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/eukyepveiob0ilfmq5nq.jpg)

## [PGSimCity：3D 方式探索 Postgres 工作原理](https://postgresweekly.com/link/188575/rss)

一种真正新颖的方式来探索 Postgres 内部的模型。这不仅仅是一个可视化工具，你可以四处游走并且*破坏东西*！它有点"繁忙"，用户体验不够完美（在移动设备上可能会遇到困难），但为一些原本不透明的技术概念提供了全新的视角。

`Nikolay Samokhvalov`


## [Postgres 19 中的三个新特性](https://postgresweekly.com/link/188576/rss)

PlanetScale 对即将发布的版本进行了反思，重点关注 `REPACK`、默认关闭 `JIT` 以及查询规划器的改进。

`Ahmed Darwich`


## [无需第二个系统的搜索](https://postgresweekly.com/link/188574/rss)

一个 Postgres 即可满足您的应用数据、全文搜索、向量检索和聚合需求。ParadeDB 是一个开源的 Postgres 扩展，性能可与 Elasticsearch 媲美。

`ParadeDB` **赞助商**


## [Postgres 19 即将推出的 Autovacuum 调整](https://postgresweekly.com/link/188577/rss)

Autovacuum 一直以目录顺序处理表，但 Postgres 19 教会它进行分类，根据回卷风险和死元组等因素对表进行评分，因此最需要处理的情况会优先得到处理。

`Shaun Thomas (pgEdge)`


## [Postgres 的 MVCC 很糟糕，但其他人的也一样](https://postgresweekly.com/link/188578/rss)

Andy Pavlo 的数据库团队称 MVCC 是[他们最讨厌的 Postgres 部分](https://postgresweekly.com/link/188579/rss)，Radim 对此表示赞同，并提供了基准测试。但随后他提出了问题：Oracle、InnoDB、SQL Server、MongoDB 和 etcd 做了什么，代价是什么？

`Radim Marek`

💡 不过，并非所有人都被说服。在[这条 Hacker News 评论](https://postgresweekly.com/link/188580/rss)中，Skeema 作者 Evan Elias 对 InnoDB 的描述提出了反驳。


## [创业公司的 Postgres 生存指南](https://postgresweekly.com/link/188581/rss)

一家创业公司公开了其内部指南，提炼了两年的 Postgres 战斗经验，从模式规则和复合索引到 autovacuum 调优、`SKIP LOCKED` 队列和分区。

`Alexander Belanger (Hatchet)`


## [为第三方 DBA 提供数据库访问权限的正确方式](https://postgresweekly.com/link/188582/rss)

从创建范围限定的角色的基础知识，到为监控提供安全访问、能够取消失控的查询，甚至进行 vacuum 和重新索引，而无需交出所有权或超级用户访问权限。

`Shridhar Khanal (Stormatics)`


## [为什么你的开创性 Postgres 功能应该从分支开始](https://postgresweekly.com/link/188583/rss)

一位 Postgres 规划器贡献者讲述了他在临时表上并行扫描的三次尝试，被本地缓冲区和会弄脏页面的只读查询所阻碍。他说，分支是证明它的地方，因为核心的"门槛很高"。

`Andrei Lepikhov`

📄 [让我们破坏 Autovacuum：重现故障以使其可观察](https://postgresweekly.com/link/188584/rss) `Nikolay Sivko (Coroot)`


**分类广告：**

💻 [从 Cursor、VS Code 或 Claude Desktop 连接 Postgres 的 MCP](https://postgresweekly.com/link/188585/rss)。默认只读，范围权限，令牌高效。

[MyDBA](https://postgresweekly.com/link/188594/rss)：为您的 Postgres 数据库提供全面监控。免费开始为期一周的健康检查，然后继续免费监控。


## 🛠 代码和工具

## [Pagila 4：Postgres 示例数据库](https://postgresweekly.com/link/188587/rss)

最初是 MySQL 的 [Sakila](https://postgresweekly.com/link/188588/rss) 示例数据库的移植版本，Pagila 已扩展以支持众多 Postgres 特定功能（如 SQL/JSON 和 UUIDv7），v4.0（需要 Postgres 18）规模更大，数据集更多样化。

`Devrim Gündüz`


## [pgGraph 1.0：为 Postgres 添加图数据库"超能力"](https://postgresweekly.com/link/188589/rss)

一个扩展，可直接对普通表运行图搜索、遍历、最短路径和关系查询。

`Evokoa`


## [Rainfrog 0.4：Postgres 的数据库管理 TUI](https://postgresweekly.com/link/188595/rss)

比 `psql` 更结构化一些，具有 vim 风格的查询、历史、模式等导航。v0.4 添加了查询自动完成功能。

`Carl Liu`

- [Postgres Operator 2.0](https://postgresweekly.com/link/188590/rss) – Zalando 的 operator，用于在 Kubernetes 上运行高可用性 Postgres 集群。

- [pg_partman 5.5](https://postgresweekly.com/link/188592/rss) – 分区管理扩展。包括多个 CVE 的修复。

- [pREST 2.4](https://postgresweekly.com/link/188591/rss) – 基于 Go 的 Postgres 数据库 RESTful 服务器。