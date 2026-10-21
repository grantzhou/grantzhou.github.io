---
layout: post
title: PostgreSQL 每周新闻 2026-10-21
---
### PostgreSQL每周新闻#670 - 2026年10月21日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/670)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/g1qnzow76mrbuxqpi5rj.jpg)

## [Postgres 19：发生了哪些变化以及现在应该测试什么](https://postgresweekly.com/link/191738/rss)

随着 RC1 的发布以及不到一个月后的正式版，Tom Kincaid 详细介绍了哪些特性经过回滚后保留下来，以及在升级前应该尝试什么，包括 `REPACK (CONCURRENTLY)`、`pg_plan_advice`、并行 autovacuum 和逻辑复制序列同步，每个都附带"应该测试什么"的清单。

Tom Kincaid (EDB)

⭐ [Postgres 19 RC1 上周发布](https://postgresweekly.com/link/191739/rss)，RC2 将于11月12日发布，最终版本预计在11月19日发布。

## [100+ 搜索引擎，一个简单的 API](https://postgresweekly.com/link/191737/rss)

无需管理代理或解析器，即可将实时网络搜索添加到您的后端。SerpApi 将 Google 和其他搜索引擎的结构化结果以干净的 JSON 格式提供。

SerpApi **赞助商**

## [`recovery_prefetch` 被认为是有害的并导致服务中断](https://postgresweekly.com/link/191741/rss)

Jeremy 展示了自 Postgres 15 以来默认启用的 `recovery_prefetch`，在写入突发后如何压垮备用存储，导致数小时的延迟。在同步复制的情况下，连接断开后阻止了主库写入长达35分钟，这在[他的重现实验](https://postgresweekly.com/link/191742/rss)中得到了验证。

Jeremy Schneider

🩹 [一个避免在完整页面镜像后进行冗余预取的补丁](https://postgresweekly.com/link/191743/rss)正在审核中，这解决了部分问题。

**简讯：**

- 🇺🇸 [Postgres Conference 2027](https://postgresweekly.com/link/191744/rss) 将于2027年4月21日至23日在加利福尼亚州圣何塞举行。如果您想演讲，其[征稿](https://postgresweekly.com/link/191745/rss)开放至1月31日。

- [谁拥有一个被放弃的扩展？](https://postgresweekly.com/link/191746/rss) PGXN 的 David Wheeler 在收到接管请求和无人维护扩展的权限提升报告后，向 `pgsql-hackers` 询问应该采取什么政策。

- 🇧🇪 [FOSDEM PGDay 2027](https://postgresweekly.com/link/191747/rss) 扩展到两天，1月28日至29日在布鲁塞尔举行。[征稿](https://postgresweekly.com/link/191748/rss)开放至12月1日。

- 🇹🇭 [FOSSASIA PGDay 2027](https://postgresweekly.com/link/191749/rss) 将于2027年3月9日在曼谷举行。他们的[征稿](https://postgresweekly.com/link/191750/rss)开放至11月30日。

- [Neon Realtime](https://postgresweekly.com/link/191751/rss) 现在处于公开测试阶段。您可以订阅任何确定性 SQL 查询，结果将随着数据的变化而保持实时更新。

- [84% 接受调查的 Ruby on Rails 开发者在生产环境中运行 Postgres](https://postgresweekly.com/link/191752/rss)，这是2026年 Rails 社区调查的结果。

## [如何让 `hstore` 在审计日志中击败 `jsonb`](https://postgresweekly.com/link/191753/rss)

depesz 看到[一篇文章](https://postgresweekly.com/link/191754/rss)声称从审计触发器中仅记录已更改的列可以将日志缩小5倍，但会减慢更新速度。但他自己的测试使用 `hstore` 而不是 `jsonb`，使差异日志成为最快的变体。

Hubert 'depesz' Lubaczewski

## [为什么 Postgres 的 `numeric` 类型如此慢？](https://postgresweekly.com/link/191756/rss)

深入探讨 `numeric` 的内部机制，解释为什么它与 double precision 或 DuckDB 的整数支持的 `DECIMAL` 相比如此缓慢，以及为什么*"只使用 int128"*无法解决它。

Andrei Lepikhov (pgEdge)

## [Citus 在一半 *Neki* 数据节点上达到 1000 万 QPS](https://postgresweekly.com/link/191757/rss)

在 PlanetScale 的 [1.18 亿 QPS Neki 帖子](https://postgresweekly.com/link/191777/rss)发布一个月后，Álvaro 在带有 StackGres 新查询路由器的 Citus 上运行了相同形状的工作负载，在24个工作节点上达到了1000万 QPS，而不是 Neki 的50个分片。

Álvaro Hernández (StackGres)

🎧 [Postgres FM 在同一天邀请了 Álvaro](https://postgresweekly.com/link/191759/rss)，进行了一个小时关于 Citus、StackGres 和基准测试背后思考的访谈。

📄 [为什么 Materialize 放弃 `SERIALIZABLE` 以获得 3 倍写入吞吐量](https://postgresweekly.com/link/191760/rss) — 数十万个谓词锁拖垮了他们基于 Postgres 的元数据存储，因此他们在 `READ COMMITTED` 上重建了它，并在 Lean 中*证明*了其正确性。*Petros Angelatos*

📄 [从警报到在线重组：Postgres 表膨胀的实战手册](https://postgresweekly.com/link/191762/rss) — 使用 `pg_cron` 和 `pgstattuple` 构建膨胀"监视器"，然后使用 `pg_repack` 在不脱机的情况下将13GB 的表缩减到3.4GB。*Haider Z (Microsoft)*

📄 [减少 Amazon RDS 快照恢复后的存储初始化影响](https://postgresweekly.com/link/191761/rss) — 为什么刚恢复的 RDS Postgres 上的查询一开始可能会慢10-15倍，以及如何预热它。*Modappady, Pattabiraman and Thakur (AWS)*

📄 [以 `text` 存储的 UUID：在 Postgres 18 中的成本](https://postgresweekly.com/link/191763/rss) *Hollis Varden*

📰 **分类广告：**

今天：让编码代理分叉、破坏和修复一个真实的 Postgres 数据库。[免费现场研讨会](https://postgresweekly.com/link/191764/rss)，包含录制。

**发布和代码：**

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/sv56ilc9yxghvv6sdnem.jpg)

## [DocumentDB 1.0：Postgres 上兼容 MongoDB 的文档数据库](https://postgresweekly.com/link/191765/rss)

去年由 Microsoft 首次开源，但现在是 Linux 基金会项目，DocumentDB 是一组扩展（加上网关），可以使用 MongoDB wire protocol 并原生存储 BSON。这个首个稳定版本附带了 Postgres 17 和 18 的软件包。

DocumentDB

## [PGX：在一个进程中运行数千个一次性数据库](https://postgresweekly.com/link/191766/rss)

来自 [pgbot](https://postgresweekly.com/link/191767/rss) 背后的团队，基于 Postgres 的 Rust 重新实现构建，PGX 在一个进程中托管大量隔离的数据库，每个数据库在几毫秒内从模板克隆，用于代理沙箱和每个 PR 的测试。测试版，AGPL 许可，`fsync` 关闭，所以仅用于开发。（[GitHub 仓库](https://postgresweekly.com/link/191768/rss)。）

PGRun

## [pgBackRest 2.60：恢复现在会在无效页面校验和时停止](https://postgresweekly.com/link/191769/rss)

这个流行的备份和恢复工具现在会在任何恢复的文件有无效页面校验和时停止恢复并报错。在下次恢复之前值得了解！（`checksum-page-error=n` 可以将其更改为仅警告。）

pgBackRest Community

- [pg_hint_plan 1.9.0](https://postgresweekly.com/link/191770/rss) — 长期存在的查询提示扩展，现在（仅）为 Postgres 19 构建，使用其新的路径生成策略。

- [PostgREST 16.5](https://postgresweekly.com/link/191771/rss) — 流行的 Postgres REST API 服务器层。为最近的 Postgres CVE 添加了客户端缓解措施。

- ⚠️ [pgmq 1.13.1](https://postgresweekly.com/link/191772/rss) — Postgres 原生消息队列。修复了两个权限问题，如果您使用它请升级。

- [pg_ivm 1.17](https://postgresweekly.com/link/191774/rss) — 增量维护的物化视图，如果使用 `pg_ivm_dump_metadata --pg-upgrade`，现在可以在 `pg_upgrade` 中幸存。

- 🌐 [PostGIS 3.7.0 RC3](https://postgresweekly.com/link/191775/rss) — 地理空间数据扩展针对 Postgres 19 RC1 — 我预计最终的 3.7 版本会在 Postgres 19 本身的同时发布。