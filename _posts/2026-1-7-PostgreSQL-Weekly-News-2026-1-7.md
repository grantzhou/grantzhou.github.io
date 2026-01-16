---
layout: post
title: PostgreSQL 每周新闻 2026-1-7
---
### PostgreSQL每周新闻#629 - 2026年1月7日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/630)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/hsvy3genjwv9bfv9klsi.jpg)
## [2025 年数据库展望：年度回顧](https://postgresweekly.com/link/178895/web)
備受尊敬的数据庫專家 Andy Pavlo 精心撰寫了一篇精彩的文章，回顧了過去一年資料庫領域的主要趨勢和動態。 Postgres 被譽為 2025 年的「主導」資料庫，但文章內容遠不止於此。

`Andy Pavlo`

## [POSETTE 2026－提案徵集即將截止！](https://postgresweekly.com/link/178894/web)
新年新目標！誠摯邀請您在 POSETTE（Postgres 盛會）上分享您的 Postgres 真知灼見。 POSETTE 是由微軟 PostgreSQL 團隊組織的免費線上開發者盛會，將於 2026 年 6 月 16 日至 18 日舉行。提案徵集將於 2 月 1 日截止。立即行動！

`Microsoft `


## **本周摘要**

🇨🇭 [CERN PGDay 2026](https://postgresweekly.com/link/178898/web) 將於今年 2 月 6 日在瑞士舉行，完整行程已公佈。

[Postgres 團隊表彰](https://postgresweekly.com/link/178900/web)了 12 位對專案做出傑出貢獻的新成員，並宣布 Floor Drees 加入貢獻者團隊，「以幫助分擔工作量」。

## [Postgres 效能：雲端和本地部署的延遲](https://postgresweekly.com/link/178901/web)
擁有高效能資料庫是一回事，但資料庫的位置對延遲有很大的影響 — 如果延遲過高，可能會抵消其他所有效能優勢。

`Hans-Jürgen Schönig`

## [Postgres 18 的 RETURNING 增強功能](https://postgresweekly.com/link/178902/web)
Postgres 18 增強了 DML 查詢（插入、更新等）中使用的 RETURNING 子句，以支援舊別名和新別名，從而明確存取資料的先前狀態和目前狀態。

`Ahsan Hadi`

## [pg_csv_loader：一款用於快速簡單地載入 CSV 檔案的工具](https://postgresweekly.com/link/178903/web)
一款基於 JavaScript 的工具，只需極少的配置即可將 CSV 檔案載入到 Postgres 資料庫中。來源。

`Hubert depesz Lubaczewski`


📄 [使用 Postgres 18 快速複製資料庫 – 利用範本資料庫](https://postgresweekly.com/link/178905/web)。 Radim Marek

📄 [幾個 Postgres 腳本編寫技巧](https://postgresweekly.com/link/178907/web)。 Paul Gross

📄 [2025 年 Postgres MCP 伺服器的現況](https://postgresweekly.com/link/178908/web)。 DBHub


## **📰 分類廣告**


🚀 [將 AI 代理部署到生產環境](https://postgresweekly.com/link/178909/web)。 Postgres 工具包，支援 MCP、混合搜尋和全球擴充。 [Beta 版現已開放](https://postgresweekly.com/link/178909/web)。

## **🐘 2025 年 Postgres 每週熱門文章：**

[在 2025 年最後一期中](https://postgresweekly.com/link/178910/web)，我們回顧了過去一年中最熱門的工具和程式碼，但這裡我們更全面地審視一下過去十二個月中最受關注的內容。這是一份值得重溫的精華清單：

## [1. 改變人生的 Postgres 模式](https://postgresweekly.com/link/178911/web)
作者承諾標題並非譁眾取寵（雖然顯然效果顯著，排名第一！），書中提供了十二條精煉實用、來之不易的技巧和見解，涵蓋了從使用 UUID 作為主鍵、表命名到模式和視圖的使用等各個方面。

`Ethan McCue`


## [2. 不要這樣做（在 Postgres 中）](https://postgresweekly.com/link/178912/web)
Postgres 官方 wiki 上的一個頁面一直都很有意思，它匯總了使用 Postgres 時常見的錯誤以及不應該做的事情，例如“不要使用 char(n)”和“不要使用 serial”。有些建議可能有爭議，但都給了理由。

`Postgres Wiki`


## [3. Kafka 速度很快，我會使用 Postgres](https://postgresweekly.com/link/178913/web)
受另一篇關於使用 Postgres 而不是 Redis 進行緩存的文章的啟發，作者開始研究 Postgres 是否足以處理你可能自然而然選擇 Kafka 的用例。

`Stanislav Kozlovski`


## [4. 如何修復 Postgres 中查詢速度慢的常見原因](https://postgresweekly.com/link/178916/web)
Render 的一位資料庫工程師展示了一個常見的、但很容易修復的效能問題，該問題是由外鍵上缺少索引引起的。

`Eric Fritz`


## [5. 將 Postgres 隊列擴展到每秒 10 萬個事件的經驗教訓](https://postgresweekly.com/link/178917/web)
RudderStack 決定使用 Postgres 作為其主要隊列系統，而不是 Kafka 之類的系統，他們的團隊分享了他們從中獲得的經驗教訓。

`Aris Tzoumas (RudderStack)`

## [6. Postgres 17 與 18 的基準測試](https://postgresweekly.com/link/178918/web)
作者對 Postgres 17 和 18 進行了一系列詳細的性能基準測試，測試組合多達 96 種，結果令人欣慰地發現 Postgres 18 提供了不錯的性能提升，本地磁碟性能更佳，調整設置仍然值得。

`Ben Dicken (PlanetScale)`

## [7. Citus 能容納 1 兆行嗎？](https://postgresweekly.com/link/178919/web)
“Postgres 可以擴展”，但究竟能擴展到什麼程度呢？ Hans-Jürgen 決定一探究竟，他進行了一項小型（或大型？）實驗，看看 1 兆行的表是否真的可行。

`Hans-Jürgen Schönig`

## [8. 即使你正在執行索引掃描，也不意味著你不能做得更好](https://postgresweekly.com/link/178920/web)
邁克爾說，如果你在查看查詢計劃時看到索引掃描，你可能會認為你正在朝著高性能查詢的方向前進，但還有更多提升空間。

`Michael Christofides`

## [9. Postgres 18 中的 psql 引入了管線功能](https://postgresweekly.com/link/178921/web)
Postgres 18 及更高版本中的 psql 配備了在 SQL 腳本中使用管線的命令，Daniel 指出這「可以大大提高查詢吞吐量」。

`Daniel Vérité`

## [10. PostgreSQL 在硬體怪獸時代](https://postgresweekly.com/link/178922/web)
你可能覺得工作站的 CPU 已經很快了，但想像一下，如果擁有一顆每個插槽 192 個核心的 AMD EPYC 處理器，以及 10 TB 的記憶體呢！現代 CPU 的強大效能（更不用說速度更快的儲存空間了）促使我們思考如何以現代方式擴展資料庫伺服器。

`Lætitia Avrot`