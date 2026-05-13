---
layout: post
title: PostgreSQL 每周新闻 2026-5-13
---
### PostgreSQL每周新闻#648 - 2026年5月13日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/648)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/ateqfl1iffefiwqk6t0z.jpg)

## [对 Postgres `VIEW` 的强烈看法](https://postgresweekly.com/link/185056/rss)
为什么视图在 Postgres 中使用起来很简洁但修改起来很痛苦，深入介绍它们在底层是如何工作的以及 `ALTER VIEW` 缺少了什么。令人惊讶的是，可以修复这个问题的机制已经存在于 `pg_dump` 中了...

`Radim Marek`


## [`REFRESH MATERIALIZED VIEW` 不应该阻塞生产环境](https://postgresweekly.com/link/185055/rss)
你编写物化视图来预计算汇总数据。现在它在刷新时锁定表。获得 $1000 的信用额度来尝试替代方案。TimescaleDB 连续聚合在实时数据上增量更新。无需 REFRESH，无锁，无 cron。

`Tiger Data (creators of TimescaleDB)` **赞助商**


## [使用生成列让 JSONB 更易查询](https://postgresweekly.com/link/185057/rss)
基于基准测试比较 GIN、表达式索引和生成列。Richard 发现基于 B-tree 的方案在查询延迟、存储和写入方面都优于 GIN，其中生成列最易于维护。

`Richard Yen`


**简讯：**

- [Render](https://postgresweekly.com/link/185058/rss)，一个流行的托管平台，已添加与 [ParadeDB](https://postgresweekly.com/link/185059/rss) 的官方集成，这是一个类似 Elastic 的 Postgres 搜索扩展。

- [*Neon* 关闭了全页写入](https://postgresweekly.com/link/185060/rss)，写入吞吐量提升高达 5 倍。


## [无需编译器：编写纯 SQL 扩展](https://postgresweekly.com/link/185061/rss)
很容易将 Postgres 扩展视为复杂的多语言项目（许多最流行的扩展确实如此！），但它们可以完全用你已经了解的 SQL 构建。Shaun 在这里演示如何创建这样的扩展。

`Shaun Thomas`


## [Postgres 替代存储引擎实地指南](https://postgresweekly.com/link/185062/rss)
在 Postgres 12 中[表访问方法 API](https://postgresweekly.com/link/185063/rss) 发布六年后，Christophe 调研了生态系统的实际情况，以及为什么它比早期预测的更加混乱。

`Christophe Pettus`


## [▶  从 MemSQL 到 HorizonDB：与 Adam Prout 的工程师之旅](https://postgresweekly.com/link/185064/rss)
Azure HorizonDB 的创始架构师讲述他 20 年来穿越关系数据库到 Postgres 的旅程。

`Talking Postgres Podcast` **podcast**


📄 [使用 eBPF 和硬件断点跟踪 Postgres](https://postgresweekly.com/link/185065/rss) – 今天学到：你可以在内存中跟踪像 `nextXid` 和 `nextOid` 这样的变量更新。至少在 Linux 上可以。*Jan Nidzwetzki*

📄 [Postgres SSL 初学者指南](https://postgresweekly.com/link/185066/rss) – 一个实用入门，包括需要避免的常见错误列表。*Shridhar Khanal*


### 📰 分类广告：

⚡ Postgres 专家不够用？[pgEdge AI DBA Workbench](https://postgresweekly.com/link/185067/rss) 为每个团队提供全天候高级 DBA。任何 Postgres。[开源](https://postgresweekly.com/link/185067/rss)。

🐘 自托管 Postgres？[试试 ParadeDB](https://postgresweekly.com/link/185068/rss)，一个 Postgres 扩展，可实现 Elasticsearch 质量的全文、向量和混合搜索。无需 ETL 管道，无需 Elastic 集群。


## 🛠 代码和工具

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/juc08pf0bya10r8midlf.jpg)

## [pg_flight_recorder: 通过 `pg_cron` 进行连续状态采样](https://postgresweekly.com/link/185069/rss)
一个纯 SQL 扩展，使用 `pg_cron` 持续快照 Postgres 状态（`pg_stat_activity`、`pg_stat_statements`、`pg_locks` 等），让你能够访问出错时发生的滚动历史记录。

`Dmitry Ventin (Supabase)`


## [pg_sorted_heap 0.13.0: 物理排序存储与 HNSW 向量搜索](https://postgresweekly.com/link/185082/rss)
一个早期阶段的扩展，提供具有区域映射块修剪的物理排序表和集成规划器的 HNSW 向量索引，无需 `pgvector`。面向 GraphRAG 和向量检索工作负载。

`Sergey Kuznetsov`


- ⚠️ [PgBouncer 1.25.2](https://postgresweekly.com/link/185071/rss) – 修补四个 CVE 的安全维护版本。

- [PGQueuer 1.0](https://postgresweekly.com/link/185072/rss) – Python 作业队列库，在 Postgres 之上提供实时、并发后台作业处理（[v1.0 发布说明](https://postgresweekly.com/link/185073/rss)）。

- 🔎 [pg_textsearch 1.2](https://postgresweekly.com/link/185074/rss) – BM25 相关性排名全文搜索扩展添加了*"对物理复制的适当支持"*。

- [pg_clickhouse 0.3](https://postgresweekly.com/link/185075/rss) – 在 ClickHouse 上执行分析查询而无需重写 SQL。[有关此版本的更多信息请点击这里。](https://postgresweekly.com/link/185076/rss)

- 🕒 [TimescaleDB 2.27.0](https://postgresweekly.com/link/185080/rss) – 时间序列扩展在某些查询上获得显著更快的性能。

- [pg_trickle 0.58](https://postgresweekly.com/link/185078/rss) – 声明式、自动刷新的物化视图。