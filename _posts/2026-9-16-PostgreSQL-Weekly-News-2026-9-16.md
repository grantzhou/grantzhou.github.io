---
layout: post
title: PostgreSQL 每周新闻 2026-9-16
categories: [PostgreSQL]
tags: [PGWeekly]
---
### PostgreSQL每周新闻#665 - 2026年9月16日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/665)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/fs6z3yph6p3jzdk4akbg.jpg)

## [Tom Lane 谈 30 年的 Postgres 架构](https://www.snowflake.com/en/blog/engineering/30-years-of-postgres-architecture-tom-lane/)
这位高产的 Postgres 核心团队成员（他还共同编写了原始的 PNG 规范！）在这里讨论了很多内容，包括为什么 Postgres 使用进程而不是线程、可靠性、MVCC，以及为什么 v13 是他最不喜欢的版本。还有[▶️ 一小时完整访谈视频](https://www.youtube.com/watch?v=2ajXkLeVXxQ)。

`Elizabeth Garrett Christensen and Tom Lane`

## [Render 在您的应用旁运行 Postgres](https://dashboard.render.com/register?utm_source=email&utm_medium=newsletter&utm_campaign=2026_newsletter_cooperpress&utm_content=pg_weekly)
几秒钟内启动一个生产就绪的 Postgres 数据库。通过私有网络从 Web 服务、后台工作进程和代理工作流连接，所有这些都在一个平台上。无需运维开销即可管理备份、扩展和高可用性。[免费开始，按需扩展](https://dashboard.render.com/register?utm_source=email&utm_medium=newsletter&utm_campaign=2026_newsletter_cooperpress&utm_content=pg_weekly)。

`Render` **赞助商**

## [分片 Postgres 查询的生命周期](https://planetscale.com/blog/the-lifecycle-of-a-sharded-postgres-query)
PlanetScale 已经[推出了 Neki](https://planetscale.com/blog/introducing-neki)，这是一个分片 Postgres 系统，其中路由器使用有线协议并跨标准 Postgres 服务器的分片规划查询。不过，这篇图解演练更有趣。

`PlanetScale Team`

💡 PlanetScale [尚未决定](https://news.ycombinator.com/item?id=49646445) Neki 是否会开源。[Citus](https://github.com/citusdata/citus) 是成熟的开源分布式 Postgres 选项，采用更集成的基于扩展的方法。

**本周摘要：**

- [postgres-contrib.org 现在有了提交表单](https://postgres-contrib.org/post/96/)，用于告知他们非代码的 Postgres 贡献（演讲、聚会、翻译、评审、指导）。无需账号或邮箱。

- 🇨🇳 你会说中文吗？Ruohang Feng [推出了 `pgsql.cc`](https://vonng.com/en/pg/pgsql-cc-online/)，一个中文 Postgres 网站，提供 11 个版本的完整中文文档。

- 🇨🇭 [CERN PGDay 2027](https://www.swisspug.org/cern-pgday-2027.html) 将于 2027 年 2 月 12 日在日内瓦 CERN 举行。[征稿](https://indico.cern.ch/event/1720940/abstracts/)截止到 11 月 8 日。

- 🇪🇺 [PGConf.EU 2026](https://2026.pgconf.eu/) 将于 10 月 20-22 日在西班牙瓦伦西亚举行，仅剩一个月。

## [Postgres 19 中的计划建议](https://tapoueh.org/blog/2026/09/plan-advice-in-postgresql-19/)
两个新模块 `pg_plan_advice` 和 `pg_stash_advice` 允许您捕获规划器建议、有选择地强制执行，并通过查询 ID 自动应用建议。Dimitri 展示了工作流程。

`Dimitri Fontaine`

## ["再加一个索引"的难以承受之轻](https://boringsql.com/posts/unbearable-lightness-of-one-more-index/)
在热表上添加索引来解决问题似乎是明智的，但随着索引的积累，成本会迅速增加。这篇文章探讨了其中的权衡以及如何评估它们。

`Radim Marek`

## [📊 28 年来的 Postgres 开发活动](https://vondra.me/posts/postgres-development-activity/)
通过图表，Tomas 展示了 `pgsql-hackers` 邮件列表随着时间的推移变得更加繁忙，而提交和插入/删除行为一直在缓慢稳定地增长。

`Tomas Vondra`

## [在 Amazon Aurora PostgreSQL 中排查行锁争用问题](https://aws.amazon.com/blogs/database/troubleshooting-row-lock-contention-in-amazon-aurora-postgresql-part-1-understanding-row-lock-contention-in-postgresql/)
如何使用内置视图、`pgrowlocks` 和锁等待日志跟踪行锁争用。[第二部分](https://aws.amazon.com/blogs/database/resolve-amazon-aurora-postgresql-lock-contention-with-database-insights-part-2/)介绍使用 AWS 工具定位争用，然后探讨修复方法。

`Kumar and Manivasakan (Amazon)`

📄 [优化聚合函数：扩展能做什么？](https://www.pgedge.com/blog/optimising-postgresql-aggregates-what-can-an-extension-do) – 使用 Postgres 19 的新规划器钩子原型，从 `SUM(x ORDER BY x)` 中剥离不必要的排序。*Andrei Lepikhov*

### 📰 分类广告

🎟️ 加入我们的 [Supabase Select](https://supabase.link/JKX1Ifb)，了解我们如何使用 Multigres 为 Postgres 构建下一代操作系统。[申请参加享受 25% 折扣：SUPAWEEKLY](https://supabase.link/JKX1Ifb)。

---

🧊 为无人阅读的数据支付 SSD 价格？[ColdFront 自动将旧 Postgres 行分层到 S3](https://github.com/pgEdge/coldfront)，开源方式。

## 🛠 代码和工具

## [pgrust 0.3：Postgres 的 Rust 重写版本，现已可供试用](https://pgrust.com/blog/pgrust-v0-3/)
这是 Postgres 的 Rust 重新实现的一个值得注意的里程碑，邀请您在实际工作负载上试用（在非关键环境中！）。[v0.3](https://github.com/malisper/pgrust/releases/tag/v0.3) 现在跟踪 Postgres 18.6，专注于可靠性。还有[基于浏览器的演示](https://pgrust.com/)，因此您无需安装即可试用。[GitHub 仓库](https://github.com/malisper/pgrust)。

`Michael Malis`

## [WalShadow：从物理 WAL 将 Postgres 复制到 ClickHouse](https://clickhouse.com/blog/introducing-walshadow)
一个新的开源引擎，无需逻辑解码即可将 Postgres 数据复制到 ClickHouse。ClickHouse 报告约 200ms 的提交到可见延迟。

`Sai Srirampur (ClickHouse)`

## [PostgreSQL Migrator 1.0：将 Oracle 和 MySQL 迁移到 Postgres](https://blog.dalibo.com/2026/09/07/postgresql-migrator-1-en.html)
用于迁移 Oracle 和 MySQL/MariaDB 数据库的单一二进制工具，带有用于发现问题的 Web UI 和基于快速 `COPY` 的数据传输。

`Étienne Bersac (Dalibo)`

- [OrioleDB beta17](https://github.com/orioledb/orioledb/releases/tag/beta17) – Supabase 的 Postgres 替代存储引擎增加了 btree 索引的 `CREATE INDEX CONCURRENTLY` 和 `REINDEX CONCURRENTLY`、页面校验和以及跨主要版本的 `pg_upgrade` 支持。

- [pgstream 1.5](https://github.com/xataio/pgstream/releases/tag/v1.5.0) – Postgres 的 CDC，也复制 DDL 和模式更改。

- [PostgREST 16.3](https://github.com/PostgREST/postgrest) – 从任何现有数据库提供完全 RESTful 的 API。

- [pgmq 1.13.0](https://github.com/pgmq/pgmq/releases/tag/v1.13.0) – 轻量级消息队列扩展。