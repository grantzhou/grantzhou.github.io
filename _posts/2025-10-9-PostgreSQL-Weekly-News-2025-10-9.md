---
layout: post
title: PostgreSQL 每周新闻 2025-10-9
---
### PostgreSQL每周新闻#619 - 2025年10月9日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/619)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/myxf1as8sucatryemg4h.jpg)
## [建置和debug Postgres](https://postgresweekly.com/link/175084/web)
如何設定容器，從原始程式碼建置 Postgres，然後使用 GDB 和 VS Code 進行debug。如果你想深入了解 Postgres 的內部機制，這些技巧很有用。

`Stefanos Baziotis`


## [使用 S3 範圍讀取探索 Postgres 到 Parquet 歸檔的 JSON 資料](https://postgresweekly.com/link/175083/web)
如何將「冷」 JSON 從 Postgres 移至 S3 上的 Parquet，然後能夠快速取回它而無需讀取整個檔案。

`Shayon Mukherjee `

## [如何實施 Postgres DevOps 和安全性](https://postgresweekly.com/link/175385/web)
審查、批准、部署和強制執行查詢存取控制。此外還有動態資料屏蔽和審計追蹤。一體化 GUI 工作區，開源，受到 350 多家公司的信賴，包括 Linear 和 note.com。

`Bytebase `

## [▶ Postgres 18 實作：非同步 I/O、B 樹跳躍掃描、UUIDv7](https://postgresweekly.com/link/175388/web)
pganalyze 的創辦人舉辦了一場網路研討會，深入探討了 Postgres 18 中一些更值得注意的改進。關於非同步 I/O 的部分（從 4:20 到 22:30）特別有用。

`Lukas Fittl `



### **本周摘要**

* 🌐 [PostGIS Day 2025](https://postgresweekly.com/link/175390/web) 是一場免費的線上活動，將於 11 月 20 日舉行，面向對地理空間應用感興趣的 Postgres 用戶。

* 🇫🇷 [2026 年巴黎 pgDay 會議](https://postgresweekly.com/link/175391/web)現已開放徵文。會議將於 2026 年 3 月舉行，投稿截止日期為 12 月 19 日。

* 歷史悠久的 Postgres 顧問公司 [CYBERTEC](https://postgresweekly.com/link/175392/web) 為慶祝成立 25 週年，[特採訪其執行長兼創辦人 Hans-Jürgen Schönig](https://postgresweekly.com/link/175393/web)，講述公司成立和發展歷程。

* 🇯🇵 [2025 年日本 PostgreSQL 大會](https://postgresweekly.com/link/175394/web)將於 11 月 11 日在東京舉行。


## [關於開發 Postgres 的 OAuth 支持](https://postgresweekly.com/link/175395/web)
Postgres 中 OAuth 支持的首批倡導者之一（在此以實際意義進行探索）講述了它在 Postgres 18 中的出現、它為何令人興奮以及未來的發展。


`Jacob Champion`


📄 [使用 Postgres CONSTRAINT](https://postgresweekly.com/link/175397/web) 進行棘輪操作 – 強制約束（例如「NOT NULL」）的方法，無需立即在全表範圍內強制執行。 Andrew Judson

📄 [使用邏輯複製進行 Postgres 遷移](https://postgresweekly.com/link/175398/web) Elizabeth Christensen

📄 [IBM 邀請 CockroachDB 在其大型主機上使用「PostgreSQL」](https://postgresweekly.com/link/175399/web)——這在 The Register 上是一個典型的古怪標題！事實上，IBM 正在尋求在其大型主機硬體上提供類似 Postgres 的資料庫。 The Register

📄 [TimescaleDB 中的 SkipScan](https://postgresweekly.com/link/175400/web)：DISTINCT 為什麼緩慢，我們如何建造它，以及如何使用它 Aksman 和 Hein（TigerData）

📄 [Postgres 16 中的關鍵操作增強和整合選項](https://postgresweekly.com/link/175401/web) Sebastian Insausti


## **发布**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/ilr1y1fd1qnoc2gwjagy.jpg)

## [pgwatch 4.0：靈活的 Postgres 監控解決方案](https://postgresweekly.com/link/175402/web)
透過 Grafana 儀表板提供使用者友善的介面，讓您可以檢查各種指標（運作狀況、效能、索引使用情況、I/O 等）和趨勢。 v4.0 引入了各種增強功能並放棄了對 Grafana v10 的支援。

`CYBERTEC`

## [pg_statement_rollback v1.5：語句層級的伺服器端回滾](https://postgresweekly.com/link/175404/web)
新增語句層級的伺服器端事務回滾，類似 Oracle 或 Db2。此版本新增了對 Postgres 18 的支援。

`Hexacluster`

[PostgreSQL R2DBC 驅動程式 1.1](https://postgresweekly.com/link/175405/web) – 將響應式 API 引入 Java 世界中的關聯式資料庫。

[QuestDB 9.1](https://postgresweekly.com/link/175406/web)– 基於 Java 的時間序列資料庫，相容於 Postgres 有線協定。

[River 0.26](https://postgresweekly.com/link/175407/web) – 快速可靠的 Postgres 後台作業系統，適用於 Go 語言。

[tbls 1.89](https://postgresweekly.com/link/175408/web) – 自動以 Markdown 格式（例如在 CI 中）記錄資料庫。

[Goose 3.26](https://postgresweekly.com/link/175409/web) – 資料庫遷移工具。支援 SQL 和 Go 函數。

[Mathesar 0.6](https://postgresweekly.com/link/175410/web) – 類似電子表格的 Postgres 表格介面。

[Barman 3.16](https://postgresweekly.com/link/175411/web) – 備份與災難復原工具。