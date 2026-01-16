---
layout: post
title: PostgreSQL 每周新闻 2025-11-6
---
### PostgreSQL每周新闻#623 - 2025年11月6日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/623)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/gyp9wmug1js5rwoeb5xc.jpg)
## [不要給 Postgres 分配過多記憶體](https://postgresweekly.com/link/176669/web)
記憶體越多越好，對嗎？正如 Tomas 在這裡演示的那樣，Postgres 的 maintenance_work_mem 和 work_mem 設定並非如此。 CPU 快取大小和作業系統記憶體管理對結果起著關鍵作用。

`Tomas Vondra`

## [隆重推出 pg_lake：將您的資料湖與 Postgres 整合](https://postgresweekly.com/link/176670/web)
這是一套擴展程序，可為 Postgres 添加全面的 Iceberg 支援和資料湖存取（包括 Parquest、CSV 和 JSON 支援），並將 DuckDB 透明地整合到查詢引擎中，從而實現快速執行，無需離開 Postgres。 GitHub 程式碼庫。

`Craig Kerstiens (Snowflake) `

## [使用 Azure 上的 Postgres 建立 AI 應用](https://postgresweekly.com/link/176354/web)
探索將進階 AI 功能整合到應用中的實用步驟和工具。了解如何將 Azure AI 和機器學習與 Azure 上的 Postgres 集成，以建立智慧的 AI 應用。立即開始學習。

`Microsoft `

## **本周摘要**

* 🗓️ [PostgreSQL 活動日曆](https://postgresweekly.com/link/176673/web)是一個追蹤 Postgres 相關活動的網站，它還提供一個 ICS/iCalendar 文件，您可以將其新增至自己的日曆應用程式。目前活動清單涵蓋到 2026 年 9 月在奧地利舉辦的 🇦🇹 [PGDay Austria](https://postgresweekly.com/link/176674/web)。

* [postgres-contrib.org](https://postgresweekly.com/link/176675/web) 是一個博客，它每週匯總 Postgres 專案的貢獻。

* 🇨🇿 如果您想在 2026 年[布拉格 PostgreSQL 開發者日](https://postgresweekly.com/link/176676/web)上發言，其徵稿將於下週截止。該活動將於 1 月 27 日至 28 日在捷克布拉格舉行。

* 雖然[PlanetScale 尚未推出每月 5 美元的 Postgres 套餐](https://postgresweekly.com/link/176678/web)，但本週它在社交媒體上引起了不小的轟動。

## [🇪🇺 PGConf EU 2025 之旅總結](https://postgresweekly.com/link/176679/web)
[歐洲最重要的 Postgres 大會](https://postgresweekly.com/link/176680/web)兩週前在拉脫維亞舉行，Claire（Talking Postgres 播客的主持人）分享了一份詳細的旅行報告，涵蓋了她作為演講嘉賓、微軟代表等角色的行程。報告還包含大量照片。

`Claire Giordano (Microsoft)`

💡 Cyber​​tec 的 Cornelia Biacsics 也[撰寫了類似的報告](https://postgresweekly.com/link/176682/web)。


📄 [“無需 Kafka，只需使用 Postgres” 被認為有害](https://postgresweekly.com/link/176683/web)——對我們上週刊登的一篇文章的回應。 Gunnar Morling

📄 [如何透過 WAL 監聽資料庫變更](https://postgresweekly.com/link/176684/web) Peter Ullrich

📄 [使用 Pgcat 在 Postgres 中實現事務池](https://postgresweekly.com/link/176685/web) Phil Eaton

📄 [SQL 查詢在 Postgres 中的運行之旅](https://postgresweekly.com/link/176686/web) Jesús Espino

📄 [什麼是 Postgres 中的「髒頁」？](https://postgresweekly.com/link/176687/web) Umair Shahid


## **发布**

## [pg_timetable 6.1 發布：高級作業調度擴展](https://postgresweekly.com/link/176688/web)
一個成熟的、高級的獨立作業調度程序擴展，完全駐留在您的資料庫中，允許您調度 Postgres 命令和查詢、系統程序和內置操作，以及將任務鏈接在一起。

`CYBERTEC PostgreSQL International GmbH`

## **📰 分類廣告**

日本領先的 C2C 內容創作平台 note.com 如何以[即時 (JIT) 存取控制](https://postgresweekly.com/link/176689/web)取代其 GitHub Actions + SSH 代理流程，從而實現更安全的 Aurora Postgres 存取。

🧠 [您信賴的 100% 開源 PostgreSQL](https://postgresweekly.com/link/176690/web)：現已升級至企業級，並支援全球分散式部署。


## [PostGraphile v5 候選版本發布](https://postgresweekly.com/link/176691/web)
PostGraphile 提供了一種建立由 Postgres 資料庫支援的自動化 GraphQL API 的方法（類似於 PostgREST 在資料庫前端提供 RESTful API）。 v5 版本歷經五年開發，即將發布。

`Benjie and Jem`


[PGSync 6.0](https://postgresweekly.com/link/176694/web) – 用於將 Postgres 資料同步到 Elasticsearch/OpenSearch 的工具。從 6.0 版本開始，它也支援 MySQL/MariaDB。

[無狀態 Postgres 查詢路由 (SPQR) 2.8](https://postgresweekly.com/link/176695/web) – 一種水平分片方案，最初由 Yandex Cloud 開發。

[PostgREST 14.1](https://postgresweekly.com/link/176696/web) – 適用於任何 Postgres 資料庫的 REST API。

[Squawk 2.30](https://postgresweekly.com/link/176697/web) – 用於 Postgres 遷移和 SQL 程式碼檢查的工具。