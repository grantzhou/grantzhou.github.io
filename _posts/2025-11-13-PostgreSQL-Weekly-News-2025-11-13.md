---
layout: post
title: PostgreSQL 每周新闻 2025-11-13
---
### PostgreSQL每周新闻#624 - 2025年11月13日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/624)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/w6r3bhlr0kdnrx2oy7yy.jpg)
## [VectorChord 1.0：Postgres 快速向量搜尋擴充](https://postgresweekly.com/link/176974/web)
一款專為高效能、磁碟效率高的向量相似性搜尋而設計的擴充功能。它相容於 pgvector 的資料類型和語法，但使用 IVF（倒排索引）和 RaBitQ 量化技術來提升索引和查詢效能，並宣稱「以相同的價格儲存比 pgvector 多 26 倍的向量」。 [v1.0 版本說明](https://postgresweekly.com/link/176975/web)和 [GitHub 程式碼庫](https://postgresweekly.com/link/176976/web)。

`TensorChord`

💡 這篇部落格文章詳細介紹了 [VectorChord 在 2024 年 12 月首次發佈](https://postgresweekly.com/link/176977/web)時的背景和技術細節。

## [Agentic Postgres：開發者導向的 AI 就緒型 Postgres](https://postgresweekly.com/link/176973/web)
Tiger Data 的 Agentic Postgres 將原生 Postgres 資料庫轉換為 AI 原生資料庫。您可以建立資料庫分支、分配代理內存，並透過 REST 或 CLI 進行查詢。它非常適合使用 Claude、Cursor 或自訂代理程式建立的 Go 後端。免費試用，無需信用卡。

`Tiger Data`

## [Postgres 內部機制隱藏在眼前](https://postgresweekly.com/link/176978/web)
方便地提醒您，在日常工作中可以通過多種方式查詢 Postgres，無論是讓 psql 描述數據庫的相關信息，還是查詢 Postgres 的眾多目錄視圖以獲取內部數據和性能統計信息。

`Elizabeth Christensen `

## **本周摘要**

* 👋 [Postgres 13 已於今日正式停止維護](https://postgresweekly.com/link/176979/web)，這個發布五年的版本將不再提供任何安全性修補程式或漏洞修復。

* 🇺🇸 [PgDay Dallas 2026](https://postgresweekly.com/link/176980/web) 將於明年 2 月 19 日在德克薩斯州舉行。早鳥票將於 11 月 28 日截止。

* 🇩🇪 [PostgreSQL Conference Germany 2026](https://postgresweekly.com/link/176981/web) 將於明年 4 月 21 日至 22 日在德國埃森舉行。[CFP](https://postgresweekly.com/link/176982/web)（接受英文和德文演講）將於 12 月 19 日截止。

* 微軟備受歡迎的年度虛擬 Postgres 大會 [POSETTE 將於 2026 年回歸](https://postgresweekly.com/link/176983/web)，其[CFP現已開放](https://postgresweekly.com/link/176984/web)。大會將於明年 6 月舉行，徵稿啟事將於 2 月 1 日截止。屆時我們將再次提醒您。

* 回顧 [Azure Database for PostgreSQL 在 10 月的新增功能](https://postgresweekly.com/link/176985/web)。

* Aiven 為其 [Postgres 雲端服務推出了每月 8 美元的「開發者層級」](https://postgresweekly.com/link/176986/web)。

* [ClickPipes for Postgres 現在支援故障轉移複製槽](https://postgresweekly.com/link/176987/web)。


## [Postgres 18 EXPLAIN 輸出中新增的「索引搜尋」行是什麼意思？](https://postgresweekly.com/link/176988/web)
在 Postgres 18 中，您現在會在 EXPLAIN ANALYZE 輸出中看到“索引搜尋”行。如果您也像我一樣想知道這些行的具體含義，那麼您來對地方了。”

`Michael Christofides`


## [你知道Postgres表最多只能有1600列嗎？](https://postgresweekly.com/link/176989/web)
如果你讀過2017年的第226期，你可能已經知道😅了……但沒錯，這個限制依然存在。在這裡，Frédéric會做一些有趣的實驗，看看超出這個限制會帶來哪些後果。

`Frédéric Delacourt`

## [▶ 在 VS Code 中為 Postgres 建立開發體驗](https://postgresweekly.com/link/176989/web)
微軟的 Rob Emanuele 做客 Talking Postgres 播客，與 Claire Giordano 討論了微軟今年早些時候發布的“Postgres 的 IDE”VS Code 擴展。

`Talking Postgres Podcast`

📄 [Postgres 18 中的時間約束](https://postgresweekly.com/link/176993/web) – 用於確保不同時間內資料的唯一性。 Vinicius Negrisolo

📄 [Postgres、Kafka 和事件Queue。](https://postgresweekly.com/link/176994/web) Kaarel Moppel

## **发布**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/qotwna6md0icziiteqao.jpg)


## [pg_statviz 0.8 版本發布，支援 Postgres 18](https://postgresweekly.com/link/176995/web)
一個用於對 Postgres 內部統計資料進行時間序列分析和視覺化的擴充和實用程式。 GitHub 程式碼庫。

`Jimmy Angelakos`

## [pg_roaringbitmap 1.0：Roaring 點陣圖擴充](https://postgresweekly.com/link/176997/web)
Roaring 點陣圖（此處有解釋）是經過壓縮和最佳化的點陣圖，其效能往往優於傳統的壓縮位圖。

`Chen Huajun`


## **📰 分類廣告**

⚙️ 需要一套 100% 可用且適用於企業級應用的 PostgreSQL 入門套件？那就選 [pgEdge Enterprise Postgres](https://postgresweekly.com/link/176999/web) 吧。

🐱 [ConfigCat 功能標誌服務[(https://postgresweekly.com/link/177000/web)讓您無需修改程式碼即可安全地發布和回溯功能。幾分鐘即可完成設定。


![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/ygajvrm4dvzmhozcarxa.jpg)

[pgCodeKeeper 12.1](https://postgresweekly.com/link/177007/web) – 用於處理 PL/pgSQL 和資料庫模式（如上圖）的 Eclipse IDE 外掛程式。

[pg-promise v12.3](https://postgresweekly.com/link/177003/web) – 適用於 Node.js 的擴展 Postgres 驅動程序，具有自動連接和事務、查詢生成等功能。

[pgwire v0.35.0](https://postgresweekly.com/link/177004/web) – 基於 Rust 的 Postgres wire 協定實作。

[pg_timetable v6.2.0](https://postgresweekly.com/link/177005/web) – 具有 cron 式調度功能的獨立作業調度器。

[PgDoorman 2.4](https://postgresweekly.com/link/177006/web) – 高性能連線池。