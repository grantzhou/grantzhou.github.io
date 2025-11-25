---
layout: post
title: PostgreSQL 每周新闻 2025-11-20
---
### PostgreSQL每周新闻#625 - 2025年11月20日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/625)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/ddacvvudkcpt1aousimk.jpg)
## [RegreSQL：Postgres 查詢的迴歸測試](https://postgresweekly.com/link/177305/web)
深入了解基於 Go 語言的工具，可將 Postgres 本身的迴歸測試方法套用至 SQL 查詢，以驗證對查詢或模式的變更是否會破壞查詢的預期運作方式（例如，是否仍使用正確的索引或掃描類型？）。

`Radim Marek`


## [Agentic Postgres：開發者導向的 AI 就緒型 Postgres](https://postgresweekly.com/link/177304/web)
Tiger Data 的 Agentic Postgres 將原生 Postgres 資料庫轉換為 AI 原生資料庫。您可以建立資料庫分支、分配代理內存，並透過 REST 或 CLI 進行查詢。它非常適合使用 Claude、Cursor 或自訂代理程式建立的 Go 後端。免費試用，無需信用卡。

`Tiger Data`

## [微軟推出全新 PostgreSQL 服務：Azure Horizo​​nDB](https://postgresweekly.com/link/177306/web)
Azure 已有 Azure Database for PostgreSQL，但 Horizo​​nDB 提供“更高水平的效能和可擴展性”，支援跨節點最多 3072 個虛擬核心 (vCore)，資料庫容量高達 128TB，可滿足企業級工作負載的需求。目前該服務處於「早期預覽」階段，估計需要相當的預算。

`Microsoft`

## **本周摘要**

* [Amazon RDS for PostgreSQL 現在支援 Postgres 18](https://postgresweekly.com/link/177308/web)，具體來說是 Postgres 18.1。 [pgcollection](https://postgresweekly.com/link/177309/web) 以及其他常用擴充功能的最新版本也已包含在內。

* 🏴研再讀形體形體許​​數許力許​​L重量殼許種種種種記號 Jimmy Angelakos 宣布將於 12 月 11 日在蘇格蘭愛丁堡舉辦[第一屆 PostgreSQL 聚會](https://postgresweekly.com/link/177310/web)。

* 如果您使用 Docker 的官方 Postgres 映像，在進行[小版本升級時請務必小心](https://postgresweekly.com/link/177311/web)，因為底層 Debian 版本也可能會更新，從而強制資料庫進行不必要的排序規則更新。

* [create_pg_super_document](https://postgresweekly.com/link/177312/web) 是一個使用 LLM 為 Postgres 程式碼庫中的每個符號建立文件的項目。如果您正在開發擴展或深入研究 Postgres 實現，這將非常有用。

* Pavlo Golub 從 Postgres 的角度[回顧了今年的 Google Summer of Code 活動](https://postgresweekly.com/link/177313/web)，以及參與者所做的工作。


## [在 Postgres 中儲存產品、價格和訂單](https://postgresweekly.com/link/176988/web)
解決在儲存產品資訊時因過度樂觀的標準化而導致的問題。

`Hans-Jürgen Schönig`


## [PostGIS效能優化：交集謂詞和疊加層](https://postgresweekly.com/link/176989/web)
這是一系列關於如何最大限度發揮PostGIS效能的文章中的最新一篇。

`Paul Ramsey`

📄 [MD5 密碼支援已棄用，如何更新密碼](https://postgresweekly.com/link/177317/web)？ ——這項工作雖然枯燥，但總得有人做。 Dan Langille

📊 [PlanetScale PostgreSQL 與 Hetzner Local Postgres 的比較——當然，兩者並不完全可比](https://postgresweekly.com/link/177318/web)。 Muhammad Azeez

📄 [如何在 Python、Django 和 Postgres 中使用 UUIDv7](https://postgresweekly.com/link/177319/web)？ Paolo Melchiorre

## **发布**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/vrzffuhfvpzthygmedjw.jpg)


## [PgManage 1.4：資料庫管理 Web 工具](https://postgresweekly.com/link/177320/web)
一個開源的基於 Web 的介面，以 Postgres 為中心，但也支援 MySQL、SQLite 和 Oracle。您可以同時操作多個資料庫，檢視表格、檢視、函數等，檢視查詢計劃，並取得 SQL 自動補全功能以建立查詢。

`Command Prompt, Inc.`

## [🌐 Martin 1.0：快速輕量級的 PostGIS、MBtiles 和 PMtiles 切片伺服器](https://postgresweekly.com/link/177321/web)
一個地理空間切片伺服器及工具集，能夠從大型 PostGIS 資料庫動態產生向量切片，​​並提供來自 PMTiles 和 MBTiles 檔案的切片。經過八年的開發，現已發布 v1.0 版本。您可以在其主頁上查看演示。

`MapLibre Contributors`


## **📰 分類廣告**


停機並非不可避免。了解 pgEdge + CloudNativePG 如何在 Kubernetes 上實現高可用性 Postgres。[了解更多並立即註冊](https://postgresweekly.com/link/177324/web)！

🛣️ [《Next.js 之路》](https://postgresweekly.com/link/177325/web)是由 Robin Wieruch 主講的課程，旨在教授使用 Next.js 15 和 React 19 進行全端 Web 開發。對於準備超越前端的 JavaScript 開發人員來說，這是理想之選。

## [pg_flo：即時串流、轉換和路由 Postgres 資料](https://postgresweekly.com/link/177321/web)
提供一系列過濾器和轉換功能，可簡化在生產資料庫和測試資料庫等之間移動資料的操作，支援三種模式：複製並串流、僅串流或一次性複製。使用 NATS 和 Postgres 的複製功能。

`Shayon Mukherjee`

## [Spock：邏輯多主 PostgreSQL 複製](https://postgresweekly.com/link/177326/web)

`pgEdge`

[🐶 PgDog 0.1.15](https://postgresweekly.com/link/177327/web) – 為 Postgres 提供水平擴展和自動分片功能。現已支援基於模式的分片。

[PGSync 6.0](https://postgresweekly.com/link/177328/web) – 將 Postgres（現在也支援 MySQL/MariaDB）資料同步到 Elasticsearch/OpenSearch。

[QuestDB 9.2](https://postgresweekly.com/link/177329/web) – 基於 Java 的時序資料庫，相容於 Postgres 的 wire 協定。

[PgParty 1.10](https://postgresweekly.com/link/177330/web) – 使用 Active Record（在 Ruby 和 Rails 中）建立和管理 Postgres 分割區。

[River 0.27](https://postgresweekly.com/link/177331/web) – 適用於 Go 的快速可靠的基於 Postgres 的後台任務系統。

[pg-boss 10.4](https://postgresweekly.com/link/177332/web) – 適用於 Node.js 的基於 Postgres 的任務佇列系統。