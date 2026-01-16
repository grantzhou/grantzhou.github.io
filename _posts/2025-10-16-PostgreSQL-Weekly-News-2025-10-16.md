---
layout: post
title: PostgreSQL 每周新闻 2025-10-16
---
### PostgreSQL每周新闻#620 - 2025年10月16日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/620)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/e692qah5p8cek2vviye8.jpg)
## [對 Postgres 17 與 18 進行基準測試](https://postgresweekly.com/link/175714/web)
作者在 Postgres 17 和 18 之間進行了一系列詳細的性能基準測試，大約有 96 種組合，令人欣慰的是，Postgres 18 為我們帶來了良好的性能提升、本地磁碟規則，並且調整設置仍然是值得的。

`Ben Dicken (PlanetScale)`


## [note.com 如何實現即時 (JIT) 資料庫存取控制](https://postgresweekly.com/link/175713/web)
note.com 是日本領先的 C2C 創作者平台，它用 Bytebase 的即時 (JIT) 訪問控制取代了用於臨時 Aurora Postgres 訪問的內部 GitHub Actions + SSH 代理流。

`Bytebase `

## [PGConf NYC 2025 的 Postgres 之旅報告](https://postgresweekly.com/link/175385/web)
PGConf NYC 2025 於兩週前舉行，取得了巨大成功。以播客 Talking Postgres 聞名的 Claire 詳細講述了此次活動的點滴，並分享了許多精彩的照片。

`Claire Giordano (Microsoft) `

[EDB 團隊也回顧了 PGConf NYC 的主要內容](https://postgresweekly.com/link/175717/web)。

## [▶ Postgres 18 實作：非同步 I/O、B 樹跳躍掃描、UUIDv7](https://postgresweekly.com/link/175388/web)
pganalyze 的創辦人舉辦了一場網路研討會，深入探討了 Postgres 18 中一些更值得注意的改進。關於非同步 I/O 的部分（從 4:20 到 22:30）特別有用。

`Lukas Fittl `

### **本周摘要**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/kgq3heua484bbrb3amtp.jpg)

* JetBrains 發布了[其最新的開發者生態系統現狀報告](https://postgresweekly.com/link/175719/web)（見上文），Postgres 首次超越 MySQL，成為 JetBrains 生態系統中最受歡迎的資料庫系統。

* Heroku 常被譽為 Postgres 雲端平台/服務概念的先驅，近日，Heroku [發布了「下一代」Heroku Postgres 的預告](https://postgresweekly.com/link/175720/web)，將其提升到了更高的規模。

* 🇨🇿 [2026 年布拉格 PostgreSQL 開發者日](https://postgresweekly.com/link/175721/web)將於明年 1 月 27 日至 28 日在捷克共和國舉行。如果您想發言，其提案徵集截止日期為 11 月 14 日。

* 微軟 Azure 團隊分享了 Azure Database for PostgreSQL [2025 年 9 月新功能的綜述](https://postgresweekly.com/link/175723/web)。

* 一個使用 Postgres 和 SQL [解決邏輯難題的精彩範例](https://postgresweekly.com/link/175724/web)。


## [探索 Postgres 18 新增的 UUIDv7 支援](https://postgresweekly.com/link/175725/web)
與 UUIDv4 不同，UUIDv7 值具有單調性且可按時間排序，這帶來了一些優勢。


`Fridriksson and Miller (Aiven)`

📄 [從文本到標記](https://postgresweekly.com/link/175726/web)：標記化管道的工作原理 James Blackwood-Sewell

📄 [理解並設定 Postgres JDBC 的獲取大小](https://postgresweekly.com/link/175727/web) Shane Borden


## **发布**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/rrsyyhvvev1npg7ro4z5.jpg)

## [pqr.sql：在 Postgres 中使用純 SQL 產生二維碼](https://postgresweekly.com/link/175728/web)
這個想法很巧妙，但可能有一些不太明顯的用例。不過，它確實需要幾百行 SQL 才能實現。

`Tanel Põder`

## [PGSync 5.0：Postgres 到 ElasticSearch/OpenSearch 的同步](https://postgresweekly.com/link/175730/web)
一款中間件，用於擷取資料庫中的變更並將結構化文件寫入搜尋叢集。 v5.0 最初僅適用於 Postgres，現已新增 MySQL/MariaDB 支援。 GitHub 程式碼庫。

`Tolu Aina`

## [使用 SQL 清理 SQL](https://postgresweekly.com/link/175732/web)
一種概念驗證 PL/pgSQL 函數，可以取得原始 SQL 並傳回經過清理的版本（不含任何個人識別資訊）。

`Jeremy Schneider`

## [pg_qualstats：用來收集謂詞統計資料的擴充](https://postgresweekly.com/link/175733/web)
分析資料庫查詢中最常用的謂詞，或許可以以此創造最有效的索引。 POWA（Postgres 工作負載分析器）專案的一部分。

`Powa Team`

[BemiDB 1.7](https://postgresweekly.com/link/175735/web) – 開源 Snowflake 與 Fivetran 替代方案捆綁在一起。

[ParadeDB 0.19](https://postgresweekly.com/link/175736/web) – 基於 Postgres 建構的事務型 Elasticsearch 替代方案。

[PgDog 0.1.10](https://postgresweekly.com/link/175737/web) – 支援 Postgres 的水平擴展和自動分片功能。