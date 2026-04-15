---
layout: post
title: PostgreSQL 每周新闻 2026-4-15
---
### PostgreSQL每周新闻#644 - 2026年4月15日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/644)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/rprmypqe54vw7gcclpxq.jpg)

## [保持 Postgres 队列健康](https://postgresweekly.com/link/183789/rss)
在 Postgres 中运行作业队列效果很好（["就用 Postgres！"](https://postgresweekly.com/link/183790/rss)），直到长时间运行的分析查询静默地阻止 autovacuum 跟上。本文介绍了实际发生的情况以及你可以做什么，以及 PlanetScale 自己的内部解决方案。

Simeon Griggs (PlanetScale)


## [你为所有其他用途扩展 Postgres。为什么不为分析扩展？](https://postgresweekly.com/link/183788/rss)
TimescaleDB 添加了超表、95% 压缩率和连续聚合，使 Postgres 能够处理实时数据上的分析。无需第二个数据库、无需管道、无需新的查询语言。你已经在编写的相同 SQL。[免费开始构建](https://postgresweekly.com/link/183788/rss)。

Tiger Data (creators of TimescaleDB) 赞助商


## [使物化视图刷新从 O(total) 变为 O(delta)](https://postgresweekly.com/link/183791/rss)
每次刷新[物化视图](https://postgresweekly.com/link/183792/rss)时，即使只有一行发生了变化，它也会重新计算整个数据集。一个正在 `pgsql-hackers` 上[讨论](https://postgresweekly.com/link/183793/rss)的补丁为 `REFRESH MATERIALIZED VIEW` 添加了 `WHERE` 子句，因此刷新只触及更改的行。这篇文章包括立即和延迟维护的触发器模式，即使补丁未进入核心代码也很有用。

Adam Brusselback

💡 [pg_ivm](https://postgresweekly.com/link/183794/rss) 作为扩展提供类似的功能，尽管对支持的 SQL 语法有更严格的限制。


## [理解 Postgres 等待事件](https://postgresweekly.com/link/183795/rss)
当查询变慢或数据库受 CPU 限制时，Postgres 已经知道原因。`pg_stat_activity` 视图公开了*等待事件*，显示每个会话在任何给定时刻被阻塞的确切原因。

Richard Yen


## [检查点、写入风暴和你](https://postgresweekly.com/link/183796/rss)
当 Postgres 被迫提前检查点（通常是在达到 `max_wal_size` 时），它会放弃通常的节流并积极刷新，猛烈冲击磁盘 I/O。默认的 1GB WAL 限制是一个常见的触发器。

Shaun Thomas (pgEdge)

💡 在后续文章中，Jeremy Schneider 指出检查点不是写入风暴的唯一来源：[将 `autovacuum_vacuum_cost_delay` 设置为零也会触发它们。](https://postgresweekly.com/link/183797/rss)


## ['我将 Linux 内核导入了 Postgres'](https://postgresweekly.com/link/183798/rss)
一位开发者通过 [pgit](https://postgresweekly.com/link/183799/rss) 将完整的 Linux 内核历史导入 Postgres。这是对 `pgit` 的良好压力测试，*并且*现在你可以通过 `SELECT` 查询多年的 Linux 内核历史。

Oliver Seifert


## [在大规模下破坏 `pg_prewarm` 的 1 GB 限制](https://postgresweekly.com/link/183800/rss)
[pg_prewarm](https://postgresweekly.com/link/183801/rss) 可以在重启后重新加载缓冲区缓存以保持性能。**但在 Postgres 16 版本 <16.10 上**，如果 `shared_buffers` 超过约 429GB，pg_prewarm 会失败并使服务器无法访问。这里解释了原因以及如何处理。

Warda Bibi

📄 [关于索引不太明显的事情](https://postgresweekly.com/link/183802/rss) – 关于复合索引排序、列上的函数调用以及索引你永远不会查询的行的快速见解。*Jon Charter*

📄 [在生产环境中轮换 Postgres 凭证而不停机](https://postgresweekly.com/link/183803/rss) *ElyDB Team*

📄 [等待 Postgres 19：新的 `pg_get_*_ddl()` 函数](https://postgresweekly.com/link/183804/rss) *Hubert Lubaczewski*


**发布和代码：**

## [`pg_6502`：完全在 Postgres 内部运行的 6502 CPU 模拟器](https://postgresweekly.com/link/183805/rss)
每个 CPU 寄存器、每个标志和 64KB 内存都是 Postgres 表；[每个 6502 操作码都是一个存储过程。](https://postgresweekly.com/link/183806/rss)一个有趣的黑客行为，展示了你可以将 PL/pgSQL 推进到多远。

lasect


## [💳 Supabase 将 *Stripe Sync Engine* 转让给 Stripe](https://postgresweekly.com/link/183807/rss)
[Stripe Sync Engine](https://postgresweekly.com/link/183808/rss) 最初由 Supabase 创建，作为将 Stripe 账户与 Postgres 数据库同步的方式，现在是一个官方的 Stripe 项目。

Supabase


## [Skunk 1.0：用于 Scala 的纯函数式 Postgres 驱动程序](https://postgresweekly.com/link/183809/rss)
[Skunk](https://postgresweekly.com/link/183810/rss) 是一个纯函数式、非阻塞的 Scala Postgres 驱动程序，现在支持跨 JVM、JS 和 [Scala Native 0.5](https://postgresweekly.com/link/183811/rss) 的 Scala 2.13 和 3。

Michael Pilquist (Typelevel)

- 🔎 [pg_wait_tracer 0.8](https://postgresweekly.com/link/183812/rss) – 基于 eBPF 的等待事件追踪器，在内核级别观察 Postgres，而不是轮询 `pg_stat_activity`。

- [pgcollection 2.0](https://postgresweekly.com/link/183813/rss) – PL/pgSQL 的关联数组数据类型，仿照 Oracle PL/SQL 的等效功能建模。（[GitHub 仓库。](https://postgresweekly.com/link/183814/rss)）

- 🔒 [column_encrypt 4.0](https://postgresweekly.com/link/183815/rss) – 使用 AES 的透明列级加密，具有自定义加密数据类型。

- [pg_datasentinel 1.0](https://postgresweekly.com/link/183816/rss) – 丰富 `pg_stat_activity` 并添加可观察性视图的扩展。

- 🌐 [PostGIS 补丁发布](https://postgresweekly.com/link/183823/rss) – PostGIS 3.2-3.6 的错误修复和安全发布。

- 🟧 [hn-fdw](https://postgresweekly.com/link/183817/rss) – 用于查询 [Hacker News](https://postgresweekly.com/link/183818/rss) 存档的外部数据包装器。

- [pgAdmin 4 v9.14](https://postgresweekly.com/link/183819/rss) – Postgres 流行的 GUI 管理工具。

- [CloudNativePG 1.29.0](https://postgresweekly.com/link/183820/rss)

- [pg_clickhouse 0.2](https://postgresweekly.com/link/183821/rss)