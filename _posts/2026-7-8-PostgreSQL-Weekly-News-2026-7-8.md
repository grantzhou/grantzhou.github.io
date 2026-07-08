---
layout: post
title: PostgreSQL 每周新闻 2026-7-8
---
### PostgreSQL每周新闻#656 - 2026年7月8日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/656)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/gh9d0pk0nfoal8f00czz.jpg)

## [Postgres is Enough：Postgres 如何替代其他系统](https://postgresweekly.com/link/187566/rss)

Postgres 世界中一个常青的话题是，搞清楚 Postgres 可以替代多少其他系统（比如 Redis、Elasticsearch 和 Kafka）。这个目录汇总了 89 个扩展和工具，帮助 Postgres 做到这一点。

`Goodway`


## [无需第二个系统的搜索](https://postgresweekly.com/link/187565/rss)

一个 Postgres 满足你的应用数据、全文搜索、向量检索和聚合需求。ParadeDB 是一个开源的 Postgres 扩展，性能可与 Elasticsearch 媲美。

`ParadeDB` **赞助商**


## [Postgres 事务是分布式系统的超能力](https://postgresweekly.com/link/187567/rss)

工作流状态应该存在于单独的编排器中，还是与数据一起存在于 Postgres 中？DBOS 主张后者：每个步骤的检查点和数据库更新在一个事务中提交，为这些更新提供精确一次语义，无需幂等性记账。

`Kraft and Li (DBOS)`

