---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-10-23
---
### PostgreSQL每周新闻#621 - 2025年10月23日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/621)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/zktpbzsf69swswdqb4nc.jpg)
## [你的资料库是读重还是写重？](https://postgresweekly.com/link/175714/web)
大多数资料库的读取操作往往比写入操作更重，但这取决于你的工作负载。这值得确定吗？在调优方面，答案是肯定的。 David 展示了一个史诗级的 SQL 查询，它能帮你计算出表格的读写比。

`David and Elizabeth Christensen`

💡 上面帖子中的查询工作正常，但如果您还想包含只读或写的表，请将第 19 行的 AND 更改为 OR。

## [Tiger Lake：连接 Postgres 和 Lakehouse](https://postgresweekly.com/link/176013/web)
Tiger Lake 将 Postgres 与您的 Lakehouse 即时统一。无需管道，无需编排。使用开放格式持续串流、分析和提供资料。基于一个整合的 Postgres 原生架构，建立仪表板、代理程式和分析工具。

`TigerData  `

## [Tiger Data 推出免费 Postgres 计划](https://postgresweekly.com/link/175385/web)
Tiger Data（前身为 Timescale）提供 Postgres 平台已有一段时间，但从未推出免费套餐。现在，您可以免费获得最多两项服务，每项服务最高可提供 750MB 的储存空间。鉴于目前的行业现状，该计划主要面向 AI 和代理开发人员，但任何人都可以将其用于小型专案或实验。

`TigerData`

💡 Aiven, Neon 和 Supabase 等其他供应商也提供类似的免费套餐。

## [🔎 Postgres 中的混合搜寻：缺少的手册](https://postgresweekly.com/link/176019/web)
解释在相关性排名方面，使用 BM25 评分的全文搜寻（由 ParadeDB 提供支援）与向量相似性搜寻（由 pgvector 提供支援）相结合如何胜过 Postgres 的本机全文搜寻。

`James Blackwood-Sewell`

## [DESCending 索引的优势](https://postgresweekly.com/link/176021/web)
“索引定义中 DESC 子句的常见用例是支援混合 ORDER BY 子句。但在某些情况下，PostgreSQL 可以更有效率地填入降序索引，并且对降序索引进行正向扫描的效能可能优于对升序索引进行反向扫描。”

`Laurenz Albe`

## [▶ 速度提高 14 倍，运算量减少 12 倍：有时 Postgres 确实是您所需要的一切](https://postgresweekly.com/link/176022/web)
James 的团队如何从不可靠的 12 台伺服器 HBase/OpenTSDB 丛集转变为使用 Postgres/Timescale 处理时间序列工作负载且正常运行时间达到 100% 的两台伺服器。

`James Udiljak`

📄 [在 Windows 上为 Postgres 18 进行便携式设定 – 简易指南](https://postgresweekly.com/link/176023/web)。 Mohit Sindhwani

📺 [正确设定 Postgres 参数，防止效能低落 – 一小时网路研讨会录影](https://postgresweekly.com/link/176024/web)。 Greg Dostatni

📄 [PostGIS 效能：pg_stat_statements 和 Postgres 调优](https://postgresweekly.com/link/176025/web) Paul Ramsey


## **发布**

## [NoraSearch：快速查找子字串匹配偏移量和计数的扩展](https://postgresweekly.com/link/176026/web)
例如，在"abracadabra"中搜寻"abra"将传回 {0,4},{7,4}。作者引用了一个用于分析 DNA 序列的用例。

`Lemmer EL ASSAL`

## [pg_ivm 1.13：增量视图维护 (IVM) 扩充 -](https://postgresweekly.com/link/176027/web)
一种更有效的增量更新物化视图的方法，仅套用更改，而不是像 REFRESH MATERIALIZED VIEW 那样完全重新计算视图。 v1.13 增加了对外连接的支援。

`IVM Development Group`

## [PL/Haskell 5.0：在您的 SQL 函数中使用 Haskell](https://postgresweekly.com/link/176028/web)
Haskell 是一种函数式语言，而不是过程式语言，但您仍然可以使用它以 Postgres 可以使用的方式定义流程。 v5 增加了对日期和时间类型的支援。

`Edward F. Behn, Jr.`


[pgwire 0.34](https://postgresweekly.com/link/176029/web)– 使用 Rust 函式库实作的 Postgres 连线协定。

[pg_dbms_errlog v2.2](https://postgresweekly.com/link/176030/web) – 用于模拟 Oracle DBMS_ERRLOG 的扩充。

[postgres-meta 0.93](https://postgresweekly.com/link/176031/web) – 用于管理 Postgres 的 RESTful API。

[Squawk 2.29](https://postgresweekly.com/link/176032/web) – 用于 Postgres 迁移和 SQL 的 Linter。

[pgAdmin 4 v9.9](https://postgresweekly.com/link/176033/web) – 流行的 Postgres 管理工具。