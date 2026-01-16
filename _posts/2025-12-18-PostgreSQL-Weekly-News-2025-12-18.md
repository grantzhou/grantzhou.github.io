---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-12-18
---
### PostgreSQL每周新闻#629 - 2025年12月18日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/628)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/nve4yipsoyaymtgsthde.jpg)
## [pg_textsearch 现已开源](https://postgresweekly.com/link/178669/webb)
绝佳的圣诞礼物！两个月前，Tiger Data 发布了 pg_textsearch，这是一个 Postgres 扩展，用于将 BM25 排名引入全文搜索，但当时仅限于他们的云端平台。现在，如果您能够安装扩充程序，也可以将其部署到您自己的 Postgres 伺服器上（我在 Postgres.app 上编译和安装进行测试时发现非常简单）。

`Tiger Data`

💡 [VectorChord](https://postgresweekly.com/link/178672/web) and [ParadeDB](https://postgresweekly.com/link/178673/web) offer similar functionality in Postgres but with different tradeoffs and licensing.


## [提交您的 POSETTE 2026 演讲 - 征稿现已开放！](https://postgresweekly.com/link/178310/web)
 分享喜悦：在 POSETTE（Postgres 盛会）上分享您的 Postgres 故事。 POSETTE 是由微软 PostgreSQL 团队组织的免费线上开发者活动，将于 2026 年 6 月 16 日至 18 日举行。为社区贡献一份力量－请在 2 月 1 日前提交提案。详情请见内文。

`Microsoft `

## [作业系统升级后哪些索引可能会损坏？](https://postgresweekly.com/link/178310/web)
 底层作业系统升级可能会更新依赖项，进而改变 Postgres 使用的排序规则定义。 Laurenz 将解释这个问题以及解决方法。

`Laurenz Albe `


## **本周摘要**

* 🤖 [pgEdge 展示了其全新的 Postgres MCP 伺服器](https://postgresweekly.com/link/178677/web)，该伺服器可将 Claude Code 等代理工具连接到任何 Postgres 资料库，以便处理模式、指标等。

* PlanetScale 推出了 [50 美元的 PlanetScale Metal](https://postgresweekly.com/link/178678/web) 套餐——本质上是一个专业工作负载的精简版套餐，仅需 1GB 内存和 10GB 存储空间即可满足需求。

* 此外，PlanetScale 也宣布 [Postgres 18 现已上线](https://postgresweekly.com/link/178679/web)。

## [Postgres 18 的资料校验和新预设值](https://postgresweekly.com/link/178680/web)
Postgres 18 预设启用资料校验和，作为一种防止静默资料损坏的机制。

`Greg Sabino Mullane`

## [🎤 PGConf.dev 大会展望](https://postgresweekly.com/link/178319/web)
Melanie Plageman 与 Claire Giordano 一起探讨明年 5 月在加拿大温哥华举行的 PGConf.dev 2026 大会的精彩内容。

`Talking Postgres Podcast`

💡 [PGConf.dev 的征稿](https://postgresweekly.com/link/178683/web)截止日期为 2026 年 1 月 16 日，如果您想发言，请与我们联络。

## [xsql：在 SQL 方言之间转换 SQL Schema DDL](https://postgresweekly.com/link/178321/web)
一个基于 Rust 的命令列工具，用于在 SQL 方言之间转换 DDL，包括 MySQL、Postgres 和 SQLite。

`Dawit Worku`


📄 [使用 ParadeDB 将 Postgres 的分面搜寻速度提升 14 倍](https://postgresweekly.com/link/178685/web)——或者说，教 Postgres 像 Elasticsearch 一样进行分面搜寻。 James Blackwood-Sewell

📄 [自行对 Postgres 进行分区的陷阱](https://postgresweekly.com/link/178686/web)。 Alexander Belanger


## **📰 分类广告**


PostgreSQL 实例现已推出，仅需 5 美元。 [Aiven 全新开发者套餐](https://postgresweekly.com/link/178687/web)，帮助您告别闲置实例的高价。

⚡[pgEdge Agentic AI 工具包](https://postgresweekly.com/link/178688/web)：MCP 伺服器、混合搜寻、全域 Postgres。生产就绪型代理，从这里开始。

## **2025 年最热门的代码项目：**

我们将在下一期回顾 2025 年的最佳项目，但现在，我们将重点介绍今年最受关注的库、工具和版本：

* [微软发布 VS Code「Postgres IDE」](https://postgresweekly.com/link/178689/web)－早在五月份，微软就发布了其 VS Code 编辑器全新 Postgres 扩充功能的预览版，该扩充功能允许用户管理资料库物件、使用 IntelliSense 建置查询并与 Copilot 整合。

`Microsoft`

* [Multigres：Vitess for Postgres](https://postgresweekly.com/link/178690/web)——Vitess 是一个流行的 MySQL 扩展和分片集群系统，今年 Supabase 聘请了其创始人之一 Sugu Sougoumarane 来开发 Vitess for Postgres。目前该专案仍处于早期阶段，但开发工作正在进行中。

`Paul Copplestone（Supabase）`

* [DocumentDB：微软为 Postgres 带来更多 NoSQL 功能](https://postgresweekly.com/link/178693/web) — 此 DocumentDB 与亚马逊专有的 DocumentDB 不同，它是一个基于 Postgres 构建的、采用 MIT 许可的文档型 NoSQL 引擎，微软最初将其用于内部的 Azure Cosmos DB for MongoDB。

`Microsoft`

* [pgcalendar：循环日程的「无限」日历功能](https://postgresweekly.com/link/178694/web) — 如果您需要储存事件日程，并可能包含例外情况（例如假日或取消），此扩充功能提供了一种建模方法。范例。

`Huseyin Akbas`

* [PostgREST 14：Postgres 资料库的 RESTful API](https://postgresweekly.com/link/178696/web) — 2025 年对于这款可以将 Postgres 资料库直接转换为 RESTful HTTP API 的独立 Web 伺服器来说是忙碌的一年，v13 和 v14 版本均已发布。

`Joe Nelson 與 Steve Chavez`

🎄 这是 2025 年最后一期 Postgres Weekly——感谢您的阅读、投稿连结和支持！我们将于 2026 年 1 月 7 日星期三回归。到时见！