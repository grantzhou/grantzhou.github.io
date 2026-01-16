---
layout: post
title: PostgreSQL 每周新闻 2025-12-4
---
### PostgreSQL每周新闻#626 - 2025年12月4日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/627)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/rgnw8r0j0wkkom96fzut.jpg)
## [關於Postgres中JSON資料的高效儲存](https://postgresweekly.com/link/177987/web)
JSON與JSONB作為資料類型，pglz與lz4作為壓縮演算法…哪一種組合能以最有效率的方式儲存JSON資料？ Hubert進行了一些調查，以了解不同組合在查詢速度和儲存空間方面的效能表現。

`Hubert depesz Lubaczewski`


## [POSETTE 2026：徵稿啟事 (CFP) 現已開放！](https://postgresweekly.com/link/177986/web)
[POSETTE：Postgres](https://postgresweekly.com/link/177988/web)，是由微軟 Postgres 團隊組織的免費線上開發者活動，將於 6 月 16 日至 18 日舉行。徵稿啟事 (CFP) 開放至 2 月 1 日。歡迎新舊演講者踴躍投稿！了解更多詳情。

`Microsoft `


## **本周摘要**

* [Postgres.app](https://postgresweekly.com/link/177989/web) 是一款受歡迎且便利的工具，可在 macOS 上快速執行 Postgres 實例。它最近新增了幾個常用擴充功能（PL/v8、http、pg_parquet 和 TimescaleDB）的[下載功能，方便使用者快速安裝](https://postgresweekly.com/link/177990/web)。

* [AWS 為其各種產品（包括 RDS 和 Aurora）推出了新的資料庫節省計劃](https://postgresweekly.com/link/177991/web)，該計劃將使那些能夠在一年內按小時支付固定費用的用戶受益。

* [Schema3D](https://postgresweekly.com/link/177992/web) 是一種有趣的實驗性工具，可用於在 3D 空間中視覺化資料庫模式。 （使用右上角的鉛筆圖示輸入您自己的 SQL 語句。）


## [透明資料加密 (TDE) 現已支援 Postgres 18](https://postgresweekly.com/link/177993/web)
Percona 現在發布了一個 Postgres 18.1 版本，該版本完全支援原生 TDE 和非同步 I/O。 TDE 提供檔案層級的加密，解決了靜態資料保護的問題。

`Percona`

## [查找表和枚舉類型哪個比較好？](https://postgresweekly.com/link/177994/web)
兩者各有優缺點，最終取決於您的特定需求。

`Laurenz Albe`


📄 [設定 Postgres 日誌：實用指南](https://postgresweekly.com/link/177995/web) – 內容比您想像的更深入。 Dash0

📄 [揭開 Postgres 段錯誤背後的 Arm64 JIT 編譯器漏洞](https://postgresweekly.com/link/177996/web) Bonnefoy、McGarvey 和 Ward (Datadog)


## **发布**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/cypidq62wbxe1ijxngco.jpg)


## [ParadeDB 0.20.0：更簡單、更快速的 Elasticsearch 等級全文搜尋](https://postgresweekly.com/link/177997/web)
ParadeDB 為 Postgres 帶來了 Elasticsearch 等級、ACID 保證的搜尋功能和分析效能。 v0.20.0 引入了新的連接和析取運算符，簡化了索引創建方式，並全面提升了效能。

`Philippe Noël`

## [Psycopg 3.3：適用於 Python 的現代 PostgreSQL 適配器](https://postgresweekly.com/link/177998/web)
新增對 Python 3.14 模板字串的支持，為編寫既簡潔又安全的動態查詢開闢了新途徑。官方主頁。

`Psycopg Development Team`


## **📰 分類廣告**


🌍 從單一節點到全球叢集：隨時隨地執行 PostgreSQL。試試 [pgEdge Enterprise](https://postgresweekly.com/link/178000/web)。

🛣️ [《Next.js 之路》](https://postgresweekly.com/link/178001/web)是 Robin Wieruch 開設的一門課程，教你如何使用 Next.js 15 和 React 19 進行全端 Web 開發。


[TimescaleDB 2.24](https://postgresweekly.com/link/178002/web) – 為 Postgres 資料庫提供時間序列功能擴充。 v2.24 版本新增了「閃電般快速」的重新壓縮功能，且連續聚合功能現已完全支援 UUIDv7。

[PEV2 v1.19.0](https://postgresweekly.com/link/178003/web) – 用於視覺化 Postgres 執行計畫的 Vue.js 元件。

[PeerDB 0.36](https://postgresweekly.com/link/178004/web) – 將資料從 Postgres 串流傳輸到資料倉儲、佇列和儲存引擎。

[Supavisor 2.8](https://postgresweekly.com/link/178005/web) – Supabase 的多租戶 Postgres 連線池。

[temBoard 10.0 RC1 ](https://postgresweekly.com/link/178006/web)– 透過 Web 介面管理 Postgres 伺服器叢集。

[PGSync 6.2](https://postgresweekly.com/link/178007/web) – Postgres 與 Elasticsearch/OpenSearch 的同步。



## [SynchDB 1.3：用於從其他資料庫複製資料的插件](https://postgresweekly.com/link/177684/web)
一款專門用於可靠地從其他資料庫系統（例如 MySQL、SQL Server 和 Oracle）複製資料的 Postgres 擴充。 v1.3 引入了一種新的、更快的基於 FDW 的快照引擎，以加快初始快照的效能。

`Hornetlabs Technology Inc`

## [Dbdock：全新的 PostgreSQL 備份與復原解決方案](https://postgresweekly.com/link/177686/web)

`Naheem Olaide`

[PGSync 6.1](https://postgresweekly.com/link/177687/web) – 用於將 Postgres 資料同步到 Elasticsearch/OpenSearch 的版本。現在無需 Redis 即可作為 WAL 消費者運作。

[Pgpool-II 4.6.4、4.5.9、4.4.14、4.3.17 和 4.2.24](https://postgresweekly.com/link/177688/web) – 連接池和負載平衡器。

[pgweb 0.17](https://postgresweekly.com/link/177689/web) – 基於 Web 的跨平台 Postgres 用戶端。 （提供螢幕截圖。）

[asyncpg 0.31](https://postgresweekly.com/link/177691/web) – 用於 Python 中 asyncio 的 Postgres 用戶端函式庫。

[Npgsql 10.0](https://postgresweekly.com/link/177692/web) – 用於 PostgreSQL 的 .NET 資料提供者。


## **🗓 2026 年即將舉行的 PostgreSQL 活動**

* 🇹🇭 [FOSSASIA PGDay 2026（3 月 10 日，曼谷](https://postgresweekly.com/link/178008/web)— 與 FOSSASIA 高峰會同期舉辦的年度活動。徵稿截止日期為 12 月 15 日。
* 🇮🇳 [PGConf India 2026（3 月 11 日至 13 日，班加羅爾）](https://postgresweekly.com/link/178010/web)— 由印度 PostgreSQL 用戶群舉辦的多日活動。
* 🇫🇷 [pgDay Paris 2026（3月26日）](https://postgresweekly.com/link/178011/web)－徵稿截止日期為12月19日。
* 🇩🇪 [PostgreSQL Conference Germany 2026（4月21-22日，埃森）](https://postgresweekly.com/link/178013/web)
* 🇧🇪 [PGConf.BE 2026（5月5日，比利時）](https://postgresweekly.com/link/178014/web)
* 🇨🇦 [PostgreSQL Development Conference 2026 – 又稱 pgconf.dev（5月19日，溫哥華）](https://postgresweekly.com/link/178015/web)
* 🇺🇸 [PG DATA 2026（6月4-5日，芝加哥）](https://postgresweekly.com/link/178016/web)－全新系列會議的首場活動，重點在於教育、開發者社區建設以及與學術界的交流。
* 🌐 [POSETTE 2026（6月16日，線上）](https://postgresweekly.com/link/177988/web)－由微軟Postgres團隊舉辦的免費線上活動。提案徵件截止日期為2月1日。

註：此列表並非詳盡無遺，我們將持續提及並推廣其他活動。