---
layout: post
title: PostgreSQL 每周新闻 2023-2-15
---
### PostgreSQL每周新闻#493 - 2023年2月15日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/493)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,e_trim,w_300,h_160/e_make_transparent/co_white,e_outline:7/chrf2e7pv4jro5ke7sue.jpg)
## [期待 Postgres 16: I/O 统计功能 withpg_stat_io](https://postgresweekly.com/link/135374/web)
查看在未来版本的 Postgres 中使用新的pg_stat_io视图查询系统范围的 I/O 统计信息，它的几个用例，以及对 I/O 可观察性未来的思考一般在 Postgres 中。


`Lukas Fittl `
## [揭露 Postgres 性能秘密](https://postgresweekly.com/link/135399/web)
长期担任 Postgres 专家的 Craig 列出了今天要设置的四项基本内容，以便在未来更快地发现和修复性能问题。


`Craig Kerstiens `
## [免费下载 PostgreSQL 高可用性架构](https://postgresweekly.com/link/135376/web)
Percona 架构仅使用经过实战测试的开源组件构建，旨在确保高达 99.9% 的可用性。架构适用于各种规模的企业。


`Percona `
## [使用 pgvector 在 Postgres 中存储 OpenAI 嵌入](https://postgresweekly.com/link/135377/web)
一个示例，说明如何使用 OpenAI 的嵌入和 Postgres 构建机器学习驱动的搜索引擎。这个想法是你将句子（在这种情况下）压缩成向量，存储这些向量，然后查询它们——pgvector可以帮助你。


`Greg Richardson (Supabase) `
## [使用 SQL 窗口函数处理排名](https://postgresweekly.com/link/135401/web)
一个方便、易于理解的教程，介绍如何进行评级和将数据划分到从 Anton 的SQL Window Functions Explained一书中提取的分区。


`Anton Zhiyanov `
## [查找当前时间戳](https://postgresweekly.com/link/135403/web)
您认为确定时间很容易，但有几个选项。详细了解实时、报表时间和交易时间。


`Hans-Jürgen Schönig `
## [▶  使用 PolyScale.ai 在边缘缓存 Postgres ](https://postgresweekly.com/link/135382/web)
Polyscale的快速介绍，这是一种无服务器即插即用数据库缓存。


`Sam Aybar and Supabase `
## [使用 pg_walinspect 调试 WAL 事件](https://postgresweekly.com/link/135384/web)
pg_walinspect是 Postgres 提供的一个模块，用于查看预写日志的内容。


`Anthony Sotolongo `
## [pgpq：将 Arrow / Parquet 数据流式传输到 Postgres](https://postgresweekly.com/link/135389/web)
一个新的“概念验证阶段”库，用于将 Arrow RecordBatches 流式传输到 Postgres，以便批量加载 Parquet 文件。用 Rust 编写。


`Adrian Garcia Badaracco `
## [SQL Notebook：SQL 中的随意数据探索](https://postgresweekly.com/link/135390/web)
从 CSV、Excel、Microsoft SQL Server、Postgres 和 MySQL 导入数据。使用 Jupyter 风格的笔记本界面进行探索性查询，并为可重用逻辑编写存储过程。


`Brian Luft `
## [Postgres 消息队列 (PGMQ) ](https://postgresweekly.com/link/135391/web)
作为扩展的 Postgres 上的轻量级分布式消息队列。用 Rust 编写，作为CoreDB Postgres 发行版的一部分存在。


`CoreDB `
# 💡本周提示


**🗓即将举办的Postgres活动**
