---
layout: post
title: PostgreSQL 每周新闻 2025-12-11
---
### PostgreSQL每周新闻#628 - 2025年12月11日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/628)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/v32txavpytfc4mqacel6.jpg)
## [EXPLAIN 執行計畫中的掃描類型詳解](https://postgresweekly.com/link/178311/web)
使用 EXPLAIN 了解查詢的執行方式對於偵錯效能問題或最佳化 SQL 語句大有裨益，但「順序掃描」和「索引掃描」之類的術語究竟是什麼意思呢？ Elizabeth 在這裡詳細講解了幾種主要的掃描類型，並附有圖表——你肯定能從中有所收穫！

`Elizabeth Christensen`


## [(CERN) 的 TimescaleDB：海量時間序列數據，規模空前](https://postgresweekly.com/link/178310/web)
CERN 的下一代歸檔系統選擇 TimescaleDB，以實現極高的吞吐量、7-10 倍的壓縮率以及 10-40 倍的讀取速度提升。了解 PostgreSQL + TimescaleDB 如何為 500 多個系統提供支持，並有望成為 CERN 歷史資料儲存的標準。

`Tiger Data `


## **本周摘要**

* [DB Fiddle](https://postgresweekly.com/link/178312/web) 線上資料庫實驗平台剛剛新增了 Postgres 18.1 的支援。

* Paul Ramsey 對近期舉辦的 [PostGIS Day 活動進行了非常詳細的回顧](https://postgresweekly.com/link/178313/web)。

* Floor Drees 採訪了 [Postgres 貢獻者 Bryan Green](https://postgresweekly.com/link/178314/web)，了解他如何透過 Postgres 進入開源領域。


## [關於Postgres中的約束，您應該了解什麼](https://postgresweekly.com/link/178317/web)
您可以為表格和列定義約束，以強制執行資料條件。 Gulcin將深入探討細節。

`Gulcin Yildirim Jelinek (Xata)`

## [閉環：建立使用 Postgres 分支的編碼代理](https://postgresweekly.com/link/178319/web)
Xata 的開發者建立了一個代理程式（實際上是開源的），專門用於監控資料庫以查找問題並提出修復建議。

`Divyendu Singh (Xata)`

## [Postgres、MongoDB 以及「無法擴展」的真正意義](https://postgresweekly.com/link/178321/web)
對 The Register 最近一篇報導的反思，該報道引用 MongoDB 執行長的話說「PostgreSQL 無法擴展」。

`Umair Shahid`


📄 [使用 Neon Postgres 進行一週實時流量測試的經驗總結](https://postgresweekly.com/link/178323/web)——對無伺服器計費方式的優缺點進行了深入思考。 Ishan Das Sharma

📄 [為 Postgres 外部資料包裝器新增非同步流程處理功能](https://postgresweekly.com/link/178324/web)。 Bo Lu（Supabase）

📄 [深入探討 Postgres 18 中的 UUIDv4 與 UUIDv7](https://postgresweekly.com/link/178325/web)。 Josef Machytka


## **发布**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/pfml9flkfq7mtl7nysak.jpg)


## [temBoard 10.0：Postgres 遠端控制/儀錶板](https://postgresweekly.com/link/178326/web)
一個基於 Python 建構的 Postgres Web 儀表板和監控系統。您只需在目標伺服器上安裝代理，temBoard Web 應用程式即可在任何您想要的位置運作。 v10 版本新增了對 Postgres 18 的支持，並可在 Python 3.9 及更高版本上運行，同時提供 RPM 和 DEB 軟體包。 GitHub 程式碼庫。

`Dalibo`


## **📰 分類廣告**


🌎 推出基於 Kubernetes 的精簡高可用性 PostgreSQL 部署（分散式或單區域），[利用 CNPG 與 pgEdge 的整合](https://postgresweekly.com/link/178330/web)。

PostgreSQL 現已推出，僅需 5 美元。使用 [Aiven 的全新開發者套餐](https://postgresweekly.com/link/178344/web)，告別為閒置實例支付過高費用的煩惱。


## [VectorChord 1.0：Postgres 上的快速向量搜尋](https://postgresweekly.com/link/178332/web)
這款前景廣闊、效能卓越的向量索引和查詢擴充程式於一年前首次發布，如今已達到 v1.0 版本。我們上個月曾提及該版本，但現在團隊撰寫了這篇博文，深入探討了 VectorChord 相較於 pgvector 如何實現如此顯著的效能提升。

`Jinjing Zhou`

💡 他們在文章[《我們如何在 PostgreSQL 上 20 分鐘內實現 1 億向量索引》](https://postgresweekly.com/link/178334/web)中進行了更深入的技術探討。


## [隆重介紹 pg_clickhouse：用於查詢 ClickHouse 的 Postgres 擴充](https://postgresweekly.com/link/178335/web)
ClickHouse 是一個流行的開源 OLAP 系統，此擴充功能提供了一種直接從 Postgres 透明地執行 ClickHouse 分析查詢的方法。

`David Wheeler (ClickHouse)`

[WhoDB 0.82](https://postgresweekly.com/link/178337/web) – 輕量級的新一代多資料庫資料瀏覽器。

[linq2db 6.0](https://postgresweekly.com/link/178338/web) – LINQ to Database 提供者。現已支援 .NET 10。

[PGSync 7.0](https://postgresweekly.com/link/178339/web) – Postgres 與 Elasticsearch/OpenSearch 的同步。

[Procrastinate 3.6](https://postgresweekly.com/link/178340/web) – 基於 Postgres 的 Python 任務佇列。

[pgroll 0.15](https://postgresweekly.com/link/178341/web) – 零停機、可逆的模式遷移。

[Squawk 2.32](https://postgresweekly.com/link/178342/web) – 用於 Postgres 遷移和 SQL 的程式碼檢查器。

[pgAdmin 4 v9.11](https://postgresweekly.com/link/178343/web)