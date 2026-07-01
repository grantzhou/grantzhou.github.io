---
layout: post
title: PostgreSQL 每周新闻 2026-7-1
---
### PostgreSQL每周新闻#655 - 2026年7月1日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/655)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/crih5wm9tpxdxxxon0jl.jpg)

## [对 Postgres 有影响的新 SQL 标准特性](https://postgresweekly.com/link/187277/rss)

Postgres 贡献者和 SQL 标准委员会成员 Peter Eisentraut 报告了最新的标准化会议情况，会议中 `QUALIFY`、`INSERT ... BY NAME` 和 `JOIN TO ONE` 被采纳进入标准草案。此外还有关于仍在讨论中的 'key joins' 提案的更新。

Peter Eisentraut

💡 Peter 指出："PostgreSQL 20 开发周期即将启动，这篇文章包含了处于不同阶段的一些项目想法，如果有人想参与的话。"

## [购买和升级 EDB Postgres，无需销售电话](https://postgresweekly.com/link/187276/rss)

购买或升级 Postgres 过去意味着需要销售电话和合同。现在你可以自己完成。该商店让技术团队按照自己的条件进行购买和扩展，无需等待报价。[选择你的产品并结账](https://postgresweekly.com/link/187276/rss)。

EDB **赞助商**

## [为什么缓慢的 Postgres 检查点使重启变得危险](https://postgresweekly.com/link/187278/rss)

重启一个遇到困难的 Postgres 实例看起来像是一个安全的操作，但一位资深工程师解释了为什么它可能恰恰相反，并使用了两个真实的、在有检查点问题的数据库上发生的长时间停机案例。他还分享了一个实用的告警起始阈值，这样你就不必通过艰难的方式来学习。

Jeremy Schneider

**简讯：**

- [PGlite](https://postgresweekly.com/link/187279/rss)，一个用于 JavaScript 环境的 Postgres WebAssembly 构建版本，[庆祝达到每周 1000 万次下载](https://postgresweekly.com/link/187280/rss)，同时解释了使用场景以及如何自己开始使用它。

- ClickHouse [推出了 WAL-RUS，一个基于 Rust 重写的 WAL-G](https://postgresweekly.com/link/187281/rss)，以在长时间运行的归档进程中获得更可预测的内存使用。

- 🇺🇸 [Postgres Summit US](https://postgresweekly.com/link/187282/rss) 的门票销售现已开放，该会议将于今年秋季在纽约市举行。[现在可以购票](https://postgresweekly.com/link/187283/rss)。

## [在 Amazon Aurora 上生产环境运行 `pgvector`](https://postgresweekly.com/link/187284/rss)

一份关于使用 [pgvector](https://postgresweekly.com/link/187285/rss) 的详细指南，涵盖索引选择、量化、查询操作符到配置设置和运维方面。它专注于 Aurora，但对于其他环境中的现有和潜在 pgvector 用户仍然非常有用。

Aichholzer and Pareek (AWS)

## [太多的表对你不利](https://postgresweekly.com/link/187286/rss)

来自 Laurenz 的一个新的性能咨询故事。这次展示了拥有太多表不仅会激增内存使用，还会减慢针对 Postgres 自身系统目录的查询。

Laurenz Albe

## [▶ POSETTE 2026 的 44 场演讲](https://postgresweekly.com/link/187287/rss)

Microsoft 在 YouTube 上分享了其最近的 POSETTE 虚拟 Postgres 会议的所有演讲。亮点包括：

- [Postgres 19 黑客小组](https://postgresweekly.com/link/187288/rss) – 四位 Postgres 贡献者讨论 Postgres 的开发和发布流程。什么能够被采纳，如何采纳，为什么？还预告了一些未来的 Postgres 特性。
- [PostgreSQL 黑客指南](https://postgresweekly.com/link/187289/rss) – 一个有用的介绍，关于如何参与 Postgres 代码库的工作。
- [在 Postgres 中使用 Apache AGE 查询和可视化图](https://postgresweekly.com/link/187290/rss)
- [JSON：邪恶的数据类型还是只需要被驯服？](https://postgresweekly.com/link/187291/rss)
- [为你的 Postgres 数据库建立 MCP](https://postgresweekly.com/link/187292/rss)

Microsoft

📄 [为什么在 Postgres 表中间添加列如此困难](https://postgresweekly.com/link/187293/rss) Tianzhou (Bytebase)

📄 [在 Postgres 19 中使用 `WAIT FOR LSN` 读取你自己的写入](https://postgresweekly.com/link/187294/rss) Redowan Delowar

---

📰 分类广告：

PostgreSQL 即服务，具有混合搜索、令牌预算、流式 API，无供应商锁定。[在 pgEdge Cloud 上试用](https://postgresweekly.com/link/187295/rss)。

---

**发布和代码：**

## [🤖 pgrust：AI 辅助的 Postgres Rust 重写](https://postgresweekly.com/link/187296/rss)

它还没有准备好用于生产环境，AI 完成了大部分工作，但能够看到产生一个通过 Postgres 自身回归测试的实现是可能的，这很酷。作者已经启动了[一个 Web 编译的演示](https://postgresweekly.com/link/187297/rss)，你可以试用一下。

Michael Malis

💡 pgrust 不仅仅是一个"Claude，用 Rust 为我重新实现 Postgres"的项目。Michael 已经[撰写博客介绍了涉及的内容](https://postgresweekly.com/link/187298/rss)以及[自四月以来的进展](https://postgresweekly.com/link/187299/rss)。他有*八个* Codex 账户在并行运行！

## [Noisia 0.3：针对 Postgres 的*有害工作负载*生成器](https://postgresweekly.com/link/187300/rss)

创建诸如死锁、无操作的事务以及产生磁盘临时文件的查询等内容，用于压力测试你的设置。请谨慎使用！最新版本添加了一个['backend killer' 工作负载](https://postgresweekly.com/link/187301/rss)（通过 OOM）和一个['slot-bloat' 工作负载](https://postgresweekly.com/link/187302/rss)。

Alexey Lesovsky

## [Biscuit：高性能模式匹配索引](https://postgresweekly.com/link/187303/rss)

一个实验性的专门索引访问方法，用于加速 `LIKE`/`ILIKE` 模式匹配。

Sivaprasad Murali

- [pgtt 4.5](https://postgresweekly.com/link/187304/rss) – 创建和管理 Oracle 风格的全局临时表。v4.5 添加了 Postgres 19 和 `CREATE INDEX CONCURRENTLY` 支持。

- [PGSync 7.1.0](https://postgresweekly.com/link/187305/rss) – Postgres 到 Elasticsearch/OpenSearch 的同步。

- [pgvector 0.8.4](https://postgresweekly.com/link/187285/rss) – 针对 HNSW 清理的两个小修复。