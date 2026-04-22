---
layout: post
title: PostgreSQL 每周新闻 2026-4-22
---
### PostgreSQL每周新闻#645 - 2026年4月22日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/645)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/obmbrc1smyax7fktvtuk.jpg)

## 📝 [PostgreSQL 19 发布说明的首个草案](https://postgresweekly.com/link/184105/rss)

Bruce [刚刚完成](https://postgresweekly.com/link/184106/rss)了 Postgres 19 发布说明的首个草案，内容以项目符号形式列出大量内容，[计划](https://postgresweekly.com/link/184107/rss)在今年9月正式发布，预计未来几个月内会有 beta 版本[推出](https://postgresweekly.com/link/184108/rss)。

Bruce Momjian

💡如果你想了解发布说明背后的制作过程，Bruce [制作了这个 wiki 页面](https://postgresweekly.com/link/184109/rss)。

---

**💰 赞助商**

## [您的热表达到了10亿行，接下来怎么办？](https://postgresweekly.com/link/184104/rss)

TimescaleDB 自动对增长的表进行分块，将冷数据压缩高达95%，并通过连续聚合预先计算汇总数据。全部都在原生 Postgres 中完成。无需新的查询语言，无需第二个数据库，无需迁移。[免费开始构建](https://postgresweekly.com/link/184104/rss)。

Tiger Data (TimescaleDB的创建者) *赞助商*

---

## [Xata OSS 简介：支持分支的 Postgres 平台，现已采用 Apache 2.0 许可证](https://postgresweekly.com/link/184117/rss)

[Xata](https://postgresweekly.com/link/184118/rss) 已将其 Postgres 平台的核心技术开源。您可以获得存储层的写时复制分支功能，在几秒钟内克隆数据库，为不活跃的分支提供零规模扩展，同时底层仍然是标准的 Postgres。

Tudor Golubenco / Xata

---

## 本周摘要：

- 🤖 一位开发者正在[尝试用 Rust 重建 Postgres](https://postgresweekly.com/link/184112/rss)，使用 AI 代理，因为...为什么不呢？到目前为止，Postgres 的三分之一测试已经通过，这里有一个[在线演示](https://postgresweekly.com/link/184113/rss)。

- Cloudflare 预告了与 PlanetScale 合作的一项开发，将于下月推出：[能够直接从 Cloudflare 仪表板部署 PlanetScale 托管的数据库](https://postgresweekly.com/link/184114/rss)，用于 *Workers*。

- 🇺🇸 [PGDay Boston 2026](https://postgresweekly.com/link/184115/rss) 将于今年6月9日在波士顿举行，Postgres 项目的原始负责人 Michael Stonebraker 将发表主题演讲。

- 🇨🇭 [Swiss PGDay 2026](https://postgresweekly.com/link/184116/rss) 将于今年6月25-26日在瑞士拉珀斯维尔举行。

---

## 📉 [调查 Linux 7.0 的 Postgres 吞吐量回归问题](https://postgresweekly.com/link/184110/rss)

我们最近介绍了一篇关于 [Linux 7.0 如何影响 Postgres 性能](https://postgresweekly.com/link/184111/rss)的文章（*在某些特定设置上*）。Lætitia 深入探讨了实际问题是什么，谁会受到影响（我们中的极少数人！）以及升级时需要记住的事项。

Lætitia Avrot

---

## [CTID 如何让我在处理2亿行时获得30倍的加速](https://postgresweekly.com/link/184119/rss)

探讨了索引扫描在大规模静态表上失效的情况，内部 `ctid`（物理行地址）如何实现真正的顺序 I/O，以及带有访问模式差异可视化的完整实现。

Connor Hallman

---

## [当 Upsert 不更新但仍然写入时](https://postgresweekly.com/link/184120/rss)

Datadog 如何追踪到双倍磁盘写入和四倍 WAL 同步到一个令人惊讶的行为：即使 `WHERE` 条件意味着实际上没有更新任何内容，`ON CONFLICT DO UPDATE` 仍会锁定冲突的行。

Anthonin Bonnefoy (Datadog)

---

📄 [使用非 ACID 存储作为缺少自治事务的解决方法](https://postgresweekly.com/link/184121/rss)  *Pavel Stehule*

📄 [等待 Postgres 19：在线启用和禁用数据校验和](https://postgresweekly.com/link/184122/rss)  *Hubert Lubaczewski*

📄 [在 Postgres 规划器中查找不可见的 Use-After-Free 错误](https://postgresweekly.com/link/184123/rss)  *Andrei Lepikhov*

---

## 分类广告：

🚀 将您的 Postgres 生产力提高三倍。[pgEdge AI DBA Workbench](https://postgresweekly.com/link/184124/rss)：适用于任何 Postgres v14+ 的 AI 监控和诊断。[开源](https://postgresweekly.com/link/184124/rss)。

[大规模收集实时搜索数据](https://postgresweekly.com/link/184125/rss)，提供为分析师、工程师和 AI 团队构建的 API。

---

## 🛠 代码和工具

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/ellyzyxvxf7hgck3wsqi.jpg)

## [PgQue：纯 SQL + PL/pgSQL 零膨胀 Postgres 队列](https://postgresweekly.com/link/184126/rss)

来自一位长期的 Postgres 贡献者，这是 Skype 的 [PgQ](https://postgresweekly.com/link/184127/rss) 的现代版本，以 *'一个 SQL 文件 + `pg_cron`'* 的形式呈现。在架构上更接近 Kafka 而不是典型的作业队列，零事件表膨胀，原生扇出，没有 `SKIP LOCKED`。

Nikolay Samokhvalov

💡 PgQue 在 Hacker News 上引起了[一些讨论](https://postgresweekly.com/link/184128/rss)，Nikolay 回答了各种问题。

---

## [Apache Cloudberry 2.1：基于 Postgres 的 MPP 数据库](https://postgresweekly.com/link/184129/rss)

MPP（大规模并行处理）数据库将数据和查询执行分散到多个节点上；对于分析工作负载来说是一大优势。Cloudberry 继续了 [Greenplum](https://postgresweekly.com/link/184130/rss) 开始的工作，但基于更现代的 Postgres 内核。[GitHub 仓库](https://postgresweekly.com/link/184131/rss)。

Apache Software Foundation

---

## 🔥 [pg_roast：审计并"吐槽"您数据库的扩展](https://postgresweekly.com/link/184132/rss)

基于《[PostgreSQL Mistakes and How to Avoid Them](https://postgresweekly.com/link/184133/rss)》一书的原则构建。

Samir Ketema

---

- 🔎 [pg-index-health-sql 0.40](https://postgresweekly.com/link/184134/rss) – 用于分析和维护索引和表的 SQL 查询。[pg-index-health 0.40](https://postgresweekly.com/link/184135/rss) 是相同功能的 Java 库版本。

- [credcheck 4.7](https://postgresweekly.com/link/184136/rss) – 在用户创建、重命名和密码更改期间验证凭据的扩展。

- [pgwire 0.39](https://postgresweekly.com/link/184137/rss) – Postgres 线协议的 Rust 库，用于编写 Postgres 兼容的服务器和客户端。

- [PostgREST 14.10](https://postgresweekly.com/link/184138/rss) – 从 Postgres 数据库提供完全 RESTful API。

- [River 0.35](https://postgresweekly.com/link/184139/rss) – 使用 Postgres 的 Go 健壮作业处理系统。

- [PgDoorman 3.5](https://postgresweekly.com/link/184140/rss) – 用 Rust 构建的多线程连接池。