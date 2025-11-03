---
layout: post
title: PostgreSQL 每周新闻 2025-10-30
---
### PostgreSQL每周新闻#622 - 2025年10月30日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/622)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/fxxr7ew1lsnr4rl5kffr.jpg)
## [pgfeaturediff：比較 Postgres 版本之間的功能](https://postgresweekly.com/link/176351/web)
該網站基於 Postgres 官方功能矩陣，讓您可以輕鬆直接地比較兩個您選擇的 Postgres 版本之間的功能差異。

`Sebastian Steenssøe`

💡 [PG 版本報告](https://postgresweekly.com/link/176353/web_是一個類似的實用工具，您只需提供伺服器的版本字串，即可查看 CVE、錯誤、EOL 日期以及與 Postgres 17 的比較。


## [Agentic Postgres：在 Postgres 中原生建立 AI 應用程式](https://postgresweekly.com/link/176350/web)
Tiger Data 的全新 Agentic Postgres 將 AI 原生功能引入 Postgres，包括可 fork 的資料庫、內建記憶體、混合搜尋和代理 API。只需幾秒鐘即可建立零拷貝分支，安全地進行實驗。在 Tiger 上免費試用，無需信用卡。

`TigerData  `

## [📊 Kafka 速度很快，但我還是會用 Postgres](https://postgresweekly.com/link/176354/web)
受最近一篇關於用 Postgres 代替 Redis 的文章啟發，作者決定探究 Postgres 是否足以應對那些你通常會考慮使用 Kafka 的場景。

`Stanislav Kozlovski`

💡 這篇文章引發了 [Hacker News 今年關於 Postgres 最熱烈的討論之一](https://postgresweekly.com/link/176357/web)。


* 🇨🇭 [CERN PGDay 2026](https://postgresweekly.com/link/176358/web) 是一個 Postgres 主題活動，將於明年 2 月 6 日在日內瓦郊外舉行。徵稿截止日期為 12 月 7 日。

* 🇪🇺 Floor Drees 分享了她[上週參加 PGConf EU 活動的體驗](https://postgresweekly.com/link/176359/web)。

* 🎤 Talking Postgres 播客採訪了 Postgres 貢獻者 Andres Freund，探討了[在 Postgres 18 中實現非同步 I/O 時遇到的問題（以及成功之處！）](https://postgresweekly.com/link/176360/web)。

* 👥 Postgres 計畫[更新了其貢獻者頁面](https://postgresweekly.com/link/176361/web)，新增了[幾位貢獻者](https://postgresweekly.com/link/176362/web)，並將四位貢獻者晉升為主要貢獻者。


## [pg_textsearch：真正的 BM25 排名和混合檢索](https://postgresweekly.com/link/176363/web)
Tiger Data 對 ParadeDB 的 BM25 全文搜尋排名印象深刻，因此希望開發一款能夠在他們基於 Postgres 的系統上運行的類似工具。目前該工具僅在 Tiger Cloud 上提供預覽版，尚不確定未來是否會開源，但我們對此充滿期待。

`Green and Arye (Tiger Data)`


📄[使用 Postgres 擴充功能傳回多行資料](https://postgresweekly.com/link/176366/web) – 如果您正在開發自己的 Postgres 擴展，本文將對您有所幫助。作者：Shaun Thomas

📄 [Oracle 採用原生布林資料類型 vs. Postgres](https://postgresweekly.com/link/176367/web) – Oracle 終於獲得了 Postgres 幾十年來一直擁有的功能。作者：Pavan Chary

📄 [Postgres 18 的 UUIDv7：更快更安全的按時間順序排列的 ID](https://postgresweekly.com/link/176368/web)。作者：Vinicius Negrisolo


## **发布**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/jspdqcd32umpy3toq4r9.jpg)

## [PostgREST 14.0：適用於任何 Postgres 資料庫的 REST API](https://postgresweekly.com/link/176369/web)
一個流行且歷史悠久的 Haskell 伺服器，可為您選擇的 Postgres 資料庫提供 RESTful API。 v14.0 版本說明。

`Steve Chavez and Joe Nelson`

## **📰 分類廣告**

日本領先的 C2C 內容創作平台 [note.com](https://postgresweekly.com/link/176371/web) 如何以 JIT 存取控制取代其 GitHub Actions + SSH 代理流程，從而實現更安全的 Aurora Postgres 存取。

🌐 [憑藉數十年的 PostgreSQL 經驗，我們擁有專業的支援團隊，可自信地在任何規模下部署](https://postgresweekly.com/link/176372/web)。


## [pg_easy_replicate 0.4：以最小的停機時間切換資料庫](https://postgresweekly.com/link/176373/web)
一個基於 Ruby 的編排器，可簡化在兩個 Postgres 資料庫之間設定邏輯複製的任務，然後讓您以最小的停機時間切換到較新的資料庫。

`Shayon Mukherjee`


[TimescaleDB 2.23](https://postgresweekly.com/link/176374/web) – 為 Postgres 資料庫提供時間序列功能的擴充。現已全面支援 Postgres 18，預設啟用 UUIDv7 壓縮，並可將超表設定為不記錄日誌。

[WhoDB 0.66](https://postgresweekly.com/link/176375/web) – 適用於多個資料庫的輕量級新一代資料瀏覽器。

[PgDog 0.1.13](https://postgresweekly.com/link/176376/web) – 為 Postgres 資料庫提供自動分片的水平擴展功能。

[ChartDB 1.17](https://postgresweekly.com/link/176377/web) – 開源的基於圖表的資料庫編輯器。