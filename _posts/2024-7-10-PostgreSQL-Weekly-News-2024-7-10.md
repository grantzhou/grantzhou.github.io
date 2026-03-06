---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-7-10
---
### PostgreSQL每周新闻#556 - 2024年7月10日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/562)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/yqiptwwohrd7ygfo38of.jpg)
## [pgPedia：Postgres 百科全书](https://postgresweekly.com/link/157419/web)
一本有趣、格式清晰的 wiki 式参考指南，介绍了 Postgres 的功能和设置，是对官方文档的良好补充。值得仔细研究一下。

`POSTGRESPEDIA `

## [🎧 向 Talking Postgres 播客问好](https://postgresweekly.com/link/157420/web)
Path to Citus Con 播客旨在通过采访演讲者和其他 Postgres 名人来推广 Citus Con（现为 POSETTE），但总体而言已成为一款出色的 Postgres 播客。为了反映这种增长，它进行了品牌重塑。


`CLAIRE GIORDANO (MICROSOFT) `
## [Postgres 中的并行查询](https://postgresweekly.com/link/157422/web)
Postgres 并未大力支持并行运行查询的各个部分（又称并行查询），因此该功能很容易被忽视。Elizabeth 为我们提供了快速入门指南。


`ELIZABETH CHRISTENSEN  `
## [查看 Postgres 17 中的新内置排序规则提供程序](https://postgresweekly.com/link/157059/web)
Postgres 17 beta 版中有一个内置的 UTF-8 语言环境和排序规则提供程序，带有二进制字符串比较功能。下面介绍它为什么有趣、如何使用它以及它的性能。


`DANIEL VÉRITÉ  `
## [窗口函数的简单介绍](https://postgresweekly.com/link/157424/web)
一个良好、紧凑的介绍，重点关注要点。


`RADIM MAREK `

### 本周摘要：

我们最近写了一篇关于 Robert Haas 为 Postgres 贡献者提出的[指导计划](https://postgresweekly.com/link/157425/web)的文章，他对此进行了[更新](https://postgresweekly.com/link/157426/web)。有 34 人申请了这 14 个名额，但 Robert 为任何有兴趣为 Postgres 做出贡献的人创建了一个 Discord 服务器，以便他们交流并获得帮助。

[Highgo 的 Grant Zhou](https://postgresweekly.com/link/157427/web) 是本周 PostgreSQL 人物的受访者。

日历上又增加了一项新的欧洲 Postgres 活动！[PGDay Lowlands](https://postgresweekly.com/link/157428/web)。它将于今年 9 月在阿姆斯特丹举行。

## [Crunchy Bridge 将 Iceberg 添加到 Postgres](https://postgresweekly.com/link/157429/web)
Crunchy Data 已扩展其 Crunchy Bridge for Analytics 平台，支持查询 Iceberg 表，并具有完整的查询下推和强大的写入缓存功能。（Iceberg 是一种专门用于大型分析数据集的表格格式。）


`MARCO SLOT (CRUNCHY DATA) `

📄 Postgres 中[审计和监控访问](https://postgresweekly.com/link/157432/web)的简要指南 UMAIR SHAHID

📄 [使用 AWS Lambda,Go 和 Postgres 自动提取图像元数据](https://postgresweekly.com/link/157433/web) HÜSEYIN BABAL

📄 [UUID 作为 Postgres 中的主键](https://postgresweekly.com/link/157434/web) MACIEJ WALKOWIAK

📄 [Postgres 使用 MapLibre 实时位置共享](https://postgresweekly.com/link/157435/web) – 通过 Supabase 边缘函数。THOR SCHAEFF (SUPABASE)

### 🛠 代码和工具

## [ETL Helper 1.0：用于数据库到数据库传输的 Python 库](https://postgresweekly.com/link/157436/web)
专为 Python开发者打造。可与 Postgres、SQLite、SQL Server 和 Oracle 配合使用，我们喜欢它因为它来自[英国地质调查局](https://postgresweekly.com/link/157437/web)。


`BRITISH GEOLOGICAL SURVEY `

[PostGIS 3.5.0.alpha2](https://postgresweekly.com/link/157438/web) – 适用于 Postgres 的强大地理空间工具包。

[River 0.9](https://postgresweekly.com/link/157439/web) – 适用于 Go 的快速可靠的 Postgres 后台作业。

[ParadeDB 0.8.3](https://postgresweekly.com/link/157440/web) – 用于搜索和分析的 Postgres。

[pg-promise 11.9](https://postgresweekly.com/link/157441/web) – 用于 Node.js 的 Postgres 接口。

