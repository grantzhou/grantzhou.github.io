---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2023-1-11
---
### PostgreSQL每周新闻#488 - 2023年1月11日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/488)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,w_430,h_100/e_make_transparent/co_white,e_outline:7/xyflkz7n00elwtgja9ne.png)
## [Supabase Wrappers：一个用 Rust 编写的 FDW 框架](https://postgresweekly.com/link/133810/web)
外部数据包装器 (FDW) 在 Postgres 中提供了一种机制来访问远程/外部系统上的数据，无论是其他 SQL 数据库还是平面文件。 Supabase 构建了 Wrappers，试图将无数的 FDW 集中在一个屋檐下（已经包括与 Stripe、Firebase 和 Airtable 集成的 FDW），并使其更容易构建更多。


`None`
## [❤️ Postgres](https://postgresweekly.com/link/133809/web)
您需要一个像您一样热爱 Postgres 的数据库提供商。 我们会处理所有麻烦 - 监控、备份、HA、灾难恢复，因此您不必这样做。 想要惊人的支持？ 当您有问题时，我们会在场。


`Crunchy Bridge `
## [更快的 PostgreSQL 到 BigQuery 传输](https://postgresweekly.com/link/133812/web)
作者以其 "11 亿次出租车出行" 数据库基准测试而闻名，演示了如何使用 ClickHouse 将 Postgres 表导出到 Parquet 以便导入到 BigQuery 比使用压缩的 CSV 更快。 一篇非常实用的文章，特别是从事 GIS 工作的任何人都会感兴趣。


`Mark Litwintschik `
## [Postgres 世界 2022 年的简短总结](https://postgresweekly.com/link/133813/web)
早在 12 月，我们就 Postgres Weekly in 2022 发表了最好的一期，但 Avinash 对去年 Postgres 发生的事情进行了更面向新闻的审视，包括其数据库引擎排名、版本、品牌 新的扩展和安全漏洞。


`Avinash Vallarapu `
## [查看 Postgres 中的索引类型](https://postgresweekly.com/link/133818/web)
介绍 Postgres 使用的常见索引类型的简单入门，包括 B-Trees、GIST、GIN 和 BRIN 索引。


`Grant Fritchey `
## [在 AWS 上从 Postgres 生成 Excel 工作簿](https://postgresweekly.com/link/133819/web)
一个明显具有 AWS 风味的方法，用于通过 AWS Lambda 和 S3 从 Postgres（包括 RDS 和 Aurora）提取数据到 Excel 工作簿。


`Shaik, Chintha, and Agarwal (AWS) `
## [免费电子书下载：了解 Kubernetes（更新版）](https://postgresweekly.com/link/133820/web)


`Linode `
## [Oracle 和 Postgres 之间的 SUBSTR 功能差异](https://postgresweekly.com/link/133821/web)
如果您参与迁移，这很有价值。


`Deepak Mahto `
## [pg_rowalesce：行合并](https://postgresweekly.com/link/133824/web)
rowalesce() 类似于 coalesce()，但用于行和其他复合类型。


`Rowan Rodrik van der Molen `
## [PL/Haskell 1.1：在 SQL 函数中使用 Haskell](https://postgresweekly.com/link/133825/web)
过程性的，符合功能性的。

`Ed Behn `
## [sqld：libSQL/SQLite 的“服务器模式”](https://postgresweekly.com/link/133826/web)
这有点不寻常。 这不是在另一个数据库前面使用 Postgres 的有线协议，这本质上是在 Postgres 有线协议前面的 SQLite（这个想法是使用 SQLite 的应用程序 - 或者它的 libSQL 分支，无论如何 - 可以继续像他们已经做的那样， 但实际上在幕后使用 Postgres）。


`libSQL `
