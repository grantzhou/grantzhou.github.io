---
layout: post
title: PostgreSQL 每周新闻 2026-9-30
---
### PostgreSQL每周新闻#667 - 2026年9月30日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/667)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/cjv01ik6nyjgnpab0kla.jpg)

## [Postgres 19 Beta 4 发布](https://postgresweekly.com/link/190987/rss)

确认了[最近的开发进展](https://postgresweekly.com/link/190988/rss)，最新的测试版主要是关于移除了哪些功能，尽管也引入了大量修复。候选发布版预计将在接下来几周内发布，如果一切顺利，最终版本*可能*在 10 月发布。

**PostgreSQL Global Development Group**

💡 移除了什么？SQL/PGQ（属性图）支持、在线启用/禁用校验和、使用 `FOR PORTION OF` 的时态更新/删除、`MERGE/SPLIT PARTITIONS`，以及 `pg_get_role_ddl()`、`pg_get_tablespace_ddl()` 和 `pg_get_database_ddl()` 函数。

## [SELECT count(*) 不应该需要八秒钟](https://postgresweekly.com/link/190986/rss)

对数百万行的计数或汇总查询运行缓慢，于是你添加索引、读取副本、夜间作业。TimescaleDB 扩展了你已经在运行的 Postgres，使这些查询能在实时数据上以毫秒级返回。无需数据仓库。[获取 $1000 信用额度开始使用](https://postgresweekly.com/link/190986/rss)。

**Tiger Data（TimescaleDB 的创建者）赞助商**

## [运行时 `REPACK (CONCURRENTLY)` 的成本是多少](https://postgresweekly.com/link/190989/rss)

对 Postgres 19 的新在线表重写功能与 `pg_repack` 和 `pg_squeeze` 进行了测量。`REPACK` 速度最快，但也有一些需要考虑的缺点。

**Radim Marek**

💡 `REPACK (CONCURRENTLY)` 本周在 pgsql-hackers 上也受到了大量关注。一个[可能丢失更新的 bug](https://postgresweekly.com/link/190990/rss) 已被修复，Radim 自己的测试发现了 repack 可以吸收的并发更改数量存在[硬性限制](https://postgresweekly.com/link/190991/rss)。

**本周摘要：**

- ⚠️ [PgBouncer 1.26](https://postgresweekly.com/link/190992/rss) 解决了三个 CVE，包括两个未经身份验证的客户端可以触发的 DoS bug。它现在默认跟踪 `search_path` 和 `default_transaction_read_only`。

- Devrim Gunduz [报告](https://postgresweekly.com/link/190993/rss)称，Postgres 的官方 [Yum](https://postgresweekly.com/link/190994/rss) 和 [Zypper](https://postgresweekly.com/link/190995/rss) 仓库现在在网络上更容易导航。他还[开始在那里打包 Rust 扩展](https://postgresweekly.com/link/190996/rss)，首先是 *PostgreSQL Anonymizer*。

- Google [总结了其今年迄今为止的上游 Postgres 工作](https://postgresweekly.com/link/190997/rss)。

- Amazon Aurora [现在支持](https://postgresweekly.com/link/190998/rss) Postgres 18.6、17.11、16.15、15.19 和 14.24。

## [你的 Postgres 能承受糟糕的查询吗？](https://postgresweekly.com/link/190999/rss)

ClickHouse 比较了四个 Postgres 云服务商（包括它自己）在查询耗尽所有 RAM 时会发生什么，并解释了为什么设置 `work_mem` 无法防止这种情况。

**Kevin Biju (ClickHouse)**

## [▶ Andres Freund 谈 Linux 在哪些方面帮助和妨碍了 Postgres](https://postgresweekly.com/link/191000/rss)

来自今年[Kernel Recipes](https://postgresweekly.com/link/191001/rss) 大会的一场坦诚演讲，面向内核开发者，涵盖了 io_uring、huge pages、futexes 和 atomic writes 等主题。

**Andres Freund**

📄 [PgQ 和 PgQue：你可能需要的队列引擎](https://postgresweekly.com/link/191002/rss) — 发现膨胀的任务表并将其迁移到专用队列。*Jobin Augustine (Percona)*

📄 [使用 `ALTER FUNCTION … SET work_mem` 修复一个函数的磁盘溢出](https://postgresweekly.com/link/191003/rss) — 一个 API 变慢的原因被追踪到一个函数每天造成 150GB 的临时文件写入，但通过函数级别的设置清理了这个问题。*Dinesh Kumar (CortexRidge)*

📄 [何时为 Postgres 选择 x86 或 ARM](https://postgresweekly.com/link/191004/rss) — 如果你能做出选择，这里有一些优缺点。*Ahmed Darwich (PlanetScale)*

📄 [pgBackRest 和故障切换：为什么 `archive_mode` 很重要](https://postgresweekly.com/link/191005/rss) *Stefan Fercot*

## 📰 分类广告：

🎟️ 加入我们的 [Supabase Select](https://postgresweekly.com/link/191006/rss)，了解我们如何使用 Multigres 为 Postgres 构建下一代操作系统。[申请参加享受 25% 折扣：SUPAWEEKLY](https://postgresweekly.com/link/191006/rss)。

## 🛠 代码和工具

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/wavbvnwvp3kzshmrqsra.jpg)

## [Safe Not Safe：我的迁移安全吗？](https://postgresweekly.com/link/191007/rss)

一个有趣的副业项目，来自 Cloudflare Postgres 平台团队的前负责人，他花了多年时间审查其他团队的迁移。粘贴 SQL 迁移脚本，它会标记常见问题，使用 Postgres 自己的 SQL 解析器通过 WASM 完全在浏览器中解析。

**Vignesh Ravichandran**

## [Kafgres 0.2：在 Postgres 上实现 700 MB/s 的 Kafka 吞吐量](https://postgresweekly.com/link/191008/rss)

几周前我们介绍了这个运行在 Postgres *内部*的 Kafka 兼容代理。其作者已将其从 113 MB/s 提升到单机 700 MB/s 的写入吞吐量。

**Raynor Elgie**

- [Pgpool-II 4.7.3、4.6.8、4.5.13、4.4.18、4.3.21](https://postgresweekly.com/link/191009/rss) — 一系列安全修复，修复了七个 CVE，其中一个允许使用证书认证的客户端无需密码即可以其他用户身份登录。

- [PgDog 0.1.60](https://postgresweekly.com/link/191010/rss) — Rust 驱动的连接池和分片代理。分片 `SELECT` 查询现在快 40%。

- [pg_raw_parse](https://postgresweekly.com/link/191011/rss) — PgDog 对 Postgres 解析器的 Rust 绑定，解析速度比 `pg_query.rs` 快 20-60 倍。

- [pgBackRest 2.59.2](https://postgresweekly.com/link/191012/rss) — 备份/恢复工具，增加了 Postgres 19 beta 4 支持。

- [PLHaskell 6.0](https://postgresweekly.com/link/191014/rss) — 在 SQL 代码中编写 Haskell。现在支持 `Range` 类型。

## ✨ 最后…

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/uyyrumbtq6jmmhybqa3p.jpg)

## ["我们将原版 Doom 移植到了 SQL"](https://postgresweekly.com/link/191013/rss)

虽然不*完全*是 Postgres，但这是 Postgres 兼容的 CedarDB 团队的一个有趣项目。它将 1993 年开创性的 FPS 游戏的逻辑和渲染器运行在 SQL 中，将每一帧作为位图返回给 Python 显示。这里有一些巧妙的架构细节（渲染器使用了 89 个 CTE！）和 SQL 查询。

**Lukas Vogel (CedarDB)**