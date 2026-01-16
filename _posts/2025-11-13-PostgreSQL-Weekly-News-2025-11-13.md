---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-11-13
---
### PostgreSQL每周新闻#624 - 2025年11月13日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/624)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/w6r3bhlr0kdnrx2oy7yy.jpg)
## [VectorChord 1.0：Postgres 快速向量搜寻扩充](https://postgresweekly.com/link/176974/web)
一款专为高效能、磁碟效率高的向量相似性搜寻而设计的扩充功能。它相容于 pgvector 的资料类型和语法，但使用 IVF（倒排索引）和 RaBitQ 量化技术来提升索引和查询效能，并宣称「以相同的价格储存比 pgvector 多 26 倍的向量」。 [v1.0 版本说明](https://postgresweekly.com/link/176975/web)和 [GitHub 程式码库](https://postgresweekly.com/link/176976/web)。

`TensorChord`

💡 这篇部落格文章详细介绍了 [VectorChord 在 2024 年 12 月首次发布](https://postgresweekly.com/link/176977/web)时的背景和技术细节。

## [Agentic Postgres：开发者导向的 AI 就绪型 Postgres](https://postgresweekly.com/link/176973/web)
Tiger Data 的 Agentic Postgres 将原生 Postgres 资料库转换为 AI 原生资料库。您可以建立资料库分支、分配代理内存，并透过 REST 或 CLI 进行查询。它非常适合使用 Claude、Cursor 或自订代理程式建立的 Go 后端。免费试用，无需信用卡。

`Tiger Data`

## [Postgres 内部机制隐藏在眼前](https://postgresweekly.com/link/176978/web)
方便地提醒您，在日常工作中可以通过多种方式查询 Postgres，无论是让 psql 描述数据库的相关信息，还是查询 Postgres 的众多目录视图以获取内部数据和性能统计信息。

`Elizabeth Christensen `

## **本周摘要**

* 👋 [Postgres 13 已于今日正式停止维护](https://postgresweekly.com/link/176979/web)，这个发布五年的版本将不再提供任何安全性修补程式或漏洞修复。

* 🇺🇸 [PgDay Dallas 2026](https://postgresweekly.com/link/176980/web) 将于明年 2 月 19 日在德克萨斯州举行。早鸟票将于 11 月 28 日截止。

* 🇩🇪 [PostgreSQL Conference Germany 2026](https://postgresweekly.com/link/176981/web) 将于明年 4 月 21 日至 22 日在德国埃森举行。[CFP](https://postgresweekly.com/link/176982/web)（接受英文和德文演讲）将于 12 月 19 日截止。

* 微软备受欢迎的年度虚拟 Postgres 大会 [POSETTE 将于 2026 年回归](https://postgresweekly.com/link/176983/web)，其[CFP现已开放](https://postgresweekly.com/link/176984/web)。大会将于明年 6 月举行，征稿启事将于 2 月 1 日截止。届时我们将再次提醒您。

* 回顾 [Azure Database for PostgreSQL 在 10 月的新增功能](https://postgresweekly.com/link/176985/web)。

* Aiven 为其 [Postgres 云端服务推出了每月 8 美元的「开发者层级」](https://postgresweekly.com/link/176986/web)。

* [ClickPipes for Postgres 现在支援故障转移复制槽](https://postgresweekly.com/link/176987/web)。


## [Postgres 18 EXPLAIN 输出中新增的「索引搜寻」行是什么意思？](https://postgresweekly.com/link/176988/web)
在 Postgres 18 中，您现在会在 EXPLAIN ANALYZE 输出中看到“索引搜寻”行。如果您也像我一样想知道这些行的具体含义，那么您来对地方了。”

`Michael Christofides`


## [你知道Postgres表最多只能有1600列吗？](https://postgresweekly.com/link/176989/web)
如果你读过2017年的第226期，你可能已经知道😅了……但没错，这个限制依然存在。在这里，Frédéric会做一些有趣的实验，看看超出这个限制会带来哪些后果。

`Frédéric Delacourt`

## [▶ 在 VS Code 中为 Postgres 建立开发体验](https://postgresweekly.com/link/176989/web)
微软的 Rob Emanuele 做客 Talking Postgres 播客，与 Claire Giordano 讨论了微软今年早些时候发布的“Postgres 的 IDE”VS Code 扩展。

`Talking Postgres Podcast`

📄 [Postgres 18 中的时间约束](https://postgresweekly.com/link/176993/web) – 用于确保不同时间内资料的唯一性。 Vinicius Negrisolo

📄 [Postgres、Kafka 和事件Queue。](https://postgresweekly.com/link/176994/web) Kaarel Moppel

## **发布**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/qotwna6md0icziiteqao.jpg)


## [pg_statviz 0.8 版本发布，支援 Postgres 18](https://postgresweekly.com/link/176995/web)
一个用于对 Postgres 内部统计资料进行时间序列分析和视觉化的扩充和实用程式。 GitHub 程式码库。

`Jimmy Angelakos`

## [pg_roaringbitmap 1.0：Roaring 点阵图扩充](https://postgresweekly.com/link/176997/web)
Roaring 点阵图（此处有解释）是经过压缩和最佳化的点阵图，其效能往往优于传统的压缩位图。

`Chen Huajun`


## **📰 分类广告**

⚙️ 需要一套 100% 可用且适用于企业级应用的 PostgreSQL 入门套件？那就选 [pgEdge Enterprise Postgres](https://postgresweekly.com/link/176999/web) 吧。

🐱 [ConfigCat 功能标志服务[(https://postgresweekly.com/link/177000/web)让您无需修改程式码即可安全地发布和回溯功能。几分钟即可完成设定。


![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/ygajvrm4dvzmhozcarxa.jpg)

[pgCodeKeeper 12.1](https://postgresweekly.com/link/177007/web) – 用于处理 PL/pgSQL 和资料库模式（如上图）的 Eclipse IDE 外挂程式。

[pg-promise v12.3](https://postgresweekly.com/link/177003/web) – 适用于 Node.js 的扩展 Postgres 驱动程序，具有自动连接和事务、查询生成等功能。

[pgwire v0.35.0](https://postgresweekly.com/link/177004/web) – 基于 Rust 的 Postgres wire 协定实作。

[pg_timetable v6.2.0](https://postgresweekly.com/link/177005/web) – 具有 cron 式调度功能的独立作业调度器。

[PgDoorman 2.4](https://postgresweekly.com/link/177006/web) – 高性能连线池。