💡 [DBOSify](https://postgresweekly.com/link/187568/rss) 将上述理念付诸实践，作为 Temporal Python SDK 的直接替代品，使用 Postgres 而无需 Temporal 服务器。


## [PgDog 为何构建又一个 Postgres 连接池](https://postgresweekly.com/link/187569/rss)

主要是为了减少用户权衡并提供无缝体验。例如，与 PgBouncer 不同，它在事务模式下保持 `SET` 和 `LISTEN`/`NOTIFY` 正常工作。

`Lev Kokotov`


## [🚨 当前 Postgres 14-16 版本中的复制死锁 Bug](https://postgresweekly.com/link/187570/rss)

报告称 v14.23、v15.18 和 v16.14 引入了一个回归，在某些情况下可能导致事务日志重放期间的 `MultiXactOffsetSLRU` 死锁。

`Credativ`


## [等待 Postgres 20：添加后端级锁统计](https://postgresweekly.com/link/187571/rss)

Postgres 19 尚未发布，但 Hubert 已经在期待 v20 及其即将推出的每后端锁统计功能，该功能将显示哪些连接因锁而被阻塞，以及阻塞了多长时间。

`Hubert 'depesz' Lubaczewski`

📄 [理解 Postgres 19 属性图](https://postgresweekly.com/link/187572/rss) – 深入探讨将关系模式映射到[属性图](https://postgresweekly.com/link/187573/rss)，包括陷阱。*Rimas Silkaitis*

📄 [期待 Postgres 19：分裂个性](https://postgresweekly.com/link/187574/rss) – `ALTER TABLE` 正在获得 `SPLIT PARTITION` 和 `MERGE PARTITIONS` 选项。*Shaun Thomas*

📄 [将 Postgres 用作时序数据库](https://postgresweekly.com/link/187575/rss)  *Gulcin Yildirim Jelinek (Xata)*

📄 [关于 `random_page_cost` 的更多思考](https://postgresweekly.com/link/187576/rss)  *Tomas Vondra*


**发布和代码：**

## [pREST 2.0：从 Postgres 数据库提供 RESTful API](https://postgresweekly.com/link/187577/rss)

将 Postgres 数据库转换为 RESTful API。与 [PostgREST](https://postgresweekly.com/link/187578/rss) 功能类似，但用 Go 而非 Haskell 构建。v2.0 [添加了对多数据库的支持](https://postgresweekly.com/link/187579/rss)。

`pREST Team`


## [PL/Ruby 2.5：Ruby 作为 Postgres 的过程语言](https://postgresweekly.com/link/187580/rss)

允许你在 Ruby 中为 Postgres 编写函数、触发器、事件触发器和过程。

`Joshua D. Drake (Command Prompt Inc.)`


## [PL/CBMBASIC：用于 Postgres 的 Commodore 64 BASIC](https://postgresweekly.com/link/187581/rss)

我喜欢在每期中加入一个有趣的内容，用 44 年历史的编程语言编写 Postgres 函数……还能更有趣吗？😅

`Thom Brown`


## [Tinbase：单个二进制文件中的 Supabase 兼容后端](https://postgresweekly.com/link/187599/rss)

一个实验项目，提供本地 Supabase 类开发体验，无需 Docker，使用基于 [PGlite](https://postgresweekly.com/link/187583/rss) 和 [pg-mem](https://postgresweekly.com/link/187584/rss) 构建的纯 JS 后端。一种迷你的、仅限本地的 Postgres，包装在与 Supabase 相同的 API 中，因此 `supabase-js` 无需修改即可使用。

`Sanket Sahu`


## [pglayers：作为 Docker 层的 Postgres 扩展](https://postgresweekly.com/link/187585/rss)

官方 Postgres Docker 镜像附带的扩展很少，添加更多扩展可能会变得棘手。pglayers 试图通过在官方镜像之上分层扩展来简化这一过程。

`Ismaël Mejía`

- [pgcopydb 0.18](https://postgresweekly.com/link/187586/rss) – 将 Postgres 数据库复制到目标服务器（增强版的 `pg_dump | pg_restore`）。

- [PostGIS 3.7.0 Alpha 1](https://postgresweekly.com/link/187587/rss) – `ST_DWithin` 获得重大速度提升，放弃了对 Postgres 12/13 的支持，`address_standardizer` 和 `tiger_geocoder` 被拆分到各自的仓库。

- [River 0.40](https://postgresweekly.com/link/187588/rss) – 使用 Postgres 的 Go 作业处理系统。包含模式清理迁移并添加 `JobStuckHandler` 作为处理卡住作业的钩子。


## 📰 分类广告

📊 [适用于任何 Postgres 14+ 的开源可观测性](https://postgresweekly.com/link/187589/rss)。分层异常检测、历史指标。可选的自然语言聊天。

[Postgres 不再需要销售电话](https://postgresweekly.com/link/187590/rss)。选择你的产品，结账，并按自己的条件扩展。[无需等待报价](https://postgresweekly.com/link/187590/rss)。


## 🗓 即将举行的 Postgres 活动

- 🇲🇬 [PostgreSQL Madagascar Conference 2026（7月18日）](https://postgresweekly.com/link/187591/rss) — 第二届马达加斯加 Postgres 线下会议，演讲使用马达加斯加语、法语和英语。

- 🇬🇧 [PGDay UK 2026（9月8日在伦敦）](https://postgresweekly.com/link/187592/rss) — 第四届年度 PGDay UK，与 PGDay Lowlands 合作举办。

- 🇪🇺 [PGConf.EU 2026（10月20-23日在西班牙瓦伦西亚）](https://postgresweekly.com/link/187593/rss) — 欧洲最大的 Postgres 活动。

- 🇦🇺 [PG Down Under 2026（10月30日在悉尼）](https://postgresweekly.com/link/187594/rss) — 第六届面向澳大利亚和新西兰 Postgres 爱好者的年度会议。[征稿](https://postgresweekly.com/link/187595/rss)将于下周（7月15日）截止。

- 🇭🇰 [PGCONF.ASIA 2026（11月17-18日在香港）](https://postgresweekly.com/link/187596/rss) — 亚洲领先的会议。征稿目前开放中。

- 🇵🇱 [PGConf.PL 2026（11月24日在格但斯克）](https://postgresweekly.com/link/187597/rss) — 波兰和中欧首届 PostgreSQL 会议。

*注：此列表并非详尽无遗，我们将继续提及和推广其他活动。*