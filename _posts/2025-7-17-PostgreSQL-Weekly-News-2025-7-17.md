---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-7-17
---
### PostgreSQL每周新闻#608 - 2025年7月17日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/608)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/sevyutm3vm21r3kje9lj.jpg)
## [📊 Xata 对 PlanetScale 的 Postgres 基准测试的反应](https://postgresweekly.com/link/171884/web)
PlanetScale 进军 Postgres 领域引发了广泛关注，其他供应商也纷纷对其基准测试结果进行仔细审查。另一个主流平台 Xata 则对 PlanetScale 的方法论进行了分析，并运行了自己的基准测试，并强调了在考虑所有变量的情况下进行准确、公平的基准测试所面临的挑战。

`Tudor Golubenco (Xata)`

💡 Neon 的人们也研究了 PlanetScale 的基准并展示了其[特定额外缓存层的影响](https://postgresweekly.com/link/171886/web)。


## [Rocketadmin：后台的瑞士军刀](https://postgresweekly.com/link/171883/web)
了解我们开源、灵活且安全的管理面板服务，以及如何将其集成到您的工作流程中。您可以为用户授予严格的权限，创建自动化功能和 UI 小部件，并使用 AI Insights 探索您的数据库。


`Rocketadmin `

## [LISTEN/NOTIFY 无法扩展](https://postgresweekly.com/link/171887/web)
虽然 LISTEN/NOTIFY 很有趣，但我从未想过使用它——与通常的查询→结果方法相比，这种机制感觉不太方便。本文探讨了锁争用带来的扩展问题，但这并没有改变我的想法。

`Elliot Levin `

## [Postgres 每秒数十亿条边的计算](https://postgresweekly.com/link/171889/web)
OneSparse 简介，它是 Postgres 的一个扩展，使用 SuiteSparse 的 GraphBLAS 库将表转换为高性能稀疏矩阵，并转换回原形，无需外部图数据库。需要一些解释才能理解，但幸运的是，Michel 对此进行了深入的讲解。

`Michel Pelletier`

### **本周摘要**

* [💰 ParadeDB 已完成 1200 万美元的 A 轮融资](https://postgresweekly.com/link/171890/web)。他们最知名的产品是 [Postgres 全文搜索扩展](https://postgresweekly.com/link/171891/web)。

* [Dian Fay](https://postgresweekly.com/link/171892/web) 是最新一期《PostgreSQL 本周人物》的受访者。她是 pdot 的创建者（详见下文）。

* 🎤 [Talking Postgres 播客节目采访了微软的 Shireesh Thota](https://postgresweekly.com/link/171894/web)，内容涵盖了他在微软的职业生涯、微软对 Postgres 的贡献，以及在 Azure 期间同时使用多个数据库系统（附完整文字记录）。

* 📈 [PGlite](https://postgresweekly.com/link/171896/web) 是 Postgres 的可嵌入 WebAssembly 版本，目前[每周下载量超过一百万次](https://postgresweekly.com/link/171897/web)。

* 🇦🇺 [PG Down Under 2025](https://postgresweekly.com/link/171898/web) 将于今年十月在澳大利亚举行。

📄 [Postgres 存储选项比较](https://postgresweekly.com/link/171899/web) – 快速比较标准行存储、列存储、CSV 和 Parquet。Hans-Jürgen Schönig

⚙️ [stripe-sync-engine](https://postgresweekly.com/link/171900/web)：一个独立的 Stripe-To-Postgres 同步引擎库 Kevin Grüneberg (Supabase)

📄 [修复缓慢的行级安全策略](https://postgresweekly.com/link/171901/web) Dian Fay


### **🛠 代码和工具**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/lxj87wujsyn2zhikvl0v.jpg)

## [pdot：数据库的交互式有向图](https://postgresweekly.com/link/171893/web)
一种生成 GraphViz 或 Mermaid 定义的工具，用于呈现图表，展示 Postgres 数据库中的各种内容，例如表关系、外键图、触发器和函数、RLS 策略关系等。

`Dian Fay`


## [Odyssey 1.4：可扩展的 Postgres 连接池](https://postgresweekly.com/link/171902/web)
一个生产就绪、仅适用于 Linux 的连接池和 Yandex 的请求路由器。v1.4 专注于修复和稳定性 - 还有一个新的 Telegram 聊天室提供支持。


`Yandex`

## [pgsqlite：用于 SQLite 数据库的 Postgres 协议适配器](https://postgresweekly.com/link/171595/web)
一种让 Postgres 客户端能够像连接 Postgres 数据库一样连接并查询 SQLite 数据库的方法。目前处于“实验阶段”。

### **📰 分类广告**

🐘 [Atlas](https://postgresweekly.com/link/171904/web) 管理 Postgres，就像 Terraform 管理基础设施一样。将模式定义为代码，并安全地规划和应用迁移。了解更多。

💌 您知道我们有一系列新闻简报吗？查看 [JavaScript 周刊](https://postgresweekly.com/link/171905/web)、[Go 周刊](https://postgresweekly.com/link/171906/web)和 [Ruby 周刊](https://postgresweekly.com/link/171907/web)，更全面地了解我们的工作。

## [Endor：添加服务（例如 Postgres）作为节点依赖项](https://postgresweekly.com/link/171908/web)
一项新颖的尝试，只需简单的 npm install 和 endor run 即可快速启动沙盒环境和服务器，涵盖 Postgres、MariaDB 和 Valkey 等服务。

`Angel M Miguel (Endor)`

## [Redka：用 SQL 重新实现的 Redis](https://postgresweekly.com/link/171908/web)
一个基于 Go 的数据存储，兼容 Redis 的 API，但在后台使用 SQL 来实现所有功能。之前它基于 SQLite，但 v0.6 引入了对 Postgres 的支持。

`Anton Zhiyanov`

[FerretDB 2.4](https://postgresweekly.com/link/171911/web) – 一款功能类似于 MongoDB 的数据库，但使用 Postgres 进行存储。

[QuestDB 9.0](https://postgresweekly.com/link/171912/web) – 基于 Java 的时间序列数据库，兼容 Postgres 有线协议。现已支持真正的 N 维数组，并改进了物化视图。

🤖 [pgai 0.11](https://postgresweekly.com/link/171913/web) – Timescale 的工具，可在 Postgres 中使用 RAG 和 LLM。

[qsv 6.0](https://postgresweekly.com/link/171914/web) – 用于查询、切片、过滤、转换、排序和转换表格数据的命令行工具。

[Squawk 2.20](https://postgresweekly.com/link/171915/web) – 用于 Postgres 迁移和 SQL 的 Linter。

[PostgreSQL Anonymizer 2.3](https://postgresweekly.com/link/171916/web)

[OrioleDB Beta 12](https://postgresweekly.com/link/171917/web)