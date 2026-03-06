---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-12-4
---
### PostgreSQL每周新闻#626 - 2025年12月4日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/627)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/rgnw8r0j0wkkom96fzut.jpg)
## [关于Postgres中JSON资料的高效储存](https://postgresweekly.com/link/177987/web)
JSON与JSONB作为资料类型，pglz与lz4作为压缩演算法…哪一种组合能以最有效率的方式储存JSON资料？ Hubert进行了一些调查，以了解不同组合在查询速度和储存空间方面的效能表现。

`Hubert depesz Lubaczewski`


## [POSETTE 2026：征稿启事 (CFP) 现已开放！](https://postgresweekly.com/link/177986/web)
[POSETTE：Postgres](https://postgresweekly.com/link/177988/web)，是由微软 Postgres 团队组织的免费线上开发者活动，将于 6 月 16 日至 18 日举行。征稿启事 (CFP) 开放至 2 月 1 日。欢迎新旧演讲者踊跃投稿！了解更多详情。

`Microsoft `


## **本周摘要**

* [Postgres.app](https://postgresweekly.com/link/177989/web) 是一款受欢迎且便利的工具，可在 macOS 上快速执行 Postgres 实例。它最近新增了几个常用扩充功能（PL/v8、http、pg_parquet 和 TimescaleDB）的[下载功能，方便使用者快速安装](https://postgresweekly.com/link/177990/web)。

* [AWS 为其各种产品（包括 RDS 和 Aurora）推出了新的资料库节省计划](https://postgresweekly.com/link/177991/web)，该计划将使那些能够在一年内按小时支付固定费用的用户受益。

* [Schema3D](https://postgresweekly.com/link/177992/web) 是一种有趣的实验性工具，可用于在 3D 空间中视觉化资料库模式。 （使用右上角的铅笔图示输入您自己的 SQL 语句。）


## [透明资料加密 (TDE) 现已支援 Postgres 18](https://postgresweekly.com/link/177993/web)
Percona 现在发布了一个 Postgres 18.1 版本，该版本完全支援原生 TDE 和非同步 I/O。 TDE 提供档案层级的加密，解决了静态资料保护的问题。

`Percona`

## [查找表和枚举类型哪个比较好？](https://postgresweekly.com/link/177994/web)
两者各有优缺点，最终取决于您的特定需求。

`Laurenz Albe`


📄 [设定 Postgres 日志：实用指南](https://postgresweekly.com/link/177995/web) – 内容比您想像的更深入。 Dash0

📄 [揭开 Postgres 段错误背后的 Arm64 JIT 编译器漏洞](https://postgresweekly.com/link/177996/web) Bonnefoy、McGarvey 和 Ward (Datadog)


## **发布**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/cypidq62wbxe1ijxngco.jpg)


## [ParadeDB 0.20.0：更简单、更快速的 Elasticsearch 等级全文搜寻](https://postgresweekly.com/link/177997/web)
ParadeDB 为 Postgres 带来了 Elasticsearch 等级、ACID 保证的搜寻功能和分析效能。 v0.20.0 引入了新的连接和析取运算符，简化了索引创建方式，并全面提升了效能。

`Philippe Noël`

## [Psycopg 3.3：适用于 Python 的现代 PostgreSQL 适配器](https://postgresweekly.com/link/177998/web)
新增对 Python 3.14 模板字串的支持，为编写既简洁又安全的动态查询开辟了新途径。官方主页。

`Psycopg Development Team`


## **📰 分类广告**


🌍 从单一节点到全球丛集：随时随地执行 PostgreSQL。试试 [pgEdge Enterprise](https://postgresweekly.com/link/178000/web)。

🛣️ [《Next.js 之路》](https://postgresweekly.com/link/178001/web)是 Robin Wieruch 开设的一门课程，教你如何使用 Next.js 15 和 React 19 进行全端 Web 开发。


[TimescaleDB 2.24](https://postgresweekly.com/link/178002/web) – 为 Postgres 资料库提供时间序列功能扩充。 v2.24 版本新增了「闪电般快速」的重新压缩功能，且连续聚合功能现已完全支援 UUIDv7。

[PEV2 v1.19.0](https://postgresweekly.com/link/178003/web) – 用于视觉化 Postgres 执行计划的 Vue.js 元件。

[PeerDB 0.36](https://postgresweekly.com/link/178004/web) – 将资料从 Postgres 串流传输到资料仓储、伫列和储存引擎。

[Supavisor 2.8](https://postgresweekly.com/link/178005/web) – Supabase 的多租户 Postgres 连线池。

[temBoard 10.0 RC1 ](https://postgresweekly.com/link/178006/web)– 透过 Web 介面管理 Postgres 伺服器丛集。

[PGSync 6.2](https://postgresweekly.com/link/178007/web) – Postgres 与 Elasticsearch/OpenSearch 的同步。



## [SynchDB 1.3：用于从其他资料库复制资料的插件](https://postgresweekly.com/link/177684/web)
一款专门用于可靠地从其他资料库系统（例如 MySQL、SQL Server 和 Oracle）复制资料的 Postgres 扩充。 v1.3 引入了一种新的、更快的基于 FDW 的快照引擎，以加快初始快照的效能。

`Hornetlabs Technology Inc`

## [Dbdock：全新的 PostgreSQL 备份与复原解决方案](https://postgresweekly.com/link/177686/web)

`Naheem Olaide`

[PGSync 6.1](https://postgresweekly.com/link/177687/web) – 用于将 Postgres 资料同步到 Elasticsearch/OpenSearch 的版本。现在无需 Redis 即可作为 WAL 消费者运作。

[Pgpool-II 4.6.4、4.5.9、4.4.14、4.3.17 和 4.2.24](https://postgresweekly.com/link/177688/web) – 连接池和负载平衡器。

[pgweb 0.17](https://postgresweekly.com/link/177689/web) – 基于 Web 的跨平台 Postgres 用户端。 （提供萤幕截图。）

[asyncpg 0.31](https://postgresweekly.com/link/177691/web) – 用于 Python 中 asyncio 的 Postgres 用户端函式库。

[Npgsql 10.0](https://postgresweekly.com/link/177692/web) – 用于 PostgreSQL 的 .NET 资料提供者。


## **🗓 2026 年即将举行的 PostgreSQL 活动**

* 🇹🇭 [FOSSASIA PGDay 2026（3 月 10 日，曼谷](https://postgresweekly.com/link/178008/web)— 与 FOSSASIA 高峰会同期举办的年度活动。征稿截止日期为 12 月 15 日。
* 🇮🇳 [PGConf India 2026（3 月 11 日至 13 日，班加罗尔）](https://postgresweekly.com/link/178010/web)— 由印度 PostgreSQL 用户群举办的多日活动。
* 🇫🇷 [pgDay Paris 2026（3月26日）](https://postgresweekly.com/link/178011/web)－征稿截止日期为12月19日。
* 🇩🇪 [PostgreSQL Conference Germany 2026（4月21-22日，埃森）](https://postgresweekly.com/link/178013/web)
* 🇧🇪 [PGConf.BE 2026（5月5日，比利时）](https://postgresweekly.com/link/178014/web)
* 🇨🇦 [PostgreSQL Development Conference 2026 – 又称 pgconf.dev（5月19日，温哥华）](https://postgresweekly.com/link/178015/web)
* 🇺🇸 [PG DATA 2026（6月4-5日，芝加哥）](https://postgresweekly.com/link/178016/web)－全新系列会议的首场活动，重点在于教育、开发者社区建设以及与学术界的交流。
* 🌐 [POSETTE 2026（6月16日，线上）](https://postgresweekly.com/link/177988/web)－由微软Postgres团队举办的免费线上活动。提案征件截止日期为2月1日。

注：此列表并非详尽无遗，我们将持续提及并推广其他活动。