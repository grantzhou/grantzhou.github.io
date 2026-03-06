---
layout: post
title: PostgreSQL 每周新闻 2026-2-4
---
### PostgreSQL每周新闻#634 - 2026年2月4日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/634)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/fulaqn5qgibbp3etaljc.jpg)

## [Hackorum：`pgsql-hackers` 的论坛式视图](https://postgresweekly.com/link/180185/rss)
[`pgsql-hackers`](https://postgresweekly.com/link/180210/rss) 是构建 Postgres 的邮件列表。这是必读内容，但在网页上浏览非常痛苦。Hackorum 通过现代论坛风格的用户界面解决了这个问题，具有线程化、用户资料、统计数据、一键补丁下载等功能。

**Kai Wagner (Percona)**

💡 Kai 在[这里分享了关于 Hackorum 的更多背景信息](https://postgresweekly.com/link/180187/rss)。


## [重新利用 `SECURITY LABELS`：在不修改核心代码的情况下为 Postgres 添加自定义元数据](https://postgresweekly.com/link/180188/rss)
一种实用且巧妙的技术，使用我之前从未遇到过的 Postgres 功能：[SECURITY LABEL](https://postgresweekly.com/link/180189/rss)，为数据库对象附加自定义元数据。非常聪明！

**Andrei Lepikhov (pgEdge)**


## [您不需要第二个数据库来进行分析](https://postgresweekly.com/link/180184/rss)
数据管道、回填、同步延迟、数据漂移。这就是将分析与操作数据库分离的成本。TimescaleDB 扩展了 Postgres，使分析可以在实时数据上运行，无需第二个系统。留在 Postgres。在 Postgres 上扩展。[免费开始构建](https://postgresweekly.com/link/180184/rss)。

**Tiger Data sponsor**


## [规划耗时 500 毫秒？统计数据如何使查询速度减慢 20 倍](https://postgresweekly.com/link/180190/rss)
了解查询如何在 2 毫秒内运行，却需要 500 毫秒来规划，这要归咎于 Postgres 优化器的次优操作。幸运的是，有解决方案。

**Andrei Lepikhov**


## [Postgres 18 开发背后的公司](https://postgresweekly.com/link/180191/rss)
我很高兴得知 Sophie Alpert 最近修复了一个可以追溯到 1999 年的 Postgres 错误！这只是对 Postgres 18 参与者分析的一个亮点。EnterpriseDB 在提交数量上获胜，而 Postgres Professional 拥有最大的团队（约 260 名贡献者中的 30 名）。

**Phil Eaton (The Consensus)**


## [检查点调优的重要性（和好处）](https://postgresweekly.com/link/180192/rss)
凭借确凿的基准数据，Jobin 实际演示了为什么以及如何值得在更长的时间段内分散 Postgres 检查点。

**Jobin Augustine**


## [▶ 如何与其他 Postgres 人员合作](https://postgresweekly.com/link/180193/rss)
是什么让团队点击？在 PGConf.EU 2025 上，Jimmy Angelakos、Floor Drees、Karen Jex 和 Boriss Mejias 深入探讨了技术的人性化方面——团队动态、神经多样性，以及一些可以产生重大影响的小变化。

**Jimmy Angelakos et al.**


## [用 Rust 替换 Protobuf 以获得 5 倍速度提升](https://postgresweekly.com/link/180194/rss)
为了追求速度，[PgDog](https://postgresweekly.com/link/180195/rss) Postgres 扩展代理的创建者撕掉了 [pg_query.rs](https://postgresweekly.com/link/180196/rss) 用于与基于 C 的 `libpg_query` 库交互的 Protobuf 机制，并编写了 6,000 行直接的 C 到 Rust 绑定。结果：查询解析速度提高 5-10 倍。

**Lev Kokotov**


📄 [相同的 SQL，不同的结果：Oracle 与 Postgres 迁移的微妙错误](https://postgresweekly.com/link/180197/rss) – 对迁移工作有价值的来之不易的实际经验知识。*Deepak Mahto*

📄 [10 个 Elasticsearch 生产问题（以及 Postgres 如何避免它们）](https://postgresweekly.com/link/180198/rss) – 对 Postgres 相当有偏见，但我们确实喜欢 [pg_textsearch](https://postgresweekly.com/link/180199/rss)。*Raja Rao DV (Tiger Data)*


---

## 📰 分类广告：

💬 使用 pgEdge MCP 服务器将 LLM 连接到任何标准 Postgres 数据库。Beta 2 现已发布：https://github.com/pgEdge/pgedge-postgres-mcp

更快修复错误。[AppSignal 提供令人愉悦的性能监控。](https://postgresweekly.com/link/180201/rss) 免费试用，无需信用卡。


---

## 🛠 代码和工具

## [Pigsty v4.0 发布](https://postgresweekly.com/link/180202/rss)
['batteries-included' PostgreSQL 发行版](https://postgresweekly.com/link/180203/rss)的主要版本，带来 Postgres 18 支持，回归到 Apache 2.0 许可证，并包含更多即用型 Postgres 扩展。

**Ruohang Feng**


## [pg_textsearch 0.5：BM25 排名的文本搜索扩展](https://postgresweekly.com/link/180199/rss)
为 Postgres 中的全文搜索带来 [BM25](https://postgresweekly.com/link/180204/rss) 排名。[v0.5](https://postgresweekly.com/link/180205/rss) 的主要新增功能是并行索引构建。多个工作进程 == 更快索引大表。

**Tiger Data**


## [Reshape 0.8：零停机时间模式迁移工具](https://postgresweekly.com/link/180206/rss)
在迁移期间，Reshape 确保新旧模式同时可用，允许您逐步推出应用程序。

**Fabian Lindfors**


- [pgagroal 2.0](https://postgresweekly.com/link/180207/rss) – 高性能连接池现在拥有更快的新 I/O 框架。

- 🌐 [Martin 1.3](https://postgresweekly.com/link/180208/rss) – 从 PostGIS、PMTile 和 MBTile 文件即时生成和提供矢量切片。

- [IvorySQL 5.0](https://postgresweekly.com/link/180209/rss) – Oracle 兼容的 Postgres。