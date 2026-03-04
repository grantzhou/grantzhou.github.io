---
layout: post
title: PostgreSQL 每周新闻 2026-3-4
---
### PostgreSQL每周新闻#638 - 2026年3月4日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/638)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/yknlytt7mywqxpnydhwc.jpg)

## ⚠️ [Postgres 18.3、17.9、16.13、15.17 和 14.22 发布](https://postgresweekly.com/link/181483/rss)

这是一次计划外的更新，用于修复上个月安全版本引入的回归问题。**如果你已经升级到 18.0、18.1 或 18.2，你需要特别注意**，因为需要手动执行步骤才能使 `json_strip_nulls` 和 `jsonb_strip_nulls` 函数变为不可变。

`PostgreSQL Global Development Group`


## [POSETTE 活动日程已公布：Postgres 开发者盛会！](https://postgresweekly.com/link/181482/rss)

POSETTE 2026，一个免费的虚拟开发者活动，将于 6 月 16-18 日举行。演讲者和日程刚刚公布！通过 4 个直播流与专家一起学习世界上最先进的开源关系数据库。[获取详情](https://postgresweekly.com/link/181482/rss)。

`Microsoft` **赞助商**


## [我们家里有 `pgvector`](https://postgresweekly.com/link/181484/rss)

这里有一些有趣的探索。使用 [`pgvector`](https://postgresweekly.com/link/181485/rss) 进行向量相似性搜索是一个合理的现代选择，但 Postgres 有一个内置扩展也可以（某种程度上）做到这一点：`cube`。Phil 还发现了一个有趣的工具 `model2vec`。

`Phil Eaton`


**简讯：**

- [PgJitter](https://postgresweekly.com/link/181486/rss) 是一个有趣的实验，为 Postgres 带来不同的 JIT 后端（除了 [Postgres 的标准方法](https://postgresweekly.com/link/181487/rss)），以实现更快的查询编译。[📊 一些基准测试结果。](https://postgresweekly.com/link/181488/rss)

- 😅 你能把 Postgres 用作实时视频会议服务器吗？[PlanetScale 的团队实现了它。](https://postgresweekly.com/link/181489/rss) 一个有趣的技术成就。

- Postgres 19 的 `pg_dumpall` [正在获得二进制格式转储的支持](https://postgresweekly.com/link/181490/rss)，`pg_restore` 也扩展以处理新选项（[更多信息](https://postgresweekly.com/link/181491/rss)）。

- 🇺🇸 [Postgres Conference 2026 的议程](https://postgresweekly.com/link/181492/rss)现已上线，会议将于今年 4 月 21-23 日在圣何塞举行。

- [Pgbeam](https://postgresweekly.com/link/181493/rss) 是一个新的商业 Postgres 代理，面向处理全球跨区域流量的 AWS 用户，希望显著降低延迟。


## [Postgres 19 即将推出：`INSERT .. ON CONFLICT .. DO SELECT`](https://postgresweekly.com/link/181494/rss)

预览一个悄然重要的新特性，可以在 upsert 操作中检索冲突行，而不仅仅是忽略或更新它。Laurenz 通过一些示例和用例解释了为什么这比 `MERGE` 更清晰和更安全。

`Laurenz Albe / CYBERTEC`


## [大部分死了就是稍微活着：杀死僵尸会话](https://postgresweekly.com/link/181495/rss)

*我不怕鬼！*...但僵尸会话确实很烦人！这篇文章探讨了是什么让它们存在、如何摆脱它们，以及一些缓解措施。

`Lætitia Avrot`


📄 [理解实时数据分析的 Postgres 性能限制](https://postgresweekly.com/link/181496/rss) - Matty Stratton (Tiger Data)

📄 [使用 `pg_semantic_cache` 进行语义缓存的实践指南](https://postgresweekly.com/link/181497/rss) - Muhammad Aqeel (pgEdge)

📄 [使用 PgHero 和 Docker 在 Windows 上监控 Postgres](https://postgresweekly.com/link/181498/rss) - Joan Frey


## 📰 分类广告：

🌟 正在为 Postgres 的 MCP 服务器添加新功能。不要错过，[在 GitHub 上为项目加星](https://postgresweekly.com/link/181499/rss)以保持最新。

📖 掌握 *Visual Studio Code*，从 Louis Lazaris 的[这本包含超过 150 个基本技巧的截图指南](https://postgresweekly.com/link/181500/rss)中学习。


## 🛠 代码和工具

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/zrdmufmiuafpjhjsit1c.jpg)

## [pgdsat 2.0：数据库安全评估工具](https://postgresweekly.com/link/181501/rss)

检查你的 Postgres 集群中近百个安全相关事项（如文件权限、配置设置、复制设置等），包括来自 [CIS 合规基准](https://postgresweekly.com/link/181502/rss)的所有建议。输出是[像这样的报告。](https://postgresweekly.com/link/181503/rss)

`HexaCluster Corp`


## [pgspot 0.9.2：发现 Postgres 扩展脚本中的漏洞](https://postgresweekly.com/link/181504/rss)

一个用于 SQL 脚本的分析工具，检查漏洞和最佳实践。

`Sven Klemm (Timescale)`


- 🔎 [pg_textsearch 0.6](https://postgresweekly.com/link/181505/rss) – BM25 相关性排名的全文搜索扩展。

- [pgvector 0.8.2](https://postgresweekly.com/link/181545/rss) – 修复了并行 HNSW 索引构建的缓冲区溢出。

- [sqlx4k 1.7](https://postgresweekly.com/link/181506/rss) – 协程优先的 SQL 工具包，支持 Kotlin 的编译时查询验证（支持 Postgres、MySQL 和 SQLite）。

- [pgxmock 5.0](https://postgresweekly.com/link/181507/rss) – 模拟 `pgx` 行为的 Mock 库，用于在 Go 中进行测试，无需真实数据库连接。

- [postgresparser v1.1.5](https://postgresweekly.com/link/181508/rss) – 基于 ANTLR 的纯 Go Postgres SQL 解析器。

- [Pigsty 4.2](https://postgresweekly.com/link/181509/rss) – 类似 RDS 的"全功能"Postgres 发行版。

- [PGQueuer 0.26](https://postgresweekly.com/link/181510/rss) – 基于 Postgres 的 Python 作业队列库。