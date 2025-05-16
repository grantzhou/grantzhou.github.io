---
layout: post
title: PostgreSQL 每周新闻 2025-5-15
---
### PostgreSQL每周新闻#600 - 2025年5月15日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/600)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/dfj5uleaimiufr8dpzej.jpg)
## [PostgREST 13：Postgres 数据库的 RESTful API](https://postgresweekly.com/link/169390/web)
一个独立的 Web 服务器，可将您的 Postgres 数据库直接转换为 RESTful HTTP API。v13.0 增加了对扩展对多对多关系和自动 tsvector 转换的支持，允许开箱即用地在文本和 json 类型上使用 fts。

`Joe Nelson and Steve Chavez`

## [Postgres 18 Beta 已发布：您应该了解的 7 个功能](https://postgresweekly.com/link/169392/web)
上周的重大新闻是 Postgres 18 Beta 1 的发布。Neon 简要总结了需要注意的七个功能。


`Heikki Linnakangas (Neon)`
## [POSETTE 2025：记住日期！](https://postgresweekly.com/link/169389/web)
POSETTE：Postgres 活动，一场免费的线上开发者盛会，距离 6 月 10 日至 12 日不到一个月了。向 45 位 PostgreSQL 生态系统的专家学习。42 场精彩演讲，4 个直播，Discord 实时聊天，任您选择。记住日期！

`Microsoft`

### **本周摘要**

* [Neon](https://postgresweekly.com/link/169394/web) 无服务器 Postgres 平台宣布已被 [Databricks 收购](https://postgresweekly.com/link/169395/web)。不过，短期内用户使用体验不会有任何改变。

* 其他 Postgres 平台新闻：[Xata 即将“重新发布”](https://postgresweekly.com/link/169396/web)，成为一项专注于云扩展的全新 Postgres 服务，该服务拥有即时写时复制分支和数据匿名化功能。

* 🎤 [Postgres FM](https://postgresweekly.com/link/169397/web) 播客的最新一期探讨了 [▶️ 十大 Postgres 相关危险问题](https://postgresweekly.com/link/169398/web)。

* 📱 [Schema](https://postgresweekly.com/link/169399/web) 是一款适用于 iOS 的全新 Postgres 和 MySQL 数据库客户端。我觉得在手机上操作数据库会比较费劲，但它的设计确实很棒。

🇩🇪 PGConf.DE 上周在柏林举行，有[几篇](https://postgresweekly.com/link/169400/web)游记[报道了那里的情况](https://postgresweekly.com/link/169401/web)。

📄 [十秒内搞定 Postgres 的求和类型](https://postgresweekly.com/link/169418/web) Evan Silberman

📄 [无需超级用户权限即可实现事件触发器——这与 Supabase 的 Supautils 扩展相关。](https://postgresweekly.com/link/169402/web) Steve Chavez

📄 [从 CockroachDB 迁移到 Postgres 的故事](https://postgresweekly.com/link/169404/web) Sean Callahan

📄 [在 Azure Database for PostgreSQL 灵活服务器上使用 pgstattuple 管理数据库膨胀](https://postgresweekly.com/link/169405/web) Gayathri Paderla (Microsoft)

📄 [如何在 Ubuntu 25.04 上将 Postgres 16 升级到 17](https://postgresweekly.com/link/169406/web) Paolo Melchiorre

📄 [法学硕士 (LLM) 如何通过自然语言革新数据库查询](https://postgresweekly.com/link/169407/web) Joe Harwood (QueryHub)

### **代码和工具**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/sixqwtolv7o1l6qnjdq5.jpg)

## [pgModeler 1.2：Postgres 数据库建模工具](https://postgresweekly.com/link/169408/web) — 一种以更直观的方式轻松创建和编辑数据库模型的方法。它已打包为付费产品，但也是开源的（GPLv3 - 代码库在此），因此您可以自行构建。v1.2 是一个重要更新。

`Raphael Araújo e Silva`

## [pgwatch 3.3：Postgres 监控解决方案](https://postgresweekly.com/link/169084/web) – 一个独立的 Postgres 服务器指标监控仪表板工具。可以轻松通过 Docker 进行非侵入式部署（无需扩展）。GitHub 仓库。

`CYBERTEC`

## [Vircadia：一个由 Postgres 提供支持的游戏反应层](https://postgresweekly.com/link/169413/web) – 这似乎还处于早期阶段，但其想法是您可以使用 Vircadia 来模拟代理世界并通过 SQL 管理游戏内实体。

`Vircadia`

## [FerretDB 2.2](https://postgresweekly.com/link/169414/web) – 一款功能类似于 MongoDB 的数据库，但使用 Postgres 进行存储。（顺便提一句，FerretDB 的联合创始人最近与 Claire Giordano 一起参加了 Talking Postgres 播客，探讨了 FerretDB 以及他们为何选择 Postgres 作为后端。）

## [River 0.22](https://postgresweekly.com/link/169416/web) – 适用于 Go 和 Postgres 的强大作业处理系统。

## [pgroll 0.12](https://postgresweekly.com/link/169417/web) – 零停机、可逆、模式迁移。