---
layout: post
title: PostgreSQL 每周新闻 2026-2-18
---
### PostgreSQL每周新闻#636 - 2026年2月18日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/636)

## [Postgres 18.2, 17.8, 16.12, 15.16 和 14.21 发布，但是..!](https://postgresweekly.com/link/180882/rss)
Postgres 的每个维护版本线都收到了更新，以修复各种错误以及五个安全问题，涉及 `oidvector`、`intarray`、`pgcrypto`、`pg_trgm`，以及一个多字节字符长度验证问题，可能导致缓冲区溢出。然而，在升级之前请查看下面的注意事项。

**PostgreSQL Global Development Group**


⚠️ 在上述发布后不久，Postgres 团队[宣布将于 2月26日发布一个周期外版本](https://postgresweekly.com/link/180883/rss)，以解决上述版本引入的回归问题。[Percona 已决定等待该版本](https://postgresweekly.com/link/180884/rss)后再发布其发行版的新版本。


## [那个分析数据库本应该是临时的](https://postgresweekly.com/link/180881/rss)
现在它有自己的管道、自己的模式、自己的问题。TimescaleDB 扩展了 Postgres，使分析可以在实时数据上运行——不需要第二个系统。支持超表、95% 压缩、连续聚合。[免费开始构建](https://postgresweekly.com/link/180881/rss)。

**Tiger Data (TimescaleDB 的创建者) 赞助商**


## [Postgres 查询中的读取效率问题](https://postgresweekly.com/link/180885/rss)
深入分析导致查询缓慢的两个原因：堆/索引膨胀和较少讨论的数据局部性问题。包含工作示例、缓冲区计数以及显示影响和如何修复的前后查询计划。

**Michael Christofides**


**简讯：**

- [Open Alliance for PostgreSQL Education](https://postgresweekly.com/link/180886/rss) 正在[寻找*技术贡献者*](https://postgresweekly.com/link/180887/rss)来帮助审查其供应商中立的 Postgres 认证考试材料。

- 🏴 Jimmy Angelakos [分享了上次 PostgreSQL Edinburgh 聚会的情况](https://postgresweekly.com/link/180888/rss) —— [下一次聚会是 3月12日](https://postgresweekly.com/link/180889/rss)，如果你想去的话。

- Roger Welin 解释了为什么 [Postgres 的"膨胀""是一个特性，而不是一个错误。"](https://postgresweekly.com/link/180890/rss)


## [Bluebox Docker：一个活跃的 Postgres 示例数据库](https://postgresweekly.com/link/180891/rss)
[Bluebox](https://postgresweekly.com/link/180892/rss) 是一个用于探索 Postgres 功能的示例数据库，具有非平凡的数据。*Bluebox Docker* 提供了预加载数据集的容器镜像，支持所有主要的 Postgres 版本，加上 `pg_cron` 作业，可以持续更新数据以测试清理、膨胀、索引使用监控等。

**Ryan Booz**


## [物化视图：何时缓存查询结果有意义（何时没有意义）](https://postgresweekly.com/link/180893/rss)
物化视图并不复杂，但要很好地使用它们需要谨慎。本指南深入探讨了重要的操作细节，通过一个具体示例，通过预计算聚合将 28 秒的查询降低到 180 毫秒。

**Umair Shahid**


📺 [语言是病毒：在 Postgres 中管理区域设置](https://postgresweekly.com/link/180894/rss) – 实用地了解 Postgres 对区域设置的支持。*Christophe Pettus*

📄 [如何在 Windows 上使用 Visual Studio 2026 编译 Postgres 扩展](https://postgresweekly.com/link/180895/rss) – 针对一项可能很棘手的任务的一些指导。*Xavier Fischer*

📄 [教 LLM 它不知道的关于 Postgres 的知识](https://postgresweekly.com/link/180896/rss) *Dave Page (pgEdge)*

📄 [子事务会影响性能吗？](https://postgresweekly.com/link/180897/rss) *Shane Borden*


## 📰 分类广告：

🔥 需要一个适用于 Postgres 的 MCP 服务器，可以用于快速原型或企业级生产 AI 应用？[github.com/pgEdge/pgedge-postgres-mcp](https://postgresweekly.com/link/180898/rss)


## 🛠 代码和工具

## [`pg_background`：在后台运行 SQL，独立于您的会话](https://postgresweekly.com/link/180899/rss)
一个在后台异步执行 SQL 命令的扩展。如果您想快速返回客户端，同时让 Postgres 继续处理任务，这很方便。与 [pg_cron](https://postgresweekly.com/link/180900/rss) 等不同，这是按需任务而不是计划任务。

**Vibhor Kumar**


## [Citus 14 发布，支持 Postgres 18](https://postgresweekly.com/link/180901/rss)
这个开源扩展（现在由 Microsoft 维护）通过在多个节点上分片表来实现水平扩展，现在支持 Postgres 18，以及它的改进，如异步 I/O、虚拟生成列、OAuth 支持等。

**Mehmet Yilmaz (Microsoft)**


## [`pg_stat_ch`：将所有指标导出到 ClickHouse 的扩展](https://postgresweekly.com/link/180902/rss)
将每个查询执行转换为约 4.6KB 的固定大小事件，并将它们流式传输到 ClickHouse。

**Kaushik Iska (ClickHouse)**


- [Postgres Language Server 0.21.0](https://postgresweekly.com/link/180903/rss) – Postgres 的 LSP 和工具，使用 `libpg_query` 实现 100% 语法兼容，为编辑器和 IDE 提供自动完成和语法高亮。

- [PGHoard 2.7.0](https://postgresweekly.com/link/180904/rss) – Aiven 的 Postgres 备份和恢复守护进程，将压缩的备份和 WAL 存储在云对象存储中。

- [pg_clickhouse v0.1.4](https://postgresweekly.com/link/180905/rss) – 从 Postgres 查询 ClickHouse 数据库。