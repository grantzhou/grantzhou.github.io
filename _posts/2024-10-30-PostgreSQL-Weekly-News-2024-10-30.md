---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-10-30
---
### PostgreSQL每周新闻#574 - 2024年10月30日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/574)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/azjqecondybgqptdvink.jpg)
## [pgdoc.link：一种搜索 Postgres 文档的新方法](https://postgresweekly.com/link/161574/web)
Hubert 一直在寻找一种方法来解决查找 Postgres 文档时出现的不一致问题 — 这就是结果。如果您要搜索的内容有一个单一的、规范的文档，您将直接进入该文档，否则您将看到一个帮助您解决歧义的页面（例如 *_connections）。这是一个好主意。

`Hubert 'depesz' Lubaczewski`
## [在 Postgres 中创建 Date Bin 的 4 种方法](https://postgresweekly.com/link/161577/web)
当您需要生成报告或以其他方式将数据打包到某些日期“箱”（例如整月、季度或一年）中时，Postgres 提供了几种方法来实现。Christopher 介绍了 INTERVAL、date_trunc、extract 和 to_char，每种方法都有其优缺点。


`Christopher Winslett `
## [如何比较 Postgres EXPLAIN 计划和调整慢速查询](https://postgresweekly.com/link/161573/web)
慢速 Postgres 查询是否会影响您的应用性能？参加此网络研讨会，了解如何有效地诊断和调整它们。我们将使用 pganalyze 来演示如何比较计划和调试常见场景，例如低效的嵌套循环和缺失索引。


`pganalyze `
## [优化“奇怪选择”错误计划的案例研究](https://postgresweekly.com/link/161578/web)
“我们最近遇到了一个有趣的案例，规划人员选择了错误的计划。有点。并认为它可以用于展示如何处理此类情况。”


`Hubert depesz Lubaczewski`

### 本周摘要：

△ Prisma 是快速发展的 Postgres 服务生态系统中的最新参与者，它推出了一种新的[即用即付平台 Prisma Postgres](https://postgresweekly.com/link/161579/web)。

🌐 [PostGIS Day 2024](https://postgresweekly.com/link/161580/web) 是一项免费的在线活动，将于 11 月 21 日举行，其时间表现已上线。

📄 PDF：[深入研究统计数据](https://postgresweekly.com/link/161581/web) - Louise Leinweber 在 PG Conf EU 上发表演讲的幻灯片。这是一个详尽的幻灯片，仅凭幻灯片就可以学到很多东西（但一旦上线，我们也会链接到视频）。

[🇨🇿 布拉格 PostgreSQL 开发者日](https://postgresweekly.com/link/161582/web) 2025 将于明年 1 月在捷克布拉格举行。[征文](https://postgresweekly.com/link/161583/web)截止日期为 11 月 23 日。

[🇺🇸 Postgres 会议](https://postgresweekly.com/link/161584/web) 2025 是一个为期四天的活动，将于明年 3 月在佛罗里达州奥兰多举行。论文征集截止日期为 1 月 27 日。

[David E. Wheeler 分享了上周 PGConf EU 和相关扩展生态系统峰会的一些最新消息](https://postgresweekly.com/link/161585/web)。


## [说方言：Postgres 和字符编码](https://postgresweekly.com/link/161586/web) 
谈到数据库时，字符编码可能是绝对“重要但我不想考虑”的话题。幸运的是，使用 UTF-8 可以让您获得最大的满足感。


`Christophe Pettus`
## [使用基于 CTID 的分页进行数据清理](https://postgresweekly.com/link/161587/web) 
CTID 字段对于表中的每一行都是唯一的，但不仅仅是简单的行 ID。它是一个结合了物理页面和行位置信息的元组，可以帮助您根据物理存储以可预测的块形式处理表。


`Shayon Mukherjee`
## [如何使用 OpenAI CLIP、Postgres 和 JavaScript 构建图像搜索应用程序](https://postgresweekly.com/link/161588/web) 
本教程将许多想法汇集在一起​​。CLIP 用于将图像转换为文本描述。Postgres 用作矢量数据库。JavaScript 为前端（使用 React）和后端（Node.js）提供了粘合剂。


`Haziqa Sajid`
## [Postgres 中的请求-回复](https://postgresweekly.com/link/161589/web) 
“前几天我在想，你是否可以使用普通的 Postgres 组件构建一个请求-回复机制。事实证明，你可以！至于是否应该这样做，就留给读者自己决定吧。”


`Anthony Accomazzo`


📄 [Postgres 的未来？扩展！](https://postgresweekly.com/link/161590/web) - Craig Kerstiens

📄 [使用 PostGIS 和 Overture 数据进行车辆路线规划](https://postgresweekly.com/link/161591/web) - Paul Ramsey



### 📰 分类广告

索引、数据类型或存储过程和函数有问题？[观看 Redgate 最新的 PG101 网络研讨会剧集](https://postgresweekly.com/link/161592/web)，了解技巧和窍门。

[Google 如何大规模处理授权](https://postgresweekly.com/link/161593/web)。Google 基于关系的授权系统与 Oso 的授权即服务的技术比较。

### 🛠 代码和工具

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/lxmkxjtoljuznvddof7h.jpg)

## [Postgres 版本报告](https://postgresweekly.com/link/161594/web)
一个在线工具，您可以在其中粘贴 Postgres 服务器的完整版本信息，并了解其与 Postgres 发布时间表、未解决的 CVE、错误以及后续版本中的改进之间的关系。


`Neon`
## [pg_duckdb：由 DuckDB 提供支持的 Postgres，用于高性能分析](https://postgresweekly.com/link/161603/web)
官方 Postgres 扩展（与 Hydra 和 MotherDuck 合作构建），将 DuckDB 的列式矢量化分析引擎和功能嵌入到 Postgres 中。


`DuckDB`

## [pg_parquet：用于连接 Postgres 和 Parquet 的扩展](https://postgresweekly.com/link/161595/web)
用于处理 Parquet 文件的新开源扩展。它直接从 Postgres 读取 parquet 文件并将其写入本地磁盘（或 S3）。GitHub 存储库。


`Craig Kerstiens`

[pgroll 0.7](https://postgresweekly.com/link/161601/web) – 适用于 Postgres 的零停机模式迁移工具。

[pgenv 1.3.8](https://postgresweekly.com/link/161602/web) – PostgreSQL 二进制管理器。