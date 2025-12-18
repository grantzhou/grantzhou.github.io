---
layout: post
title: PostgreSQL 每周新闻 2025-12-18
---
### PostgreSQL每周新闻#629 - 2025年12月18日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/628)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/nve4yipsoyaymtgsthde.jpg)
## [pg_textsearch 現已開源](https://postgresweekly.com/link/178669/webb)
絕佳的聖誕禮物！兩個月前，Tiger Data 發布了 pg_textsearch，這是一個 Postgres 擴展，用於將 BM25 排名引入全文搜索，但當時僅限於他們的雲端平台。現在，如果您能夠安裝擴充程序，也可以將其部署到您自己的 Postgres 伺服器上（我在 Postgres.app 上編譯和安裝進行測試時發現非常簡單）。

`Tiger Data`

💡 [VectorChord](https://postgresweekly.com/link/178672/web) and [ParadeDB](https://postgresweekly.com/link/178673/web) offer similar functionality in Postgres but with different tradeoffs and licensing.


## [提交您的 POSETTE 2026 演讲 - 徵稿現已開放！](https://postgresweekly.com/link/178310/web)
 分享喜悅：在 POSETTE（Postgres 盛會）上分享您的 Postgres 故事。 POSETTE 是由微軟 PostgreSQL 團隊組織的免費線上開發者活動，將於 2026 年 6 月 16 日至 18 日舉行。為社區貢獻一份力量－請在 2 月 1 日前提交提案。詳情請見內文。

`Microsoft `

## [作業系統升級後哪些索引可能會損壞？](https://postgresweekly.com/link/178310/web)
 底層作業系統升級可能會更新依賴項，進而改變 Postgres 使用的排序規則定義。 Laurenz 將解釋這個問題以及解決方法。

`Laurenz Albe `


## **本周摘要**

* 🤖 [pgEdge 展示了其全新的 Postgres MCP 伺服器](https://postgresweekly.com/link/178677/web)，該伺服器可將 Claude Code 等代理工具連接到任何 Postgres 資料庫，以便處理模式、指標等。

* PlanetScale 推出了 [50 美元的 PlanetScale Metal](https://postgresweekly.com/link/178678/web) 套餐——本質上是一個專業工作負載的精簡版套餐，僅需 1GB 內存和 10GB 存儲空間即可滿足需求。

* 此外，PlanetScale 也宣布 [Postgres 18 現已上線](https://postgresweekly.com/link/178679/web)。

## [Postgres 18 的資料校驗和新預設值](https://postgresweekly.com/link/178680/web)
Postgres 18 預設啟用資料校驗和，作為一種防止靜默資料損壞的機制。

`Greg Sabino Mullane`

## [🎤 PGConf.dev 大會展望](https://postgresweekly.com/link/178319/web)
Melanie Plageman 與 Claire Giordano 一起探討明年 5 月在加拿大溫哥華舉行的 PGConf.dev 2026 大會的精彩內容。

`Talking Postgres Podcast`

💡 [PGConf.dev 的徵稿](https://postgresweekly.com/link/178683/web)截止日期為 2026 年 1 月 16 日，如果您想發言，請與我們聯絡。

## [xsql：在 SQL 方言之間轉換 SQL Schema DDL](https://postgresweekly.com/link/178321/web)
一個基於 Rust 的命令列工具，用於在 SQL 方言之間轉換 DDL，包括 MySQL、Postgres 和 SQLite。

`Dawit Worku`


📄 [使用 ParadeDB 將 Postgres 的分面搜尋速度提升 14 倍](https://postgresweekly.com/link/178685/web)——或者說，教 Postgres 像 Elasticsearch 一樣進行分面搜尋。 James Blackwood-Sewell

📄 [自行對 Postgres 進行分區的陷阱](https://postgresweekly.com/link/178686/web)。 Alexander Belanger


## **📰 分類廣告**


PostgreSQL 實例現已推出，僅需 5 美元。 [Aiven 全新開發者套餐](https://postgresweekly.com/link/178687/web)，幫助您告別閒置實例的高價。

⚡[pgEdge Agentic AI 工具包](https://postgresweekly.com/link/178688/web)：MCP 伺服器、混合搜尋、全域 Postgres。生產就緒型代理，從這裡開始。

## **2025 年最熱門的代碼項目：**

我們將在下一期回顧 2025 年的最佳項目，但現在，我們將重點介紹今年最受關注的庫、工具和版本：

* [微軟發布 VS Code「Postgres IDE」](https://postgresweekly.com/link/178689/web)－早在五月份，微軟就發布了其 VS Code 編輯器全新 Postgres 擴充功能的預覽版，該擴充功能允許用戶管理資料庫物件、使用 IntelliSense 建置查詢並與 Copilot 整合。

`Microsoft`

* [Multigres：Vitess for Postgres](https://postgresweekly.com/link/178690/web)——Vitess 是一個流行的 MySQL 擴展和分片集群系統，今年 Supabase 聘請了其創始人之一 Sugu Sougoumarane 來開發 Vitess for Postgres。目前該專案仍處於早期階段，但開發工作正在進行中。

`Paul Copplestone（Supabase）`

* [DocumentDB：微軟為 Postgres 帶來更多 NoSQL 功能](https://postgresweekly.com/link/178693/web) — 此 DocumentDB 與亞馬遜專有的 DocumentDB 不同，它是一個基於 Postgres 構建的、採用 MIT 許可的文檔型 NoSQL 引擎，微軟最初將其用於內部的 Azure Cosmos DB for MongoDB。

`Microsoft`

* [pgcalendar：循環日程的「無限」日曆功能](https://postgresweekly.com/link/178694/web) — 如果您需要儲存事件日程，並可能包含例外情況（例如假日或取消），此擴充功能提供了一種建模方法。範例。

`Huseyin Akbas`

* [PostgREST 14：Postgres 資料庫的 RESTful API](https://postgresweekly.com/link/178696/web) — 2025 年對於這款可以將 Postgres 資料庫直接轉換為 RESTful HTTP API 的獨立 Web 伺服器來說是忙碌的一年，v13 和 v14 版本均已發布。

`Joe Nelson 與 Steve Chavez`

🎄 這是 2025 年最後一期 Postgres Weekly——感謝您的閱讀、投稿連結和支持！我們將於 2026 年 1 月 7 日星期三回歸。到時見！