---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-10-16
---
### PostgreSQL每周新闻#574 - 2024年10月16日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/574)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/q2dcgl4uk6v6jfvnbiwt.jpg)
## [使用 JSON_TABLE 将 JSON 转换为列和行](https://postgresweekly.com/link/161088/web)
新的 Postgres 17 功能提醒！JSON_TABLE 是一种函数，可让您查询 JSON 数据并在典型的关系视图中获取结果。Paul 向我们展示了一个实际用例。

`Paul Ramsey`
## [SQL/JSON 来了（某种程度上！）](https://postgresweekly.com/link/161090/web)
JSON_TABLE（上文）很棒，但只是 SQL/JSON 体验的一部分。SQL/JSON 是一个广义术语，指的是用于处理 SQL 中的 JSON 数据的路径语言、查询函数和运算符，在这里我们可以看到 Postgres 17 为 JSON 表带来的更多内容。


`Hubert depesz Lubaczewski `
## [使用此月度检查清单主动提高 Postgres 性能](https://postgresweekly.com/link/161087/web)
掌握 PostgreSQL 维护的最新情况可能具有挑战性。我们的月度检查清单将指导您完成关键任务，以快速有效地保持性能、可靠性和正常运行时间。立即下载您的免费检查清单。


`pganalyze `
## [触发器递归及其处理方法](https://postgresweekly.com/link/161091/web)
如果您设置了一个触发器，而该触发器的行为会导致触发同一个触发器，那么您将面临许多潜在的调试难题。幸运的是，调整触发器以使其仅在预期时运行并不困难。


`Laurenz Albe`

### 本周摘要：

* 🎤 Talking Postgres 播客采访了[] Postgres 贡献者 Tom Lane](https://postgresweekly.com/link/161092/web)，了解了他如何进入编程领域、Postgres 核心团队的工作方式等。

* 📺 Aaron Francis 终于推出了他的大型 [Mastering Postgres 视频课程](https://postgresweekly.com/link/161093/web)。这需要付费，但前 25 个视频是免费的，只需提供电子邮件地址即可观看。

* 🇬🇷 下周，[欧洲 Postgres 生态系统峰会](https://postgresweekly.com/link/161094/web)将在雅典举行（恰逢 2024 年欧洲 PostgreSQL 会议的开始）。

* 🇩🇪 Andreas Scherbaum 分享了 [PostgreSQL Berlin 最近聚会的最新消息](https://postgresweekly.com/link/161096/web)。

* 🇳🇱 与此同时，[Pavlo Golub 分享了上个月 PGDay Lowlands 2024 的进展情况](https://postgresweekly.com/link/161097/web)。


## [pg_dump 是一个“备份”工具吗？](https://postgresweekly.com/link/160798/web) 
—我曾经使用 pg_dump 进行备份，你也许也用过，但文档似乎热衷于强调它实际上是一种导出工具。Robert 思考了这一说法。


`Robert Haas`


📄 [您注意到 Postgres 的增强版发行说明了吗？](https://postgresweekly.com/link/161100/web) - Greg Sabino Mullane

📄 [调整 glibc 内存分配器（用于 Postgres）](https://postgresweekly.com/link/161101/web) - Tomas Vondra



### 📰 分类广告

[参加 Redgate 10 月 29 日的网络研讨会](https://postgresweekly.com/link/161102/web)，了解 PostgreSQL 和 SQL Server 之间存储过程和函数的惊人差异。

🧰 PostgreSQL 是 AI 所需的一切。使用 [pgvectorscale](https://postgresweekly.com/link/161103/web) 可实现 28 倍更快的搜索速度，比流行的向量数据库便宜 75%。

✨ [Kestra 可自动执行整个工作流程编排](https://postgresweekly.com/link/161104/web)，包括 ETL 和实时数据处理。轻松跨 Postgres 和云堆栈进行扩展。


### 🛠 代码和工具

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/aijivbzv57ibiilnxehn.jpg)

## [Postgres 类型浏览器：查看各种用例的数据类型](https://postgresweekly.com/link/161105/web)
作为 Mastering Postgres 发布的一部分，Aaron Francis 推出了一款在线工具，该工具可针对不同情况（例如存储哈希、金额、UUID、二进制数据）提供使用哪种数据类型的建议。它还提供了每种数据类型可使用的存储空间大小的指示。


`Aaron Francis`
## [PGroonga：将全文搜索功能扩展到所有语言](https://postgresweekly.com/link/161106/web)
将 Groonga 全文搜索引擎引入 Postgres，它比 Postgres 默认的搜索引擎更适合某些用例，例如日语或中文。现在从 v3.2.4 开始支持 Postgres 17。


`PGroona Project`

## [Greenmask：Postgres 数据屏蔽和混淆工具](https://postgresweekly.com/link/161108/web)
种由 Go 提供支持的实用程序，用于转储 Postgres 数据库并以确定性方式匿名化数据。GitHub 存储库。


`Greenmask`

[pgrx 0.12.6](https://postgresweekly.com/link/161110/web) – 一种使用 Rust 构建 Postgres 扩展的方法。

[tbls 1.78](https://postgresweekly.com/link/161111/web) – 自动以 Markdown 格式记录数据库。

[Prisma 5.21](https://postgresweekly.com/link/161112/web) – 适用于 Node.js 和 TypeScript 的流行 ORM。

[SeaORM 1.1](https://postgresweekly.com/link/161113/web) – 适用于 Rust 的动态异步 ORM。

[ParadeDB 0.11](https://postgresweekly.com/link/161114/web) – 用于搜索和分析的 Postgres。

[pg-promise 11.10](https://postgresweekly.com/link/161115/web) – 适用于 Node.js 的 Postgres 接口。