---
layout: post
title: PostgreSQL 每周新闻 2025-10-23
---
### PostgreSQL每周新闻#621 - 2025年10月23日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/621)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/zktpbzsf69swswdqb4nc.jpg)
## [你的資料庫是讀重還是寫重？](https://postgresweekly.com/link/175714/web)
大多數資料庫的讀取操作往往比寫入操作更重，但這取決於你的工作負載。這值得確定嗎？在調優方面，答案是肯定的。 David 展示了一個史詩級的 SQL 查詢，它能幫你計算出表格的讀寫比。

`David and Elizabeth Christensen`

💡 上面帖子中的查詢工作正常，但如果您還想包含只讀或寫的表，請將第 19 行的 AND 更改為 OR。

## [Tiger Lake：連接 Postgres 和 Lakehouse](https://postgresweekly.com/link/176013/web)
Tiger Lake 將 Postgres 與您的 Lakehouse 即時統一。無需管道，無需編排。使用開放格式持續串流、分析和提供資料。基於一個整合的 Postgres 原生架構，建立儀表板、代理程式和分析工具。

`TigerData  `

## [Tiger Data 推出免費 Postgres 計畫](https://postgresweekly.com/link/175385/web)
Tiger Data（前身為 Timescale）提供 Postgres 平台已有一段時間，但從未推出免費套餐。現在，您可以免費獲得最多兩項服務，每項服務最高可提供 750MB 的儲存空間。鑑於目前的行業現狀，該計劃主要面向 AI 和代理開發人員，但任何人都可以將其用於小型專案或實驗。

`TigerData`

💡 Aiven, Neon 和 Supabase 等其他供應商也提供類似的免費套餐。

## [🔎 Postgres 中的混合搜尋：缺少的手冊](https://postgresweekly.com/link/176019/web)
解釋在相關性排名方面，使用 BM25 評分的全文搜尋（由 ParadeDB 提供支援）與向量相似性搜尋（由 pgvector 提供支援）相結合如何勝過 Postgres 的本機全文搜尋。

`James Blackwood-Sewell`

## [DESCending 索引的優勢](https://postgresweekly.com/link/176021/web)
“索引定義中 DESC 子句的常見用例是支援混合 ORDER BY 子句。但在某些情況下，PostgreSQL 可以更有效率地填入降序索引，並且對降序索引進行正向掃描的效能可能優於對升序索引進行反向掃描。”

`Laurenz Albe`

## [▶ 速度提高 14 倍，運算量減少 12 倍：有時 Postgres 確實是您所需要的一切](https://postgresweekly.com/link/176022/web)
James 的團隊如何從不可靠的 12 台伺服器 HBase/OpenTSDB 叢集轉變為使用 Postgres/Timescale 處理時間序列工作負載且正常運行時間達到 100% 的兩台伺服器。

`James Udiljak`

📄 [在 Windows 上為 Postgres 18 進行便攜式設定 – 簡易指南](https://postgresweekly.com/link/176023/web)。 Mohit Sindhwani

📺 [正確設定 Postgres 參數，防止效能低落 – 一小時網路研討會錄影](https://postgresweekly.com/link/176024/web)。 Greg Dostatni

📄 [PostGIS 效能：pg_stat_statements 和 Postgres 調優](https://postgresweekly.com/link/176025/web) Paul Ramsey


## **发布**

## [NoraSearch：快速查找子字串匹配偏移量和計數的擴展](https://postgresweekly.com/link/176026/web)
例如，在"abracadabra"中搜尋"abra"將傳回 ``{{0,4},{7,4}}``。作者引用了一個用於分析 DNA 序列的用例。

`Lemmer EL ASSAL`

## [pg_ivm 1.13：增量視圖維護 (IVM) 擴充 -](https://postgresweekly.com/link/176027/web)
一種更有效的增量更新物化視圖的方法，僅套用更改，而不是像 REFRESH MATERIALIZED VIEW 那樣完全重新計算視圖。 v1.13 增加了對外連接的支援。

`IVM Development Group`

## [PL/Haskell 5.0：在您的 SQL 函數中使用 Haskell](https://postgresweekly.com/link/176028/web)
Haskell 是一種函數式語言，而不是過程式語言，但您仍然可以使用它以 Postgres 可以使用的方式定義流程。 v5 增加了對日期和時間類型的支援。

`Edward F. Behn, Jr.`


[pgwire 0.34](https://postgresweekly.com/link/176029/web)– 使用 Rust 函式庫實作的 Postgres 連線協定。

[pg_dbms_errlog v2.2](https://postgresweekly.com/link/176030/web) – 用於模擬 Oracle DBMS_ERRLOG 的擴充。

[postgres-meta 0.93](https://postgresweekly.com/link/176031/web) – 用於管理 Postgres 的 RESTful API。

[Squawk 2.29](https://postgresweekly.com/link/176032/web) – 用於 Postgres 遷移和 SQL 的 Linter。

[pgAdmin 4 v9.9](https://postgresweekly.com/link/176033/web) – 流行的 Postgres 管理工具。