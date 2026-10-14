---
layout: post
title: PostgreSQL 每周新闻 2026-10-14
---
### PostgreSQL每周新闻#669 - 2026年10月14日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/669)

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/gn9k4gm9cggzc04p2iws.jpg)

## [pg_vectorsearch: 基于分区的 HNSW 替代方案](https://postgresweekly.com/link/191510/rss)

一个向量搜索扩展，使用 PRISM 向量索引，它扫描压缩的 k-means 分区而不是像 HNSW 那样遍历图，并可用于现有的 `pgvector` 列。它目前处于 alpha 阶段，需要 Postgres 18+，同时 [pgvectorscale](https://postgresweekly.com/link/191511/rss) 进入维护模式。

Erik Nordström et al. (Tiger Data)


## [Agent Memory: 原始检索 VS. 提取事实，已测试](https://postgresweekly.com/link/191509/rss)

Redis 在 LongMemEval 上重新运行了 agent memory 系统。已发布的分数与重现结果相差高达 28 分，将原始对话检索与提取事实配对比单独使用任一方法都更好。查看数据、成本和方法。

Redis `赞助商`


## [Savepoints 如何限制我们的 Postgres 队列](https://postgresweekly.com/link/191512/rss)

一篇技术性文章，配有一些相当精美的可视化效果，讲述了如何为基于 Postgres 的队列添加更多 workers 却因为每个作业的 `SAVEPOINT` 而使其变慢（以及使用租约声明作业如何解决了这个问题）。

Rory Malcolm (incident.io)


**本周摘要：**

- ⭐ [Postgres 19 的发布被推迟](https://postgresweekly.com/link/191513/rss)到 11 月 19 日，11 月 12 日将发布额外的 RC2 以包含更多近期修复。第一个候选版本仍将于明天（10 月 15 日）发布。

- ⚠️ [PgBouncer 1.26.1](https://postgresweekly.com/link/191514/rss) 修复了三个 CVE，最严重的是当使用 SCRAM 认证时，知道一个用户密码的客户端可以以不同用户（甚至超级用户）的身份登录。


## ['回滚将持续到士气改善为止'](https://postgresweekly.com/link/191515/rss)

一位 Postgres 提交者（他自己的工作也在其中受到影响）分享了他对为什么在 beta 期间有这么多 Postgres 19 功能被回滚的看法。

Peter Eisentraut

📊 与此同时，Kaarel Moppel [对 Postgres 19 betas 进行了 800 小时的基准测试](https://postgresweekly.com/link/191516/rss)，发现在 OLTP 工作负载上它比 v18 快几个百分点。


## [不要依赖 `SELECT` 顺序：随机打乱你的行，看看会出什么问题](https://postgresweekly.com/link/191517/rss)

如果你的应用或测试隐式依赖于按插入顺序返回的行，这可能会导致许多烦人的 bug（我自己也曾被咬过！）。[pg_disorder](https://postgresweekly.com/link/191518/rss) 扩展会打乱缺少 `ORDER BY` 的 `SELECT` 结果，以在测试中捕获此类 bug。

Yaroslav Kurbatov (Evil Martians)


## [删除行对表的影响](https://postgresweekly.com/link/191519/rss)

一个简洁的解释和演示，涵盖了一个常见的误解。删除表中一半的行，然后运行 `VACUUM`，表在磁盘上仍占用 137 MB，只有 `VACUUM FULL` 才能回收它。

Hollis Varden

📄 [为什么将 `archive_command` 设置为 `/bin/true` 会导致数据丢失](https://postgresweekly.com/link/191520/rss) – 这个"修复"满 WAL 磁盘问题的方法会在没有警告的情况下破坏恢复。*Shaun Thomas*

📄 [PgBouncer 池化模式实践](https://postgresweekly.com/link/191521/rss) – 事务池化对 advisory locks 的影响。*Oskar Dudycz*

📄 [PgBouncer vs. Amazon RDS Proxy: 两种池化工具的差异](https://postgresweekly.com/link/191522/rss) *Wood and Chiba (AWS)*

📄 [TABLESAMPLE 如何选择行](https://postgresweekly.com/link/191523/rss) *Radim Marek*


## 📰 分类广告：

RDST 的始终在线代理监视每个 PG 查询，自动向你发送已解释的修复，并在应用后验证它们是否有效。[让代理在你的 Postgres 数据库上工作。它是免费的](https://postgresweekly.com/link/191524/rss)。

⚡ [Rebase](https://postgresweekly.com/link/191525/rss): 一个用于 Postgres 的开源后端。REST、类型化 SDK、认证、实时、存储和一个你不必构建的管理面板。

[试用 ClickHouse Managed Postgres](https://postgresweekly.com/link/191526/rss): 对于 I/O 密集型工作负载，在本地 NVMe 上快达 10 倍，并与原生 ClickHouse 集成。


## 🛠 代码和工具

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/h6i6uifi9p9kdurhphne.jpg)

## [pg-delta: 将 Postgres 模式差异转换为有序迁移](https://postgresweekly.com/link/191527/rss)

Supabase 的新开源模式差异引擎。将它指向两个 Postgres 14-18 数据库，就能得到涵盖 RLS 策略、权限和域的有序迁移。它取代了已弃用的 `migra`，但仍处于 *alpha* 阶段。

Valleteau and Xie (Supabase)


## [asyncpg 0.32.0: Python/asyncio 的快速 Postgres 客户端库](https://postgresweekly.com/link/191528/rss)

这个长期存在的用于 `asyncio` 框架的 Python 客户端库现在支持 Postgres 19，以及新发布的 Python 3.15。

MagicStack


## [Orafce: Postgres 的 Oracle 兼容性函数](https://postgresweekly.com/link/191529/rss)

实现了一些 Oracle 函数，这些函数对于迁移到 Postgres 的用户可能有用。我们已经好几年没有链接这个项目了，但它仍在频繁发布。

Orafce Project

- [wal2json 2.7](https://postgresweekly.com/link/191530/rss) – 一个逻辑解码插件，将行更改输出为 JSON，被许多变更数据捕获设置使用。这是两年多来的第一个版本，添加了 Postgres 18 和 19 支持。

- [PGQueuer 1.6](https://postgresweekly.com/link/191532/rss) – 一个构建在 Postgres 上的 Python 作业队列库。

- [Squawk 2.68](https://postgresweekly.com/link/191531/rss) – 一个用于 Postgres 模式迁移的 linter。