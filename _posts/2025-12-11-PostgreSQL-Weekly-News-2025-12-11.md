---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-12-11
---
### PostgreSQL每周新闻#628 - 2025年12月11日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/628)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/v32txavpytfc4mqacel6.jpg)
## [EXPLAIN 执行计划中的扫描类型详解](https://postgresweekly.com/link/178311/web)
使用 EXPLAIN 了解查询的执行方式对于侦错效能问题或最佳化 SQL 语句大有裨益，但「顺序扫描」和「索引扫描」之类的术语究竟是什么意思呢？ Elizabeth 在这里详细讲解了几种主要的扫描类型，并附有图表——你肯定能从中有所收获！

`Elizabeth Christensen`


## [(CERN) 的 TimescaleDB：海量时间序列数据，规模空前](https://postgresweekly.com/link/178310/web)
CERN 的下一代归档系统选择 TimescaleDB，以实现极高的吞吐量、7-10 倍的压缩率以及 10-40 倍的读取速度提升。了解 PostgreSQL + TimescaleDB 如何为 500 多个系统提供支持，并有望成为 CERN 历史资料储存的标准。

`Tiger Data `


## **本周摘要**

* [DB Fiddle](https://postgresweekly.com/link/178312/web) 线上资料库实验平台刚刚新增了 Postgres 18.1 的支援。

* Paul Ramsey 对近期举办的 [PostGIS Day 活动进行了非常详细的回顾](https://postgresweekly.com/link/178313/web)。

* Floor Drees 采访了 [Postgres 贡献者 Bryan Green](https://postgresweekly.com/link/178314/web)，了解他如何透过 Postgres 进入开源领域。


## [关于Postgres中的约束，您应该了解什么](https://postgresweekly.com/link/178317/web)
您可以为表格和列定义约束，以强制执行资料条件。 Gulcin将深入探讨细节。

`Gulcin Yildirim Jelinek (Xata)`

## [闭环：建立使用 Postgres 分支的编码代理](https://postgresweekly.com/link/178319/web)
Xata 的开发者建立了一个代理程式（实际上是开源的），专门用于监控资料库以查找问题并提出修复建议。

`Divyendu Singh (Xata)`

## [Postgres、MongoDB 以及「无法扩展」的真正意义](https://postgresweekly.com/link/178321/web)
对 The Register 最近一篇报导的反思，该报道引用 MongoDB 执行长的话说「PostgreSQL 无法扩展」。

`Umair Shahid`


📄 [使用 Neon Postgres 进行一周实时流量测试的经验总结](https://postgresweekly.com/link/178323/web)——对无伺服器计费方式的优缺点进行了深入思考。 Ishan Das Sharma

📄 [为 Postgres 外部资料包装器新增非同步流程处理功能](https://postgresweekly.com/link/178324/web)。 Bo Lu（Supabase）

📄 [深入探讨 Postgres 18 中的 UUIDv4 与 UUIDv7](https://postgresweekly.com/link/178325/web)。 Josef Machytka


## **发布**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/pfml9flkfq7mtl7nysak.jpg)


## [temBoard 10.0：Postgres 远端控制/仪表板](https://postgresweekly.com/link/178326/web)
一个基于 Python 建构的 Postgres Web 仪表板和监控系统。您只需在目标伺服器上安装代理，temBoard Web 应用程式即可在任何您想要的位置运作。 v10 版本新增了对 Postgres 18 的支持，并可在 Python 3.9 及更高版本上运行，同时提供 RPM 和 DEB 软体包。 GitHub 程式码库。

`Dalibo`


## **📰 分类广告**


🌎 推出基于 Kubernetes 的精简高可用性 PostgreSQL 部署（分散式或单区域），[利用 CNPG 与 pgEdge 的整合](https://postgresweekly.com/link/178330/web)。

PostgreSQL 现已推出，仅需 5 美元。使用 [Aiven 的全新开发者套餐](https://postgresweekly.com/link/178344/web)，告别为闲置实例支付过高费用的烦恼。


## [VectorChord 1.0：Postgres 上的快速向量搜寻](https://postgresweekly.com/link/178332/web)
这款前景广阔、效能卓越的向量索引和查询扩充程式于一年前首次发布，如今已达到 v1.0 版本。我们上个月曾提及该版本，但现在团队撰写了这篇博文，深入探讨了 VectorChord 相较于 pgvector 如何实现如此显著的效能提升。

`Jinjing Zhou`

💡 他们在文章[《我们如何在 PostgreSQL 上 20 分钟内实现 1 亿向量索引》](https://postgresweekly.com/link/178334/web)中进行了更深入的技术探讨。


## [隆重介绍 pg_clickhouse：用于查询 ClickHouse 的 Postgres 扩充](https://postgresweekly.com/link/178335/web)
ClickHouse 是一个流行的开源 OLAP 系统，此扩充功能提供了一种直接从 Postgres 透明地执行 ClickHouse 分析查询的方法。

`David Wheeler (ClickHouse)`

[WhoDB 0.82](https://postgresweekly.com/link/178337/web) – 轻量级的新一代多资料库资料浏览器。

[linq2db 6.0](https://postgresweekly.com/link/178338/web) – LINQ to Database 提供者。现已支援 .NET 10。

[PGSync 7.0](https://postgresweekly.com/link/178339/web) – Postgres 与 Elasticsearch/OpenSearch 的同步。

[Procrastinate 3.6](https://postgresweekly.com/link/178340/web) – 基于 Postgres 的 Python 任务伫列。

[pgroll 0.15](https://postgresweekly.com/link/178341/web) – 零停机、可逆的模式迁移。

[Squawk 2.32](https://postgresweekly.com/link/178342/web) – 用于 Postgres 迁移和 SQL 的程式码检查器。

[pgAdmin 4 v9.11](https://postgresweekly.com/link/178343/web)