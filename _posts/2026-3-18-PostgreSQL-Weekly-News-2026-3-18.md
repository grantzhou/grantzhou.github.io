---
layout: post
title: PostgreSQL 每周新闻 2026-3-18
---
### PostgreSQL每周新闻#640 - 2026年3月18日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/640)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/bg5bo8e2gztsetgvhrbo.jpg)

## [`work_mem`：这是个陷阱！](https://postgresweekly.com/link/182380/rss)

拥有2 TB的RAM和`work_mem`设置为2MB，你不会预料到你的Postgres服务器会被OOM（内存不足）杀手干掉。然而，一个写得很糟糕的查询*确实*导致了这种情况，两位Postgres专家开发者发现了背后令人惊讶的原因。

**Lætitia Avrot and Henrietta Dombrovskaya**

💡 我很喜欢Lætitia说的 *"使用Postgres二十年了，我每周都能学到新东西"*，她提到的是[`pg_log_backend_memory_contexts()`](https://postgresweekly.com/link/182381/rss) —— 你可以[在这里了解更多关于使用它来调优`work_mem`的信息](https://postgresweekly.com/link/182382/rss)。


## [赞助商：`SELECT COUNT(*)`不应该需要8秒](https://postgresweekly.com/link/182379/rss)

表在增长。查询在变慢。大多数团队会添加第二个数据库。但Postgres可以处理它。TimescaleDB添加了hypertables、95%压缩和持续聚合。在实时数据上进行分析，使用你已经在写的相同SQL。[免费开始构建](https://postgresweekly.com/link/182379/rss)。

**Tiger Data (creators of TimescaleDB) 赞助商**


**本周摘要：**

- 🤖 Bruce Momjian说[`COMMENT`命令对MCP用例特别有用](https://postgresweekly.com/link/182383/rss)，通过为LLM提供额外的元数据来使用（或作为存储它们自己元数据的方式）。

- EDB的Floor Drees分享了[PGConf.dev即将到来的主题预览](https://postgresweekly.com/link/182384/rss)，会议将于5月在Vancouver举行。

- PGCA（PostgreSQL Community Association）已经[显著更新了其网站](https://postgresweekly.com/link/182385/rss)，并解释了其在保护Postgres各种商标方面的作用以及你如何帮助支持它。

- Pavel Luzanov [总结了最新的CommitFest](https://postgresweekly.com/link/182386/rss)以及因此将登陆Postgres 19的众多功能。


## [Netflix如何自动化其RDS Postgres到Aurora Postgres的迁移](https://postgresweekly.com/link/182387/rss)

早在2024年，Netflix决定将数百个Postgres集群从RDS迁移到Aurora，这是一项具有挑战性的任务，零数据丢失和最小停机时间是必须的。这是对该过程的详细记录，虽然这是AWS内部的迁移，但大多数技术具有普遍适用性。

**Kannan, Akintayo, Bharadwaj, et al. (Netflix)**


## [我们跳过了OLAP堆栈，在Postgres中构建了我们的数据仓库](https://postgresweekly.com/link/182388/rss)

作为一个Postgres服务，Xata想要[吃自己的狗粮](https://postgresweekly.com/link/182389/rss)，所以这里介绍了他们如何在原生Postgres之上构建自己的数据仓库方法。

**Noémi Ványi (Xata)**


## [等待Postgres 19：为`pg_dumpall`添加非文本输出格式](https://postgresweekly.com/link/182390/rss)

深入了解一个令人欢迎的Postgres 19变化：*"`pg_dumpall`现在除了纯文本外，还可以生成custom、directory或tar格式的输出"*。

**Hubert 'depesz' Lubaczewski**


📄 [Postgres是网关药物](https://postgresweekly.com/link/182391/rss) — 三家公司，18个月内与Postgres相关的收购超过15亿美元。发生了什么？**Vignesh Ravichandran**


## 分类广告：

👾 没有成功的表演。只有工程师分享实际出了什么问题以及他们如何修复它。[BugBash](https://postgresweekly.com/link/182392/rss) 2026，4月23-24日在华盛顿特区。

使用Aiven的免费套餐构建和分享你的开发之旅，竞争1000美元。在3月31日前使用#AivenFreeTier分享你的项目。[在这里参加](https://postgresweekly.com/link/182393/rss)。

🤖 喜欢Claude？利用自然语言数据库操作与[Postgres的MCP服务器](https://postgresweekly.com/link/182394/rss)。


## 🛠 代码和工具

**[pg_turret：将结构化Postgres日志流式传输到HTTP或Kafka端点](https://postgresweekly.com/link/182395/rss)** — 钩入Postgres的`emit_log_hook`来捕获事件，并将它们作为结构化JSON实时流式传输到HTTP（或Kafka）端点，无需任何日志文件解析。

**lasect**


**[pg_stat_ch：将每个查询的Postgres遥测导出到ClickHouse](https://postgresweekly.com/link/182396/rss)** — ClickHouse团队构建了一个Postgres扩展，它捕获每个查询的执行遥测并实时导出到ClickHouse。

**ClickHouse**


**[pg_duckpipe：为你的Lakehouse提供实时CDC](https://postgresweekly.com/link/182397/rss)** — 一个新的Postgres扩展，通过基于WAL的CDC将常规堆表持续同步到[DuckLake](https://postgresweekly.com/link/182398/rss)列式表（基于Parquet的格式）。

**Relyt**

- [Tansu 0.6](https://postgresweekly.com/link/182399/rss) – Apache Kafka的替代品，支持Postgres、libSQL/SQLite、S3或内存存储引擎。

- [PostgreSQLCopyHelper 3.0](https://postgresweekly.com/link/182400/rss) – 使用二进制COPY为.NET批量插入数据。

- [pg_timetable 6.3](https://postgresweekly.com/link/182401/rss) – 高级独立作业调度器。