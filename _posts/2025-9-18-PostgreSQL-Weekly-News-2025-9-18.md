---
layout: post
title: PostgreSQL 每周新闻 2025-9-18
---
### PostgreSQL每周新闻#616 - 2025年9月18日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/616)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/s9qtubbavnoqyklkrzoh.jpg)
## [「数据库不接受指令」：現在該怎麼辦？](https://postgresweekly.com/link/174454/web)
這個錯誤你肯定不想遇到，因為這意味著你需要做一些認真的工作來避免交易 ID 重疊。不過，如果你真的遇到了，Laurenz 會提醒我們該怎麼做，以及一些需要避免的「低階措施」。

`Laurenz Albe`

## [亲身体验 Postgres 18：异步 I/O、B 树跳过扫描等](https://postgresweekly.com/link/174453/web)
Postgres 18 将于本月发布，现在是时候了解其以性能为中心的更新了：从异步 I/O 和计划器更改，到 B 树跳过扫描、UUIDv7、VACUUM 更改以及对生产工作负载的增强监控。

`pganalyze  `

## [核心 Postgres 資料庫分片（零停機）](https://postgresweekly.com/link/174104/web)
Gadget 是一個線上 JavaScript 開發平台，它將所有內容都保存在一個大型 Postgres 實例中，但最終達到了垂直擴展的極限。以下是他們如何在零停機或零請求的情況下對資料庫進行分片的方法。 “分片的意義在於‘硬’！”

`Harry Brundage (Gadget) `


### **本周摘要**

* 🇺🇸 [PGConf NYC ](https://postgresweekly.com/link/174456/web)將於本月稍後在紐約舉行，目前仍有門票出售。

* 您能在 Postgres 中儲存世界上已知最古老的金融交易日期嗎？[事實證明可以](https://postgresweekly.com/link/174457/web)。

* 如果您使用的是 Debian 12 系統，並且在 US/* 時區下運行 Postgres，[那麼在升級到 Debian 13 之前，請注意以下幾點](https://postgresweekly.com/link/174480/web)。


## [Postgres 邏輯複製的演變：歷史概述](https://postgresweekly.com/link/174458/web)
簡要介紹過去 20 年採用的方法。多年來，Petr 參與了許多與邏輯複製相關的專案（並在 PostgresOpen 2016 上發表了關於 Postgres 複製的演講），因此這是一個可靠的觀點。


`Petr Jelinek`

## [無需超級使用者的 Postgres 維護](https://postgresweekly.com/link/174460/web)
查看內建的、預先定義的管理角色，這些角色可讓您執行許多維護任務而無需超級使用者存取權限。


`Radim Marek`

## [Postgres 18 令人興奮](https://postgresweekly.com/link/174458/web)
距離 Postgres 18 最終版本發布還有一周時間，但已經有很多值得興奮的地方，尤其是異步 I/O 的引入，它將為我們許多人帶來性能提升。


`Elizabeth Christensen（Crunchy Data）`

📊 [Cyber​​tec PostgreSQL 企業版 (PGEE) 中 TDE 和校驗和的成本](https://postgresweekly.com/link/174463/web)——透明数据加密對效能的影響如此之小，我感到很驚喜。 Christoph Berg

📄 [如何在 Go 和 Postgres 中實作寄件匣模式](https://postgresweekly.com/link/174464/web)－一種確保訊息最終到達指定目的地的彈性方法。 Alex Pliutau

📄 [使用 CloudNativePG 讓 Postgres 缩放至零](https://postgresweekly.com/link/174465/web) Esther Minano Sanz (Xata)

📺 [使用 PGlite 將 Postgres 編譯為 WebAssembly](https://postgresweekly.com/link/174466/web)——30 分鐘演講。 Sam Willis

## 📰 分類廣告

🏁 [擴展毫秒速度](https://postgresweekly.com/link/174467/web)。 Redis 8.2 已實現每秒 100 萬次以上操作。[免費部署](https://postgresweekly.com/link/174467/web)並在您自己的技術堆疊中進行壓力測試。

💌 您知道我們有一系列新聞簡報嗎？看看 [JavaScript Weekly](https://postgresweekly.com/link/174468/web)、[Go Weekly](https://postgresweekly.com/link/174469/web) 和 [Ruby Weekly](https://postgresweekly.com/link/174470/web)，更全面地了解我們的工作。


## **发布**

## [pgsql_tweaks 1.0.0 發布](https://postgresweekly.com/link/173459/web)
這是作者作為 Postgres 用戶在日常工作中使用的一套函數和視圖，涵蓋檢查數據類型、收集統計數據、WAL 監控、查找未使用的索引以及轉換函數等領域。官方主頁上有每個功能的文件。

`Stefanie Janine Stölting`

## [pgstream：Postgres 複製與 DDL 變更](https://postgresweekly.com/link/174124/web)
一個基於 Go 的變更資料擷取 (CDC) 命令列工具和函式庫，支援 Postgres 複製，並支援對其他 Postgres 資料庫、Elasticsearch/OpenSearch 或 Webhook 等目標的 DDL 變更。更多資訊請參閱這篇文章。

`Xata`

🌐 [osm2pgsql 2.2](https://postgresweekly.com/link/174475/web) – 將 OpenStreetMap 資料匯入 Postgres/PostGIS 資料庫。

[無狀態 Postgres 查詢路由器 (SPQR) 2.7 ](https://postgresweekly.com/link/174476/web)– 一種水平分片方法，最初由 Yandex Cloud 建構。

[VectorChord 0.5.2](https://postgresweekly.com/link/174477/web) – Postgres 中可擴充、快速且磁碟友善的向量搜尋。

[River 0.25](https://postgresweekly.com/link/174478/web) – 適用於 Go 應用的強大 Postgres 驅動的作業處理系統。

[pgwatch v4 Beta 版](https://postgresweekly.com/link/174479/web)