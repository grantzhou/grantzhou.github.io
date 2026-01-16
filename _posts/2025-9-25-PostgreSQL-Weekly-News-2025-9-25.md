---
layout: post
title: PostgreSQL 每周新闻 2025-9-25
---
### PostgreSQL每周新闻#617 - 2025年9月25日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/617)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/iosout28y26yrnqummvo.jpg)
## [Postgres 18 發布](https://postgresweekly.com/link/174773/web)
Postgres 的最新主要版本如期發布。它並非 Postgres 史上最大的進步之一，但卻包含許多顯著的改進，可以提升資料庫的效能。以下是一些新功能：

* 引進[非同步 I/O 子系統](https://postgresweekly.com/link/174740/web)，實現更有效率的掃描、清理等功能。
* 支援 [UUIDv7](https://postgresweekly.com/link/174741/web)，並新增[多項功能](https://postgresweekly.com/link/174742/web)。
* [UPDATE...RETURING](https://postgresweekly.com/link/174743/web)功能顯著改善。
* [支援並行應用大型事務](https://postgresweekly.com/link/174744/web)。
* [OAuth 2.0 授權和身份驗證](https://postgresweekly.com/link/174745/web)。

💡 如果您想要所有新功能的完整列表，[發行說明](https://postgresweekly.com/link/174746/web)提供了詳盡的要點演練。

## [首期專為產品工程師打造的簡報](https://postgresweekly.com/link/174737/web)
《產品工程師》是 PostHog 的簡報，致力於幫助工程師提升產品技能。它涵蓋了工程師在建立 PostHog 流程中的經驗、對頂級新創公司的研究，以及打造優秀產品的精選建議。

`PostHog   `

## [PlanetScale for Postgres 現已正式發布](https://postgresweekly.com/link/174747/web)
今年 7 月，以 MySQL 服務聞名的雲端資料庫平台 PlanetScale 宣布將進軍 PG 領域，並分享了一系列基準測試，以展示其解決方案與其他同類產品相比的優勢。此前，該服務一直處於「私人預覽」階段，現已向所有人開放。

`Sam Lambert`

💡 值得注意的是，[Hacker News 上對此消息的評論非常積極](https://postgresweekly.com/link/174749/web)，許多早期用戶都對這項服務表示稱讚。


### **本周摘要**

* 伊麗莎白·克里斯滕森 (Elizabeth Christensen) 查閱了 [1986 年 Postgres 的原始設計目標論文](https://postgresweekly.com/link/174750/web)，並得出[結論：“PostgreSQL 的創建者完全做到了這一點](https://postgresweekly.com/link/174751/web)。”

* IEEE 發布了 [2025 年頂級程式語言榜單](https://postgresweekly.com/link/174752/web)，SQL 位列第四。

* 本·迪肯 (Ben Dicken) [製作了一個可視化的進程和線程解釋器](https://postgresweekly.com/link/174753/web)，對 Postgres 和 MySQL 的方法進行了比較。

* Red Gate 正在進行其[最新的資料庫現況調查。更多資訊請點擊此處](https://postgresweekly.com/link/174754/web)。


## [Postgres 18 中非同步 I/O (AIO) 的調優](https://postgresweekly.com/link/174756/web)
Postgres 18 最引人注目的變化之一是引入了非同步 I/O（又稱 AIO，您可以點擊此處了解更多資訊）。 Tomas 將介紹引入的新配置設置，這些設置會影響 AIO 的工作方式和擴展方式。


`Tomas Vondra`

📄 [Redis 速度很快 - 我會用 Postgres 做cache](https://postgresweekly.com/link/174758/web) – 比較 Postgres 和 Redis 的基本快取任務。 Redis 速度更快，但不一定快到值得運行第二個系統，這取決於您的設定。 Viktoras Kuznecovas

📄 [一週只寫文件](https://postgresweekly.com/link/174759/web) – PgDog Postgres 連接池和分片器的創建者真的非常重視文件。 Lev Kokotov

📄 [Postgres 分區最佳實踐](https://postgresweekly.com/link/174761/web)：Sofia 的故事 Karen Jex

📄 [理解 WAL 並使用專用磁碟對其進行最佳化](https://postgresweekly.com/link/174762/web) Warda Bibi


## **发布**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/c2401vxr0z16de9mqvp2.jpg)

## [pgschema：Postgres 的聲明式模式遷移](https://postgresweekly.com/link/174763/web)
想像一下類似 Terraform 的東西，但將宣告式模式遷移工作流程引入 Postgres。它提供了許多功能，並支援許多高級功能——GitHub 倉庫。

`Tianzhou et al.`

## [pgAudit 18.0：稽核日誌擴展](https://postgresweekly.com/link/174766/web)
Postgres 18 支援此擴展，用於產生可能需要遵守政府、財務或 ISO 認證的稽核日誌。

`PostgreSQL Global Development Group`

## [pgexporter 0.7：適用於 Postgres 的 Prometheus 導出器](https://postgresweekly.com/link/174767/web)
現已改善核心指標，包括新增的 autovacuum 指標，並新增對 PostGIS、pg_stat_statements、pgvector 和 Timescale 等多個擴充功能的支援。主頁。

`pgexporter community`


[DoltgreSQL 0.52](https://postgresweekly.com/link/174769/web) – 類似 Postgres 的版本控制，具有類似 Git 的功能。

[BemiDB 1.6](https://postgresweekly.com/link/174770/web) – 針對分析最佳化的單二進位 Postgres 唯讀副本。

[pgFormatter 5.8](https://postgresweekly.com/link/174771/web) – SQL 程式碼格式化程式和美化器。

[pgenv 1.4.3](https://postgresweekly.com/link/174772/web) – Postgres 二進位檔案管理器。