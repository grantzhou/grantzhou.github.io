---
layout: post
title: PostgreSQL 每周新闻 2025-11-27
---
### PostgreSQL每周新闻#626 - 2025年11月27日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/626)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/qqnso0ubnlkmlojsw4nf.jpg)
## [Postgres 19 即將迎來超高速聚合](https://postgresweekly.com/link/177659/web)
Postgres 19 距離正式發布還有十個月，但最近的一些提交表明，我們可以期待聚合速度的顯著提升，而無需更改查詢語句。查詢優化器不再採用「先連接後聚合」的模式，而是能夠根據實際情況選擇先聚合，然後在更合適的時機進行連接。

`Hans-Jürgen Schönig`


## [Tiger Data教會AI編寫真正的Postgres程式碼](https://postgresweekly.com/link/177658/web)
立即體驗－Tiger Data教會AI如何寫出道地的Postgres程式碼，並將其開源。 pg-aiguide將真正的資料庫專業知識帶入Claude Code或任何其他支援MCP的工具。。

`Tiger Data`


## **本周摘要**

* 📘 [《Just Use Postgres!》](https://postgresweekly.com/link/177660/web)是 Denis Magda 撰寫、Manning 出版的一本書，本月正式發行。本書是對 Postgres 的現代入門介紹，內容超越了典型的關聯式資料庫管理系統 (RDBMS) 操作，涵蓋了 JSON、全文搜尋、pgvector、TimescaleDB、訊息佇列實作等諸多面向。

* 🌐 12 月 9 日，舊金山灣區 Postgres 用戶群將[舉辦一場免費的線上活動](https://postgresweekly.com/link/177661/web)，屆時 Christophe Pettus 將介紹 Postgres 18 的新功能。

* 🇧🇪 [FOSDEM PGDay 2026 ](https://postgresweekly.com/link/177662/web)將於 1 月 30 日在比利時布魯塞爾舉行，如果您有意發言，論文徵集現已開放，截止日期為 12 月 15 日。

* 旅遊報告：Andreas Scherbaum 參加了 [PostgreSQL 日本大會](https://postgresweekly.com/link/177664/web)和 [PostgreSQL 柏林大會](https://postgresweekly.com/link/177665/web)，Henrietta Dombrovskaya 則報道了[草原 PostgreSQL 用戶組](https://postgresweekly.com/link/177666/web)的聚會情況。

* [PlanetScale](https://postgresweekly.com/link/177667/web)推出了每月5美元的Postgres託管服務。


## [探索 psql 腳本語言中的斐波那契數列和圖靈完備性](https://postgresweekly.com/link/177668/web)
psql 支援多種語法元素，讓您可以執行一些在資料庫前端可能意想不到的結構化、類似程式設計的任務。 Phil 將進行簡報；您可能也能從中了解一些關於 psql 的知識。

`Phil Eaton`


📺 [計算機想要遺失你的資料](https://postgresweekly.com/link/177669/web)－SREcon25 大會上的演講，以 MySQL 和 Postgres 為例，探討安全資料儲存。 Chris Sinjakli

📄 [PostGIS 效能：資料採樣](https://postgresweekly.com/link/177670/web)－Paul 關於 PostGIS 效能係列文章的最新一篇。 Paul Ramsey

📄 [Laravel 的 PostgreSQL 與 MongoDB：選擇合適的資料庫](https://postgresweekly.com/link/177672/web)－從 Laravel 的角度出發，進行了詳盡的比較。 Farhan Hasin Chowdhury

📄 [Postgres 18：跳躍掃描－突破最左索引的限制](https://postgresweekly.com/link/177673/web)。 Ahsan Hadi

📄 [為什麼你應該對資料庫進行分片](https://postgresweekly.com/link/177674/web)？ Lev Kokotov (PgDog)


## **发布**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/fdv1bgar1zoh5vyodpme.jpg)


## [🤖 pg_ai_query：自然語言查詢擴充](https://postgresweekly.com/link/177675/web)
這款有趣的擴充功能能夠接收您用自然語言編寫的請求，並使用 OpenAI 或 Anthropologie 模型將其即時轉換為 SQL。 README 文件中提供了許多範例。

`Sachin Beniwal`

## [IvorySQL 5.0：開源的 Oracle 相容 Postgres](https://postgresweekly.com/link/177677/web)
從 Oracle 遷移到 Postgres 的方法有很多，IvorySQL 的方法是新增相容性元素，例如支援 Oracle 的 PL/SQL 語法和 XML 函數。 [v5.0](https://postgresweekly.com/link/177678/web) 現在基於 Postgres 18，並引入了更多 Oracle 相容性功能以及對更多 Postgres 擴充功能的支援。此外，現在還有一個[線上 Playground](https://postgresweekly.com/link/177679/web)，您可以在其中體驗實例。

`IvorySQL`


## **📰 分類廣告**

🐘 [pgEdge Enterprise Postgres](https://postgresweekly.com/link/177680/web)：100% 開源、可擴充、設計正常運作時間高達 99.999%，並支援分散式部署。

🛣️ [《通往 Next.js 之路》](https://postgresweekly.com/link/177681/web)是由 Robin Wieruch 主講的課程，旨在幫助學員使用 Next.js 15 和 React 19 進行全端 Web 開發。對於準備超越前端的 JavaScript 開發人員來說，這門課程堪稱完美之選。

## [SynchDB 1.3：用於從其他資料庫複製資料的擴充](https://postgresweekly.com/link/177684/web)
一款專門用於可靠地從其他資料庫系統（例如 MySQL、SQL Server 和 Oracle）複製資料的 Postgres 擴充。 v1.3 引入了一種新的、更快的基於 FDW 的快照引擎，以加快初始快照的效能。

`Hornetlabs Technology Inc`

## [Dbdock：全新的 PostgreSQL 備份與復原解決方案](https://postgresweekly.com/link/177686/web)

`Naheem Olaide`

[PGSync 6.1](https://postgresweekly.com/link/177687/web) – 用於將 Postgres 資料同步到 Elasticsearch/OpenSearch 的版本。現在無需 Redis 即可作為 WAL 消費者運作。

[Pgpool-II 4.6.4、4.5.9、4.4.14、4.3.17 和 4.2.24](https://postgresweekly.com/link/177688/web) – 連接池和負載平衡器。

[pgweb 0.17](https://postgresweekly.com/link/177689/web) – 基於 Web 的跨平台 Postgres 用戶端。 （提供螢幕截圖。）

[asyncpg 0.31](https://postgresweekly.com/link/177691/web) – 用於 Python 中 asyncio 的 Postgres 用戶端函式庫。

[Npgsql 10.0](https://postgresweekly.com/link/177692/web) – 用於 PostgreSQL 的 .NET 資料提供者。