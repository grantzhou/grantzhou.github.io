---
layout: post
title: PostgreSQL 每周新闻 2026-3-25
---
### PostgreSQL每周新闻#641 - 2026年3月25日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/641)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/c8b5irmunnl1pv85xfak.jpg)

## [在 `psql` 中按 Ctrl-C 让我感到不安](https://postgresweekly.com/link/182715/rss)

当你在 `psql` 中按下 Ctrl-C 时，取消请求会通过一个单独的连接以**非加密**方式发送，即使你的主会话使用了 TLS。这篇深入分析解释了 `CancelRequest` 在协议层面的工作原理、潜在的安全风险，以及为什么它会这样运行。

**George MacKerron (Neon)**


## [深入探究 `pg_plan_advice`：Postgres 19 的查询计划"提示"功能](https://postgresweekly.com/link/182716/rss)

我们最近[介绍了 Robert Haas 的解释文章](https://postgresweekly.com/link/182717/rss)，但 Hubert 通过使用他的 [explain.depesz.com](https://postgresweekly.com/link/182718/rss) 数据集的实例进一步探讨，展示了这个新模块如何让你捕获、重放并覆盖关键的规划器决策。

**Hubert Lubaczewski**


## [Postgres 安全网关 – 检查查询和结果](https://postgresweekly.com/link/182714/rss)

在你的 PostgreSQL 前面设置第二层防御来保护敏感数据。白名单查询、检查结果、强制执行 SQL 策略，并隔离你的数据库网络。完整的双向审计跟踪。无需更改应用程序。

**Signando GmbH sponsor**


**简讯：**

- Corey Quinn 介绍了 [AWS 最近结束对 RDS 上 Postgres 13 的支持](https://postgresweekly.com/link/182719/rss)。如果你升级，要小心：这可能会破坏 [AWS Glue](https://postgresweekly.com/link/182720/rss)。

- 📘 *Supabase* 和 *Manning Publications* 发布了 [《精通 Postgres：加速你的周末项目并无缝扩展到数百万级》](https://postgresweekly.com/link/182721/rss)，一本免费电子书 *（尽管需要提供电子邮件）*。

- *PlanetScale* 推出了 [Database Traffic Control](https://postgresweekly.com/link/182748/rss) 功能，可以根据预算即时管理数据库工作流。[这里是技术层面的工作原理](https://postgresweekly.com/link/182749/rss)。

**四月活动：**

- 🇩🇪 寻找四月份参加的 Postgres 活动？前往 4 月 21-22 日在 Essen 举行的 [PostgreSQL Conference Germany 2026](https://postgresweekly.com/link/182722/rss)。

- 🇨🇳 与此同时在中国，[HOW2026 Postgres and IvorySQL Conference](https://postgresweekly.com/link/182723/rss) 将于 4 月 26-28 日在济南举行。

- 🇦🇲 最后但同样重要的是，[PGDay Armenia](https://postgresweekly.com/link/182724/rss) 的注册本周开放。活动将于 4 月 30 日在 Yerevan 举行。


## [移动一个单词如何让查询速度提升 10-50 倍](https://postgresweekly.com/link/182725/rss)

两个逻辑等价的查询（一个使用 `EXISTS ... AND NOT deleted`，另一个使用 `NOT EXISTS ... AND deleted`）导致了 32 倍的性能差异。这归结于索引使用方式的差异，这是某天可能也会困扰你的问题。

**Boguk & Samokhvalov (PostgresAI)**


## [Postgres 19 的新内置 `REPACK` 命令](https://postgresweekly.com/link/182726/rss)

*"`REPACK` 在单个命令中吸收了 `VACUUM FULL` 和 `CLUSTER` 的功能。因为这个功能与常规 VACUUM 完全不同，将其分离使用户更容易理解..."* Hubert 对这一发展非常兴奋，向我们展示了它在实践中的工作方式。

**Hubert Lubaczewski**


## [等待 Postgres 19：允许在发布中排除表](https://postgresweekly.com/link/182727/rss)

使用 `FOR ALL TABLES` 的逻辑复制发布将能够通过新的 `EXCEPT TABLE` 语法*排除特定表*。

**Hubert Lubaczewski**


## [▶ 在 Azure 上构建 Postgres 服务](https://postgresweekly.com/link/182728/rss)

Charles 领导微软 [Azure 上的 Postgres](https://postgresweekly.com/link/182729/rss) 的生产管理，他加入 Claire Giordano，解释微软在 Postgres 之上构建了*什么*、为什么，以及他们如何尊重和参与开源社区。

**Talking Postgres podcast**


📄 [EXPLAIN 的其他超能力](https://postgresweekly.com/link/182730/rss) — 看看常被忽视的选项，如 `BUFFERS`、`MEMORY`（PG18 中的新功能）、`WAL`、`SETTINGS` 和 `VERBOSE`。*Richard Yen*

📄 [调试 RDS Proxy Pinning：隐藏的 JIT 开关如何创建数千个固定连接](https://postgresweekly.com/link/182731/rss) *Richard Yen*

📄 [Postgres 17 到 18 升级指南](https://postgresweekly.com/link/182732/rss) *Ilya Kosmodemiansky (Data Egret)*


## 📰 分类广告

📌 [pgedge-postgres-mcp](https://postgresweekly.com/link/182733/rss)：AI 助手与你的数据之间的开源桥梁，具有生产级性能。

👾 一个为进行了大重写并活下来讲述故事的工程师举办的会议。[BugBash](https://postgresweekly.com/link/182734/rss) 2026，4 月 23-24 日，华盛顿特区。

使用 Aiven 的免费套餐构建并分享你的开发之旅，竞争 1,000 美元。在 3 月 31 日之前使用 #AivenFreeTier 分享你的项目。[在此处参与](https://postgresweekly.com/link/182735/rss)。


## 🛠 代码和工具

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/vtjthtgfvu2k0dek91vn.jpg)

## [TigerFS：由 Postgres 支持的文件系统](https://postgresweekly.com/link/182736/rss)

来自 [Tiger Data](https://postgresweekly.com/link/182737/rss) 的一个新项目，提供一个 FUSE/NFS 文件系统，其中每个文件都是一个表行，写入使用事务，多个用户可以并发读写，并具有完整的 ACID 保证。专为代理协调或任何使用文件的工具而设计。

**Tiger Data**


## [pg_jitter 0.2：Postgres 14-18 的替代 JIT 后端](https://postgresweekly.com/link/182738/rss)

为 Postgres 带来额外的 JIT 后端以加快查询编译（[基准测试在这里](https://postgresweekly.com/link/182739/rss)）。v0.2 增加了对字符串和 JSON 操作的 SIMD 加速、正则表达式和 `LIKE` 的加速、`CASE` 的二分搜索、Windows 支持等。

**Vladimir Churyukin**


## [介绍 `pgtui`：Postgres TUI 客户端](https://postgresweekly.com/link/182740/rss)

一个新的 Rust 和 Ratatui 驱动的 TUI，用于在 Postgres 数据库上进行基本操作。独特的想法是你使用自己的编辑器进行数据输入和编辑，使用 TOML 作为交换格式。

**Kris Warner**


## [🔎 SlowQL：SQL 静态分析器](https://postgresweekly.com/link/182741/rss)

一个 SQL 静态分析器，在危险的查询模式到达生产环境之前识别它们，提供超过 250 条规则，涵盖安全性、性能反模式和合规性。它完全离线工作，包括对 Postgres 的方言感知分析。

**makroumi**


- 🕒 [TimescaleDB 2.26.0](https://postgresweekly.com/link/182742/rss) – 流行的时间序列数据库扩展获得了一些关键的性能改进。

- 🔒 [safesession 0.1](https://postgresweekly.com/link/182743/rss) – 将会话锁定为只读的扩展。加载后，会话中的每个事务都被强制为只读。针对 AI 代理和自动化用例。

- [River 0.32](https://postgresweekly.com/link/182744/rss) – 用于 Go 的高性能 Postgres 驱动的作业处理。

- [Knex.js 3.2](https://postgresweekly.com/link/182745/rss) – 用于 Node.js 的强大 SQL 查询构建器。

- [squawk 2.44.0](https://postgresweekly.com/link/182746/rss) – Postgres 迁移的检查工具。

- [pg_clickhouse 0.1.5](https://postgresweekly.com/link/182747/rss)