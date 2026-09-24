---
layout: post
title: PostgreSQL 每周新闻 2026-9-2
categories: [PostgreSQL]
tags: [PGWeekly]
---
### PostgreSQL每周新闻#663 - 2026年9月2日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/663)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/hfb97u0pwpy9p7faaaif.jpg)

## [从主库读取自己的写入：`WAIT FOR` 性能测试](https://boringsql.com/posts/read-your-own-writes/)
上周，我们分享了一篇解释 Postgres 19 的 `WAIT FOR` 功能的文章。现在，Radim 对其进行了测试：即使在回环网络上，朴素的副本读取在 1000 次中有 992 次是陈旧的，但 `WAIT FOR` 将其降至零，只增加约 1-2ms 的开销。

`Radim Marek`

## [Postgres 在智能体时代：Forrester 炉边谈话](https://www.enterprisedb.com/resources/webinar/multimodel-data-platforms-agentic-era?utm_source=newsletter&utm_medium=email&utm_campaign=wb_ww_vcop_webinar-promotion-tai-20260828)
Forrester 的 Indranil Bandyopadhyay 与 EDB 的 Lizzy Nguyen 一起探讨多模型数据平台市场：发展方向、融合带来的机遇，以及在做出承诺之前如何规划工作负载。基于 The Forrester Wave，2026 年第二季度。

`EnterpriseDB` **赞助商**

