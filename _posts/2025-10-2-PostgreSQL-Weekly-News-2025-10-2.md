---
layout: post
title: PostgreSQL 每周新闻 2025-10-2
---
### PostgreSQL每周新闻#618 - 2025年10月2日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/617)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/y9wrtagqf7bunkiwxang.jpg)
## [深入了解 Postgres 18 的功能](https://postgresweekly.com/link/175084/web)
如果我們仍然保持著上週發布 Postgres 18 時的興奮之情，請見諒。 Tudor 將以比冗長的發布說明更容易理解的方式，向您介紹各種令人興奮且實用的新功能。

`Tudor Golubenco (Xata)`

💡 Bytebase 的 Tianzhou 在《[Postgres 18 新功能－開發者視角](https://postgresweekly.com/link/175087/web)》中也發表了類似的綜述。本期稍後，我們也將深入探討 Postgres 18 的具體功能。

## [🚀 將 Postgres 擴展到 2PB 數據量和每日數萬億指標](https://postgresweekly.com/link/175083/web)
TimescaleDB 的創建者 TigerData 正在將 Postgres 推向新的極限：擴展到 2PB 數據量和每日 1.5 萬億指標——無需專有黑盒或隱藏工具。使用 Tiger Postgres，您可以獲得大規模擴展，同時保留您熟悉和喜愛的 SQL。

`TigerData    `

## [Postgres 18 中的 psql 新增了管道功能](https://postgresweekly.com/link/175088/web)
從 Postgres 18 開始，psql 配備了在 SQL 腳本中使用管道的命令，Daniel 指出這「可以大幅提升查詢吞吐量」。

`Daniel Vérité`


### **本周摘要**

* Postgres 18 剛剛發布，但 Hubert Lubaczewski 期待著 Postgres 19 的到來，並發布了一系列部落格文章，介紹 [GROUP BY ALL](https://postgresweekly.com/link/175089/web) 的引入、[random(min, max) 的日期和時間戳版本](https://postgresweekly.com/link/175090/web)，以及在 EXPLAIN 中[顯示 memoize 規劃器估算值](https://postgresweekly.com/link/175091/web)。

* EDB 的 Floor Drees 分享了 EDB 公司為[新 Postgres 貢獻者引入的幕後花絮](https://postgresweekly.com/link/175092/web)。


## [如何執行 UPDATE ... LIMIT](https://postgresweekly.com/link/175093/web)
抱歉，您不能在 Postgres 中使用帶有 LIMIT 的 UPDATE（或 DELETE）（儘管某些 SQL 方言，如 MySQL 的方言，支持它）但您可以（謹慎地）使用其他方法。


`Laurenz Albe`


## [Postgres 18 及後續版本：從 AIO 到 Direct IO？](https://postgresweekly.com/link/175094/web)
Postgres 18 最令人興奮的功能之一是它支援非同步 IO，但我們能否利用 Direct IO 並完全跳過作業系統緩存，做得更好？


`Laurenz Albe`

## [我如何學習使用 wal_inspect](https://postgresweekly.com/link/175096/web)
pg_walinspect 是一個用於檢查預寫日誌內容的模組。


`Hettie Dombrovskaya`

📄 [在 Postgres 中實作卡爾曼濾波器來平滑 GPS 資料](https://postgresweekly.com/link/175098/web)——這絕對是我以前在 SQL 中從未見過的功能。 Thorsten Rieß

📄 [Postgres 18：RETURNING 子句中的舊行與新行](https://postgresweekly.com/link/175099/web) Brandur Leach

📄 [Postgres 18 中 COPY 命令如何變得更加用戶友好](https://postgresweekly.com/link/175100/web) Deepak Mahto

📄 [Postgres 18 中的累積統計](https://postgresweekly.com/link/175101/web) Cédric Villemain


## **发布**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/xpbhlpxeazos0yneoxrx.jpg)

## [PG Back Web 0.5：具有 Web 介面的 Postgres 備份系統](https://postgresweekly.com/link/175102/web)
一款基於 Go 語言的應用，旨在為 Postgres 備份、定時備份（包括備份到 S3）、備份監控和 Webhook 帶來更友善的使用者介面。它以 Docker 映像的形式提供，現在也支援 Postgres 18。

`Luis Eduardo`

## [介紹 Elephantshark：一款監控 Postgres 網路流量的工具](https://postgresweekly.com/link/175103/web)
一款基於 Ruby 的工具，位於 Postgres 協定交換的雙方之間，在解析和記錄訊息的同時雙向轉送訊息。 GitHub 倉庫。

`George MacKerron (Neon)`

[pgrx 0.16.1](https://postgresweekly.com/link/175105/web) – 使用 Rust 建立 Postgres 擴充功能的方法（完整功能集請點擊此處）– 現已支援 Postgres 18。

[VectorChord 0.5.3](https://postgresweekly.com/link/175107/web) – Postgres 中可擴充、快速且磁碟友善的向量搜尋。

[pgmetrics 1.18](https://postgresweekly.com/link/175108/web) – 從正在運行的 Postgres 伺服器收集並顯示統計資料。

[ChartDB 1.16](https://postgresweekly.com/link/175109/web) – 以圖表為基礎的開源資料庫編輯器。