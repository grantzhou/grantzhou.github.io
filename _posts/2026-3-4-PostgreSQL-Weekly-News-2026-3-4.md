---
layout: post
title: PostgreSQL 每周新闻 2026-3-4
---
### PostgreSQL每周新闻#638 - 2026年3月4日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/638)

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/yknlytt7mywqxpnydhwc.jpg)

## ⚠️ [Postgres 18.3、17.9、16.13、15.17 和 14.22 发布](https://www.postgresql.org)

一次例行周期外的更新，以修复上个月安全版本引入的回归问题。**如果您已经升级到 18.0、18.1 或 18.2，您需要特别注意**，因为需要手动步骤来使 `json_strip_nulls` 和 `jsonb_strip_nulls` 函数成为不可变函数。

`PostgreSQL Global Development Group`


## [POSETTE 的日程已发布：Postgres 活动！](https://posetteconf.com)

POSETTE 2026 是一个免费的虚拟开发者活动，将于 6 月 16-18 日举行。演讲者和日程刚刚公布！通过 4 个直播流与专家一起了解世界上最先进的开源关系数据库。[获取详情](https://posetteconf.com)。

`Microsoft` **赞助商**


## [我们家里有 `pgvector`](https://theconsensus.dev)

这是一次有趣的探索。转向 [`pgvector`](https://github.com/pgvector/pgvector) 进行向量相似性搜索是一个合理且现代的选择，但 Postgres 有一个内置扩展也可以（某种程度上）做到这一点：`cube`。Phil 还发现了一个有趣的宝藏：`model2vec`。

`Phil Eaton`


### 本周摘要：

- [PgJitter](https://github.com/pgjitter/pgjitter) 是一个有趣的实验，将不同的 JIT 后端（除了 [Postgres 的标准方法](https://www.postgresql.org/docs/current/jit.html)）引入 Postgres，以实现更快的查询编译。[📊 一些基准测试结果。](https://github.com/pgjitter/pgjitter/blob/main/doc/benchmarks.md)

- 😅 您能使用 Postgres 作为实时视频会议服务器吗？[PlanetScale 的人们实现了它。](https://planetscale.com/blog/we-built-a-video-conferencing-server-in-postgres) 一项有趣的技术成就。

- Postgres 19 的 `pg_dumpall` [正在获得以二进制格式转储的支持](https://git.postgresql.org/gitweb/?p=postgresql.git;a=commit;h=cebdf88b)，`pg_restore` 也扩展了以处理新选项（[更多信息在这里](https://www.depesz.com/2026/02/28/waiting-for-postgresql-19-add-support-for-directory-format-in-pg_dumpall/)）。

- 🇺🇸 [Postgres Conference 2026 的议程](https://postgresconf.org/conferences/2026/program/proposals)已上线，会议将于今年 4 月 21-23 日在圣何塞举行。

- [Pgbeam](https://pgbeam.com/) 是一个新的商业 Postgres 代理，针对在全球跨区域处理流量的 AWS 用户，并希望在此过程中显著降低延迟。


## [Postgres 19 即将推出：`INSERT .. ON CONFLICT .. DO SELECT`](https://www.cybertec-postgresql.com/en/insert-on-conflict-do-select/)

预览一个悄然重要的新特性，在 upsert 时检索冲突行，而不仅仅是忽略或更新它。Laurenz 通过一些示例和用例解释了为什么这比 `MERGE` 更干净、更安全。

`Laurenz Albe / CYBERTEC`


## [大部分死亡是略微活着：杀死僵尸会话](https://mydbanotebook.org/post/2026/zombie_sessions/)

*我不怕鬼！* ..但僵尸会话确实很烦人！这篇文章探讨了是什么让它们存在、如何摆脱它们，以及一些缓解措施。

`Lætitia Avrot`


📄 [理解用于实时数据分析的 Postgres 性能限制](https://tiger-data.com/blog/understanding-postgres-performance-limits-for-analytics-on-live-data/) `Matty Stratton (Tiger Data)`

📄 [使用 `pg_semantic_cache` 进行语义缓存的实践指南](https://www.pgedge.com/blog/semantic-caching-with-pg-semantic-cache) `Muhammad Aqeel (pgEdge)`

📄 [使用 PgHero 和 Docker 在 Windows 上监控 Postgres](https://www.joanfrey.ch/monitoring-postgres-on-windows-with-pghero-and-docker/) `Joan Frey`


## 📰 分类广告：

🌟 正在向 Postgres 的 MCP 服务器添加新功能。不要错过，[在 GitHub 上为项目加星](https://github.com/modelcontextprotocol/servers) 以保持最新。

📖 掌握 *Visual Studio Code*，在 [Louis Lazaris 这本充满截图的指南中学习超过 150 个基本技巧](https://vscode.tutorial-ebook.com/)。


## 🛠 代码和工具

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/zrdmufmiuafpjhjsit1c.jpg)

## [pgdsat 2.0：数据库安全评估工具](https://github.com/HexaCluster/pgdsat)

检查您的 Postgres 集群近百个安全相关事项（如文件权限、配置设置、复制设置等），包括 [CIS 合规性基准](https://www.cisecurity.org/benchmark/postgresql) 的所有建议。输出是 [这样的报告](https://hexacluster.github.io/pgdsat/pgdsat-report-postgres-16-pass.html)。

`HexaCluster Corp`


## [pgspot 0.9.2：发现 Postgres 扩展脚本中的漏洞](https://github.com/timescale/pgspot)

一个用于 SQL 脚本的分析工具，检查漏洞和最佳实践。

`Sven Klemm (Timescale)`


- 🔎 [pg_textsearch 0.6](https://github.com/paradedb/pg_textsearch) – BM25 相关性排名的全文搜索扩展。

- [pgvector 0.8.2](https://github.com/pgvector/pgvector/releases/tag/v0.8.2) – 修复并行 HNSW 索引构建的缓冲区溢出。

- [sqlx4k 1.7](https://github.com/smyrgeorge/sqlx4k) – Kotlin 的协程优先 SQL 工具包，具有编译时查询验证（支持 Postgres、MySQL 和 SQLite）。

- [pgxmock 5.0](https://github.com/pashagolub/pgxmock) – 模拟库，用于在 Go 中测试 `pgx` 行为，无需真实数据库连接。

- [postgresparser v1.1.5](https://github.com/bytebase/postgresql-parser) – 基于 ANTLR 的纯 Go Postgres SQL 解析器。

- [Pigsty 4.2](https://github.com/pgsty/pigsty) – 类似 RDS 的"包含电池"的 Postgres 发行版。

- [PGQueuer 0.26](https://github.com/janbjorge/pgqueuer) – 基于 Postgres 的 Python 作业队列库。