---
layout: post
title: PostgreSQL 每周新闻 2026-8-12
categories: [PostgreSQL]
tags: [PGWeekly]
---
### PostgreSQL每周新闻#661 - 2026年8月12日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/661)

🏖️ **我们下周将进行夏季休息**，因此下一期将于8月26日发布。

*您的编辑，Peter Cooper*

---

## [介绍 `sqlfmt`：一个 SQL `gofmt` 风格的格式化工具](https://tapoueh.org/blog/2026/08/introducing-sqlfmt-an-sql-gofmt-style-formatter/)
![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/mmevx99yjrirxdxontes.jpg)

Postgres 贡献者 Dimitri 长期以来开发了自己的 SQL 风格方式（如他的书《The Art of PostgreSQL》中所用），并构建了一个 Go 工具来自动应用它。更好的是，[你可以在网页上使用它](https://theartofpostgresql.com/postgresql-sql-formatter/)，因此如果你正在准备演示文稿或博客文章，可以在你的查询上试试。

`Dimitri Fontaine`

## [即将推出：ParadeDB Cloud](https://paradedb.com/cloud)
我们正在构建一个完全托管的 ParadeDB：一个用于应用数据、全文搜索、向量检索和聚合的 Postgres。我们的早期访问候补名单现已开放。

`ParadeDB` **赞助商**

## [Postgres 子事务的危险](https://planetscale.com/blog/the-dangers-of-postgres-subtransactions)
一个包含超过 64 个子事务的事务可能会使集群陷入停滞。一次 `pgbench` 运行显示吞吐量从 7,200 TPS 下降到 160 TPS，而且情况会更糟：新的只读副本可能会完全拒绝连接。

`Nidzwetzki and Berube (PlanetScale)`

**简讯：**

- ⏰ **Postgres 的季度小版本更新预计将在明天（8月13日）发布。** 截至发稿时尚未宣布任何消息，但由于我们下周休息，你需要[自己查看发布说明](https://www.postgresql.org/docs/release/) —— 预计所有支持的分支都会有更新。

- *Electric* 团队，即 [PGlite](https://pglite.dev/)（编译为 WASM 的 Postgres）和 Electric 同步引擎的幕后团队，正在[加入 Databricks 的 Neon 团队](https://neon.com/blog/electric-joins-neon)。这里是 [Electric 方面的故事](https://electric.ax/blog/2026/08/11/electric-joining-databricks)。

- **快速发布：** [pg_clickhouse 0.10.0](https://clickhouse.com/blog/pg_clickhouse-whats-new-july-2026)、[PostgREST 16.0](https://github.com/PostgREST/postgrest/releases/tag/v16.0)（和 [16.1](https://github.com/PostgREST/postgrest/releases/tag/v16.1)）、[Citus 14.2](https://github.com/citusdata/citus/releases/tag/v14.2.0)、[Doltgres 1.0](https://www.dolthub.com/blog/2026-08-06-doltgres-1-0/)、[pgAdmin 4 9.17](https://www.pgadmin.org/docs/pgadmin4/9.17/release_notes_9_17.html)、[E-Maj 5.0](https://www.postgresql.org/about/news/announcing-e-maj-500-3353/)

## [重建 Postgres 以实现 300 倍更快的分析](https://malisper.me/how-we-made-postgres-hundreds-of-times-faster-the-query-engine/)
[pgrust](https://github.com/malisper/pgrust) 的创建者（一个用 Rust 重写 Postgres 的尝试）反思了查询引擎中批处理、算子融合和 SIMD 的力量。

`Michael Malis`

## [介绍 `pg-java`：JVM 的新 Postgres 驱动程序](https://launchbylunch.com/posts/2026/Jul/29/introducing-pg-java/)
一位长期的 [pgjdbc](https://github.com/pgjdbc/pgjdbc) 维护者解释了为什么他从头创建了一个基于虚拟线程构建的 Postgres 优先 JVM 驱动程序：[pg-java](https://github.com/pgjdbc/pg-java)。不过它仍被认为是*预发布*版本。

`Sehrope Sarkuni`

📄 [在 Postgres 中建模状态转换](https://thoughtbot.com/blog/modeling-state-transitions-in-postgres) – 当属性随时间变化且这些变化很重要时，将其建模为带时间戳行的单独表。`Thiago Araújo Silva`

📄 [选择正确的 Postgres 分区键](https://stormatics.tech/blogs/choosing-the-right-postgresql-partition-key) – 你可以"完美"地分区一个巨大的表，但慢查询仍然可能保持同样慢... `Umair Shahid (Stormatics)`

📄 [使 Postgres 文档更好](https://www.fromdual.com/blog/postgresql/improve-postgresql-documentation/) – 在 Postgres 中落地文档修复的实践要素。`Oli Sennhauser`

📄 [在 Postgres 中使用 `pgcrypto` 实现多租户 BYOK 加密](https://xata.io/blog/multi-tenant-byok-encryption-in-postgresql-with-pgcrypto) `Tudor Golubenco`

## 📰 分类广告

将机器数据的实时流转换为实时仪表板，全部在 Postgres 上。9月9日免费实践研讨会。[预留你的位置](https://www.tigerdata.com/events/workshop-ignition-meets-tiger-cloud?utm_source=content-syndication&utm_medium=referral&utm_campaign=postgres-weekly-newsletter)。

🚀 将你的 Postgres 生产力提高三倍。[pgEdge AI DBA Workbench](https://pgedge.com/download/ai-dba-workbench)：适用于任何 Postgres v14+ 的 AI 监控和诊断。[开源](https://pgedge.com/download/ai-dba-workbench)。

---

## 今年迄今为止的热门内容：

由于我们休息一周，这是一个自然的时刻来反思并关注 2026 年迄今为止的一些最佳内容。我们知道并不是每个人都有时间阅读*每一*期，所以可能有一些你错过的精彩内容... :-)

从热门内容（按点击量）中精选：

1. [Postgres is Enough](https://postgresisenough.dev/) – 一个有用的目录，展示 Postgres 如何替代其他系统，包括 Redis、Elasticsearch 和 Kafka。

2. [`work_mem`: It's a Trap!](https://mydbanotebook.org/posts/work_mem-its-a-trap/) – 一个有趣的故事，讲述两位经验丰富的 Postgres 开发人员深入研究一台拥有 2TB RAM（`work_mem` 设置仅为 2MB）的服务器是如何被一个写得很糟糕的查询搞垮的。

3. [移动一个词如何使查询速度提高 10-50 倍](https://postgres.ai/blog/20260311-not-exists-vs-exists-partial-index) – 一个*"但是...怎么会？"*的时刻，两个逻辑上等价的查询导致性能差异达 32 倍。

4. [Postgres Locks Explained](https://postgreslocksexplained.com/) – *"这是我刚开始学习锁时希望存在的资源"*，该网站的作者如是说，该网站专注于以易于理解的方式解释 Postgres 中使用的不同类型的锁。

5. [Life Altering Postgresql Patterns](https://mccue.dev/pages/3-11-25-life-altering-postgresql-patterns) – 十二个小贴士和见解，从使用 UUID 作为主键和表命名到使用模式和视图。这一条来自[第 630 期](https://postgresweekly.com/issues/630)对 *2025* 年最佳内容的回顾，但我想我们可以再运行一次...

---

在我离开之前，我想感谢所有最近提交内容的人。我已经积累了相当多的队列要处理，我不确定需要多长时间。但请放心，我会阅读每一条，并将在未来的期刊中包含一些 :-)

👋 我们现在休息一周 —— 8月26日再见！