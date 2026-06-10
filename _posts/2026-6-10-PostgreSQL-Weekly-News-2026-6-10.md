---
layout: post
title: PostgreSQL 每周新闻 2026-6-10
---
### PostgreSQL每周新闻#652 - 2026年6月10日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/652)

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/krjjheur4jzublurtcvw.jpg)

## [PostgreSQL 19 Beta 1 发布](https://postgresweekly.com/link/186319/rss)

Postgres 最令人兴奋的主要版本之一又近了一步，现在可以尝试图查询、更快的插入、[pg_plan_advice](https://postgresweekly.com/link/186320/rss)、并行工作线程的自动清理、[在线切换数据校验和](https://postgresweekly.com/link/186322/rss)等功能。最终版本将在9月底/10月初左右发布。

**PostgreSQL Global Development Group**

💡 准备好尝试 Postgres 19 了吗？这里介绍[如何在 Docker 中运行它](https://postgresweekly.com/link/186323/rss)或[在 Kubernetes 集群上运行](https://postgresweekly.com/link/186324/rss)。

## [参加精彩的 PostgreSQL 讲座，还有周边产品](https://postgresweekly.com/link/186318/rss)

POSETTE: An Event for Postgres 即将到来（6月16-18日）。挑选并参加您必看的讲座。加入 Discord 上的 Hallway Track，获取限量独家活动周边，供参加实时活动的任何地方的与会者使用。最后召集：[立即注册](https://postgresweekly.com/link/186318/rss)。

**Microsoft | AMD** 赞助商

### **简要新闻：**

- 📘 [官方 Postgres 19 文档](https://postgresweekly.com/link/186326/rss)现已成形，例如[这个关于属性图的页面](https://postgresweekly.com/link/186327/rss)和[草稿发布说明](https://postgresweekly.com/link/186329/rss)。

- 💰 [Supabase 已完成 5 亿美元的 F 轮融资](https://postgresweekly.com/link/186330/rss)，估值达 100 亿美元。

- Spectral Core [推出了 SQL Tran](https://postgresweekly.com/link/186331/rss)，这是一个（商业）工具，用于自动化 Oracle 到 Postgres 的迁移。

## [⚾ 比较 Postgres、DuckDB 和 LadybugDB 的图功能](https://postgresweekly.com/link/186332/rss)

一个以棒球为主题的比较，研究三个数据库在对数百万行球员、场馆和比赛数据进行图式查询时的表现（在开发者体验和原始性能方面）。

**John Nevin**

## [`EXPLAIN` Prettier（或后处理查询计划）](https://postgresweekly.com/link/186333/rss)

`EXPLAIN` 输出在最好的情况下也可能难以阅读，而且它也可能在不同机器和版本之间发生微妙的变化。Andrei 展示了 [explain_prettier](https://postgresweekly.com/link/186334/rss)，它通过去除不必要的信息使 `EXPLAIN` 输出更清晰、更简单。

**Andrei Lepikhov**

📄 [Postgres 开发者向量索引权衡指南](https://postgresweekly.com/link/186335/rss) – 了解什么是 HNSW、IVFFlat、DiskANN 和 SPFresh 索引以及何时选择每种索引。_Hien Phan (Tiger Data)_

📄 [SQL 的 `ORDER BY` 已经走了很长一段路](https://postgresweekly.com/link/186337/rss) – 从 80 年代到 ISO 规定的 SQL:2023 现在的功能之旅。_Markus Winand_

📄 [pgBackRest 能否与 `pg_tde` 配合使用？](https://postgresweekly.com/link/186338/rss) – pgBackRest 能透明地处理加密的 WAL 段吗？基本上，可以！_Stefan Fercot_

📄 [文件描述符：拖垮 Postgres 的操作系统限制](https://postgresweekly.com/link/186339/rss) _Warda Bibi_

---

## 📰 分类广告：

🧮 [在 Postgres 中构建完整的 RAG 堆栈](https://postgresweekly.com/link/186340/rss)。Docloader、Vectorizer、RAG 和 MCP。[100% 开源](https://postgresweekly.com/link/186340/rss)。

🐘 AI 编写了迁移。谁来审查它？开源多代理 PR 审查 - 每个 PR 自定义审查视角，每次运行只需几美分。[收藏并部署 →](https://postgresweekly.com/link/186341/rss)

---

## 🛠 **代码和工具**

## [Absurd: Postgres 原生的持久工作流系统](https://postgresweekly.com/link/186342/rss)

被描述为_"你能想到的最简单的持久执行工作流系统"_，Absurd 是[一个 SQL 文件](https://postgresweekly.com/link/186343/rss)，在常规 Postgres 上实现了多步骤任务/队列/工作线程系统。有 [SDK](https://postgresweekly.com/link/186344/rss) 可以让从 TypeScript、Python 和 Go 中轻松使用它。

**Armin Ronacher (Earendil)**

## [Multigres v0.1 Alpha: Postgres 的"操作系统"](https://postgresweekly.com/link/186345/rss)

一年前，[Supabase 宣布](https://postgresweekly.com/link/186346/rss)聘请 Vitess 的联合创始人开发一个类似 Vitess 的水平扩展数据库集群系统，但用于 Postgres。这个 alpha 版本是他们正在构建的内容的早期公开预览。

**Sugu Sougoumarane**

- [TimescaleDB 2.27](https://postgresweekly.com/link/186347/rss) – Tiger Data 的时间序列扩展继续关注性能，特别是对压缩数据的更高效操作。

- [pg_clickhouse 0.3](https://postgresweekly.com/link/186348/rss) – 用于从 Postgres 查询 ClickHouse 数据库的 FDW。底层的 C++ 库被替换为更快、更稳健的 C 替代方案。

- [pg_background 2.0](https://postgresweekly.com/link/186349/rss) – 在后台工作线程中运行 SQL。现在可与 Postgres 19 配合使用。

- [Kanel 4.0](https://postgresweekly.com/link/186350/rss) – 从实时 Postgres 数据库生成 TypeScript 类型。

- [pgrls](https://postgresweekly.com/link/186351/rss) – RLS（行级安全性）的静态分析器，用于捕获常见的策略错误。

- [NeonD](https://postgresweekly.com/link/186352/rss) – 基于 Neon 的开源 Postgres 控制平面守护进程，作为单个 Docker 容器运行。

- [pgcheck](https://postgresweekly.com/link/186353/rss) – 用 Go 编写的轻量级 Postgres 健康检查 CLI。