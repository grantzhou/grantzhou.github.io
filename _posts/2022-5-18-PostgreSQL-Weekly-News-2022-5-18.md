---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2022-5-18
---
### PostgreSQL每周新闻#455 - 2022年5月18日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/455)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/ycm7mm2ynvs9dxxbuwh7.jpg)
## [Google Cloud 推出了适用于 PostgreSQL 的 AlloyDB](https://postgresweekly.com/link/123595/web)
这并不是一个完美的比较，但想想 Amazon Aurora，除了 Google 吹嘘这是“只有 Google 才能提供的 PostgreSQL”。 AlloyDB 是一个托管的与 Postgres 兼容的服务（尽管它看起来确实像 Postgres 的元素就在幕后），它承诺以一定的价格实现无缝扩展。 这里有更技术性的解释。


`Google Cloud `
## [在几分钟内全球扩展 Postgres，无需编写代码](https://postgresweekly.com/link/123597/web)
PolyScale.ai 是 Postgres 的即插即用无服务器边缘缓存。 无需编写代码或部署基础架构，即可在几分钟内实现全球扩展。 轻松启用数据驱动的无服务器功能。


`PolyScale.ai `
## [Postgres 15 发行说明草案](https://postgresweekly.com/link/123598/web)
Postgres 15 几个月后才发布（尽管第一个测试版将在几周内发布），但 Bruce Momjian 已经完成了 PG 15 发行说明的初稿并列出了主要的调整和改进。


`PostgreSQL Documentation `
## [CloudNativePG：用于 Postgres 的新 Kubernetes operator](https://postgresweekly.com/link/123601/web)
EDB 发布了一个获得 Apache 2.0 许可的 Kubernetes Operator，它可以处理 Postgres 集群的整个生命周期。 GitHub 存储库。 


`Gabriele Bartolini (EDB) `
## [Postgres 索引扫描解释](https://postgresweekly.com/link/123603/web)
Egor 回来了，对索引扫描进行了深入研究，如果您在查询计划中看到“位图索引扫描”或“仅并行索引扫描”并想知道它们的真正含义，这应该有助于清除问题。


`Egor Rogov `
## [由 SQL 提供支持的可观察性：将 OpenTelemetry Traces 带入 Postgres](https://postgresweekly.com/link/123604/web)
OpenTelemetry 是一种检测标准（跟踪、指标、日志等），Timescale 人员宣布了 Promscale，它是基于 Postgres 和 TimescaleDB 构建的 Promethius 和 OpenTelemetry 的后端，用于分析此类数据 用 SQL。


`Ramon Guiu (Timescale) `
## [在几分钟内在 Postgres 上构建任何内部工具。 使用点击界面从其他来源或 API 添加数据](https://postgresweekly.com/link/123606/web)


`Retool — 10x faster internal tools `
## [将 Postgres RDS 分区表导出到 S3 的经验](https://postgresweekly.com/link/123607/web)
我们都喜欢编写脚本来移动数据，对吧？...对吗？ 好吧，正如我们在这里看到的那样，这并不总是有趣或容易的，他们最终不得不将这种方法置于冰上。


`George Petropoulos `
## [在 Linux、Docker 和 Postgres 中整理文本的冒险](https://postgresweekly.com/link/123608/web)
作者正在开发的一个应用程序中出现了一个文本排序错误，它需要在整理设置中进行比您预期的更多的挖掘。


`Paul Cochrane `

