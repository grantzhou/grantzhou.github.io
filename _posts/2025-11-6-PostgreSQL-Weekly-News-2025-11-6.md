---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-11-6
---
### PostgreSQL每周新闻#623 - 2025年11月6日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/623)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/gyp9wmug1js5rwoeb5xc.jpg)
## [不要给 Postgres 分配过多记忆体](https://postgresweekly.com/link/176669/web)
记忆体越多越好，对吗？正如 Tomas 在这里演示的那样，Postgres 的 maintenance_work_mem 和 work_mem 设定并非如此。 CPU 快取大小和作业系统记忆体管理对结果起著关键作用。

`Tomas Vondra`

## [隆重推出 pg_lake：将您的资料湖与 Postgres 整合](https://postgresweekly.com/link/176670/web)
这是一套扩展程序，可为 Postgres 添加全面的 Iceberg 支援和资料湖存取（包括 Parquest、CSV 和 JSON 支援），并将 DuckDB 透明地整合到查询引擎中，从而实现快速执行，无需离开 Postgres。 GitHub 程式码库。

`Craig Kerstiens (Snowflake) `

## [使用 Azure 上的 Postgres 建立 AI 应用](https://postgresweekly.com/link/176354/web)
探索将进阶 AI 功能整合到应用中的实用步骤和工具。了解如何将 Azure AI 和机器学习与 Azure 上的 Postgres 集成，以建立智慧的 AI 应用。立即开始学习。

`Microsoft `

## **本周摘要**

* 🗓️ [PostgreSQL 活动日历](https://postgresweekly.com/link/176673/web)是一个追踪 Postgres 相关活动的网站，它还提供一个 ICS/iCalendar 文件，您可以将其新增至自己的日历应用程式。目前活动清单涵盖到 2026 年 9 月在奥地利举办的 🇦🇹 [PGDay Austria](https://postgresweekly.com/link/176674/web)。

* [postgres-contrib.org](https://postgresweekly.com/link/176675/web) 是一个博客，它每周汇总 Postgres 专案的贡献。

* 🇨🇿 如果您想在 2026 年[布拉格 PostgreSQL 开发者日](https://postgresweekly.com/link/176676/web)上发言，其征稿将于下周截止。该活动将于 1 月 27 日至 28 日在捷克布拉格举行。

* 虽然[PlanetScale 尚未推出每月 5 美元的 Postgres 套餐](https://postgresweekly.com/link/176678/web)，但本周它在社交媒体上引起了不小的轰动。

## [🇪🇺 PGConf EU 2025 之旅总结](https://postgresweekly.com/link/176679/web)
[欧洲最重要的 Postgres 大会](https://postgresweekly.com/link/176680/web)两周前在拉脱维亚举行，Claire（Talking Postgres 播客的主持人）分享了一份详细的旅行报告，涵盖了她作为演讲嘉宾、微软代表等角色的行程。报告还包含大量照片。

`Claire Giordano (Microsoft)`

💡 Cyber​​tec 的 Cornelia Biacsics 也[撰写了类似的报告](https://postgresweekly.com/link/176682/web)。


📄 [“无需 Kafka，只需使用 Postgres” 被认为有害](https://postgresweekly.com/link/176683/web)——对我们上周刊登的一篇文章的回应。 Gunnar Morling

📄 [如何透过 WAL 监听资料库变更](https://postgresweekly.com/link/176684/web) Peter Ullrich

📄 [使用 Pgcat 在 Postgres 中实现事务池](https://postgresweekly.com/link/176685/web) Phil Eaton

📄 [SQL 查询在 Postgres 中的运行之旅](https://postgresweekly.com/link/176686/web) Jesús Espino

📄 [什么是 Postgres 中的「脏页」？](https://postgresweekly.com/link/176687/web) Umair Shahid


## **发布**

## [pg_timetable 6.1 发布：高级作业调度扩展](https://postgresweekly.com/link/176688/web)
一个成熟的、高级的独立作业调度程序扩展，完全驻留在您的资料库中，允许您调度 Postgres 命令和查询、系统程序和内置操作，以及将任务链接在一起。

`CYBERTEC PostgreSQL International GmbH`

## **📰 分类广告**

日本领先的 C2C 内容创作平台 note.com 如何以[即时 (JIT) 存取控制](https://postgresweekly.com/link/176689/web)取代其 GitHub Actions + SSH 代理流程，从而实现更安全的 Aurora Postgres 存取。

🧠 [您信赖的 100% 开源 PostgreSQL](https://postgresweekly.com/link/176690/web)：现已升级至企业级，并支援全球分散式部署。


## [PostGraphile v5 候选版本发布](https://postgresweekly.com/link/176691/web)
PostGraphile 提供了一种建立由 Postgres 资料库支援的自动化 GraphQL API 的方法（类似于 PostgREST 在资料库前端提供 RESTful API）。 v5 版本历经五年开发，即将发布。

`Benjie and Jem`


[PGSync 6.0](https://postgresweekly.com/link/176694/web) – 用于将 Postgres 资料同步到 Elasticsearch/OpenSearch 的工具。从 6.0 版本开始，它也支援 MySQL/MariaDB。

[无状态 Postgres 查询路由 (SPQR) 2.8](https://postgresweekly.com/link/176695/web) – 一种水平分片方案，最初由 Yandex Cloud 开发。

[PostgREST 14.1](https://postgresweekly.com/link/176696/web) – 适用于任何 Postgres 资料库的 REST API。

[Squawk 2.30](https://postgresweekly.com/link/176697/web) – 用于 Postgres 迁移和 SQL 程式码检查的工具。