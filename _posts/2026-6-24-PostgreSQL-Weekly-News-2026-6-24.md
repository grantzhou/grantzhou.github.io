---
layout: post
title: PostgreSQL 每周新闻 2026-6-24
---
### PostgreSQL每周新闻#654 - 2026年6月24日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/654)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/tvcjxyzjawv5araqeimo.jpg)

## [展望 Postgres 19](https://postgresweekly.com/link/186969/rss)

*"Postgres 19 感觉是那种拥有一点点所有东西的版本，"* Craig说道。他重点关注日常 Postgres 用户将会喜欢的生活质量改进，无论是在操作层面（例如 `REPACK` 和分区改进）还是在 SQL 层面（例如 SQL/PGQ 和 `GROUP BY ALL`）。

**Craig Kerstiens**

💡 Shaun Thomas [深入探讨 Postgres 19 的序列逻辑复制](https://postgresweekly.com/link/186970/rss)。


![](https://res.cloudinary.com/cpress/image/upload/c_limit,w_480,h_480,q_auto/copm/d0e5a96d.png)

## [44 场已录制的 PostgreSQL 演讲现已可供观看](https://postgresweekly.com/link/186968/rss)

POSETTE: An Event for Postgres 2026 已经结束，但演讲内容永久保留。所有会议现已在 YouTube 上可用，因此您可以按照自己的节奏直接向 Postgres 专家学习。[访问完整的 44 场演讲播放列表](https://postgresweekly.com/link/186968/rss)。

**Microsoft | AMD** 赞助商


## [▶ Postgres 中缺少什么？](https://postgresweekly.com/link/186971/rss)

我们一直在报道 Postgres 添加的新功能，但什么是"缺失的"，为什么缺失？Bruce 涉及了从分片和连接池到列式存储和透明数据加密等各种主题。*无法观看？这里有 [PDF 格式的幻灯片](https://postgresweekly.com/link/186972/rss)。*

**Bruce Momjian**


## [Postgres 18 性能增强](https://postgresweekly.com/link/186973/rss)

Postgres 18 有许多值得回顾的增强功能和性能调整。本次介绍涵盖了跳跃扫描优化、自联接消除、autovacuum 设置等。它从 AWS 的角度出发，但其中大部分内容适用于任何使用 Postgres 18 的人。

**Jafri, Bedi, Burman and Shaik (Amazon)**


## [pg_stats: Postgres 内部统计信息如何工作](https://postgresweekly.com/link/186974/rss)

了解 [`pg_stats`](https://postgresweekly.com/link/186975/rss) 是什么，以及它如何影响查询规划器的决策。

**Richard Yen**

📄 [在 Postgres 中优化多态关联](https://postgresweekly.com/link/186976/rss) *Andrei Lepikhov*

📄 [在没有 `psql` 的情况下交付 `psql`：`neonctl` 中的纯 TypeScript 客户端](https://postgresweekly.com/link/186977/rss) *Vadim Kharitonov (Neon)*

📄 [展望 Postgres 19：查询提示](https://postgresweekly.com/link/186978/rss) *Shaun Thomas*


## 📰 分类广告：

❄️ [ColdFront Beta](https://postgresweekly.com/link/186979/rss)：自动将旧 Postgres 数据分层到 S3 上的 Iceberg。同一张表，同样的 SQL。冷数据保持可写。[开源](https://postgresweekly.com/link/186979/rss)。

像微服务一样运行 AI 代理 —— 具有自动生成 API、持久内存、基于策略的编排的代理。无需粘合代码。开源。[→ 在 GitHub 上星标](https://postgresweekly.com/link/186980/rss)。


## 🛠 代码和工具

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/q8lzgtssd0mct5obsmxx.jpg)

## [`pg_hardstorage` 1.0：一种新的备份和恢复方法](https://postgresweekly.com/link/186981/rss)

一个流优先、无需主机访问、无链式的备份工具，打包在单个二进制文件中，通过普通复制连接流式传输 WAL，实现无间隙、字节精确的 PITR。它包含 pgBackRest 和 Barman shim，因此您可以在不重写自动化的情况下将其替换进来/试用。

**Cybertec**


## [🌐 Datum：PostGIS 的本地优先空间同步](https://postgresweekly.com/link/186985/rss)

一个本地优先的同步层，将 Postgres/PostGIS 表镜像到浏览器内的 PostGIS 实例（通过基于 WASM 的 [PGlite](https://postgresweekly.com/link/186986/rss)），并通过 `NOTIFY` 实时增量同步。

**Abdulrhman Elsaed**


## [Migration Autopilot：审查数据库迁移 PR 的 GitHub Action](https://postgresweekly.com/link/186982/rss)

查看数据库迁移并检测列和表的重命名或删除、截断[以及类似问题](https://postgresweekly.com/link/186983/rss)。

**Isabelle Hue**

* [SPQR 3.0](https://postgresweekly.com/link/186987/rss) – *Stateless Postgres Query Router*，通过分片实现水平扩展。v3.0 添加了分布式查询支持、分布式和引用表，以及用于跨分片 DDL/迁移的两阶段提交。

* [pgrx v0.19](https://postgresweekly.com/link/186988/rss) – 用 Rust 构建 Postgres 扩展的框架。v0.19 添加了 Postgres 19 Beta 支持，更新了依赖项，并进行了清理。

* [pgAdmin 4 9.16](https://postgresweekly.com/link/186989/rss) – 流行的基于 Web 的 Postgres 管理工具。

* [pg_parse 0.15.0](https://postgresweekly.com/link/186990/rss) – 用于 Rust 的 Postgres SQL 解析器。