## [介绍 YeSQL：实用 Postgres，一次一个概念](https://tapoueh.org/blog/2026/08/introducing-yesql-practical-postgresql-one-concept-at-a-time/)
27 节免费 SQL 课程（位于[这里](https://theartofpostgresql.com/yesql/)），涵盖 `NULL` 语义、窗口框架、`LATERAL` 连接和读取 `EXPLAIN` 结果等内容。查询使用 [PGlite](https://pglite.dev/) 在浏览器中运行，无需注册。

`Dimitri Fontaine`

### 本周摘要：

- ⭐ [Postgres 19 已删除 `ALTER TABLE … MERGE/SPLIT PARTITION(S)`](https://git.postgresql.org/gitweb/?p=postgresql.git;a=commitdiff;h=7612ae8ed8c941985d9cbf60a0674c48f5b0abe5)，因为[发布团队要求撤销](https://www.postgresql.org/message-id/ao8WNnQXpGUykHLA%40nathan)该功能，原因是存在未解决的设计问题。这是该功能第二次被删除（之前在 Postgres 17 中）。期待 Postgres 20 吧。

- Tiger Data 询问了几位行业观察人士[为什么一个"40 年历史的数据库"在 AI 时代仍然获胜](https://www.tigerdata.com/blog/why-40-year-old-database-still-winning-ai-era)。

- ❓ 那么 Postgres 是 30 岁还是 40 岁？都是！[文档的历史页面](https://www.postgresql.org/docs/current/history.html)将 Berkeley 的 "POSTGRES" 追溯到 1986 年，这是 Tiger 提到的 40 年的来源，而[我们在 7 月份提到的 30 周年](https://vonng.com/en/pg/happy-30-birthday/)则是指 Postgres95 获得其第一个公共 CVS 服务器的时间（本质上是社区运行项目的开始）。

- 🇬🇧 [PGDay UK 2026](https://2026.pgday.uk/) 将于下周（9 月 8 日）在伦敦举行。门票仍然可用。

## [Postgres 18 中使用 UUID v7 实现 23 倍快速插入](https://andyatkinson.com/postgresql-18-uuidv7)
切换到 `uuidv7()` 大幅缩短了十亿行表的插入时间（相比之前使用的 v1 和 v4 键），尽管 `ALTER TABLE` 需要访问排他锁和抖动重试循环来完成切换。

`Andrew Atkinson`

## [深入了解 Postgres 19 的众多 `pg_catalog` 变化](https://richyen.com/postgres/2026/08/31/pg_catalog_almanac.html)
`pg_catalog` 是关于数据库结构、对象和内部工作的宝贵信息来源。[pg-catalog-almanac](https://richyen.com/pg-catalog-almanac/) 可让您查看目录结构多年来的变化，Richard 有三个亮点要分享。

`Richard Yen`

🤩 截至 beta 3，Postgres 19 的 `pg_catalog` 变化是近期版本中最多的，新增了 12 个目录和视图以及 43 个列，因此这个年鉴可能会很有用！

## [pg_tre 和 pg_re2：Postgres 中正则表达式的新选择](https://www.depesz.com/2026/08/25/new-things-for-regular-expressions-in-postgresql-pg_tre-and-pg_re2/)
在 33GB 表上针对 [pg_trgm](https://www.postgresql.org/docs/current/pgtrgm.html) 对两个新正则表达式扩展进行基准测试。ClickHouse 的 [pg_re2](https://github.com/clickhouse/pg_re2/) 在速度上获胜，而 [pg_tre](https://codeberg.org/gregburd/pg_tre) 提供模糊匹配，但索引需要数小时。

`Hubert 'depesz' Lubaczewski`

📄 [Postgres 并不慢：是你的存储慢](https://clickhouse.com/blog/posette-talk-recap-postgres-isnt-slow-your-storage-is) – [POSETTE 2026 演讲](https://www.youtube.com/watch?v=h7by8IKtJG0)的摘要，关于对本地 NVMe 存储与 EBS 的基准测试，展示网络存储的延迟如何复合。*Sai Srirampur / ClickHouse*

📄 [Postgres 19 中的新系统视图](https://clickhouse.com/blog/postgres-19-new-system-views) – 查看 `pg_stat_lock`、`pg_stat_recovery`、`pg_stat_autovacuum_scores` 和 `pg_dsm_registry_allocations`。*Gülçin Yıldırım Jelínek*

### 🛠 代码和工具

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/sj8mvqfrsfjkudthhf5r.jpg)

## [pgterm：适用于所有 Postgres 数据库的 `htop`](https://pgterm.dev/)
一个 Rust TUI，每个 Postgres 数据库一个选项卡，后台健康检查，以及查询、索引和表的视图。在底层，诊断来自我们上周推荐的 [pgbot](https://pgbot.dev/)。[GitHub 仓库](https://github.com/pgrundev/pgterm) README 有更多信息。

`Alex Shapalov`

## [pg_shmemviz：在浏览器中可视化 Postgres 共享内存](https://bdrouvot.github.io/2026/08/20/welcome-to-pg-shmemviz-postgresql-shared-memory-visualizer/)
渲染分配、C 结构字段、填充和原始字节，从您自己的 `postgres` 二进制文件读取 DWARF（仅限开发实例）。您还可以对比快照。

`Bertrand Drouvot`

## 📊 [PoWA (PostgreSQL Workload Analyzer) 5.3](https://powa.readthedocs.io/en/latest/)
一个从多个实例收集和聚合指标的工具，然后可以通过实时图表查看以帮助优化您的设置。v5.3 改进了 Postgres 19 兼容性。

`PoWA Team`

- [Doltgres 1.3](https://github.com/dolthub/doltgresql/releases/tag/v1.3.0) – 类似 Git 的版本控制数据库（构建在 [Dolt](https://www.dolthub.com/) 之上），支持 Postgres 线路协议。

- [Stateless Postgres Query Router (SPQR) 3.1](https://github.com/pg-sharding/spqr/releases/tag/3.1.0) – 由 Yandex Cloud 构建的生产就绪 Postgres 分片解决方案。

- [pg_trickle 0.91.0](https://github.com/trickle-labs/pg-trickle/releases/tag/v0.91.0) – 提供声明式流表的扩展，通过差分数据流进行增量视图维护。

- [sabiql 3.0](https://github.com/riii111/sabiql) – 基于 `psql` 构建的用于浏览、查询和编辑数据库的 TUI。

### 来自 DATADOG 的 POSTGRES 统计数据：

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/h7seqwjyy4nrsrvxqgwl.jpg)

## [2026 年 Postgres 现状](https://www.datadoghq.com/state-of-postgres/)
对 Datadog 许多客户运行其 APM 和监控代理的数据进行分析显示，Postgres 的采用率持续攀升，但只有 15% 的实例设置了 `statement_timeout`，覆盖索引仅占所有索引的 0.3%，22% 的表有（很少索引的！）JSONB 列，`pgvector` 是增长最快的非捆绑扩展，等等。

`Datadog`

🤔 他们还发现，在抽样时间中，Postgres 后端有 56% 的时间在打开的事务中处于空闲状态，显然是在等待应用程序，而只有 37% 的时间在进行数据库工作。