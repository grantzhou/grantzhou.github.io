---
layout: post
title: PostgreSQL 每周新闻 2026-8-26
categories: [PostgreSQL]
tags: [PGWeekly]
---
### PostgreSQL每周新闻#662 - 2026年8月26日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/662)

🏖️ 在迪士尼玩了一周后，我疲惫但又比以往任何时候都更准备好潜回到 Postgres 的（远没那么潮湿的）水域中！

*主编：Peter Cooper*

---

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/dgkdziqztsotu3zsbej3.jpg)

## [八年 Postgres 建议，针对 Postgres 19 重新检验](https://www.crunchydata.com/blog/postgres-19-how-our-advice-has-changed-since-we-wrote-it)
回顾多年来关于 `COPY`、TOAST、BRIN、覆盖索引和分区的建议，检查随时间推移哪些行为和实践发生了变化。按主题的表格显示了每个版本中哪些方面发生了变化，因此无论您使用哪个版本，这都是一个有用的回顾。

`Christopher Winslett (Crunchy Data)`

## [即将推出：ParadeDB Cloud](https://paradedb.com/cloud)
我们正在构建一个完全托管的 ParadeDB：一个 Postgres 用于您的应用数据、全文搜索、向量检索和聚合。[我们的早期访问候补名单现已开放](https://paradedb.com/cloud)。

`ParadeDB` **赞助商**

## [Postgres 18.6、17.11、16.15、15.19 和 14.24 发布](https://www.postgresql.org/about/news/postgresql-186-1711-1615-1519-1424-and-19-beta-3-released-3365/)
在我们上期之后仅一天就发布了一大波更新，包括 28 个 CVE 的修复。对每个人来说这都不是简单的更新。Postgres 18 上的 GIN 用户需要检查 `reltuples` 值，而 `btree_gist` 和 `ltree` 的用户可能需要重建索引（完整详情请参阅*"Updating"*部分）。

`PostgreSQL Global Development Group`

💡 作为上述发布浪潮的一部分，[Postgres 19 Beta 3](https://www.postgresql.org/about/news/postgresql-186-1711-1615-1519-1424-and-19-beta-3-released-3365/) 也发布了，包含大量修复，值得注意的是，**对 [`GROUP BY ALL`](https://www.depesz.com/2025/10/02/waiting-for-postgresql-19-add-group-by-all/) 的支持已被移除**，其实现推迟到 Postgres 20 - [更多详情请见此处](https://git.postgresql.org/gitweb/?p=postgresql.git;a=commitdiff;h=a32733d8f10f0e35f7e4ee772ddbef552296577f)。

**本周摘要：**

- Pavel Stehule 创建了 [lua-psql](https://github.com/okbob/lua-psql)，一组补丁用于在 `psql` 中添加对 Lua 的实验性支持。

- 是谁帮助 Postgres 占领世界？[Michael Stonebraker 令人惊讶的答案](https://www.theregister.com/databases/2026/08/19/postgres-pioneer-credits-oracle-with-helping-his-database-take-over-the-world/5289087)是……Oracle！

- 🇺🇸 [Postgres Summit US 2026](https://2026.postgressummit.us/) 的门票仍然可用，将于今年 9 月 30 日至 10 月 2 日在纽约举行。[这是日程安排](https://postgresql.us/events/postgressummitus2026/schedule/)。

- 🎧 在最新一期 [Talking Postgres](https://talkingpostgres.com/) 中，Claire Giordano [与 Datasette 创建者 Simon Willison 会面](https://talkingpostgres.com/episodes/how-ai-is-changing-software-development-with-simon-willison)，讨论 AI 如何改变软件开发。

## [读取您的写入：Postgres 19 中的 `WAIT FOR`](https://clickhouse.com/blog/postgresql-19-wait-for-read-your-writes)
一个新的 SQL 命令（[历经十年打造](https://www.postgresql.org/message-id/0240c26c-9f84-30ea-fca9-93ab2df5f305%40postgrespro.ru)），让会话阻塞直到 WAL 达到指定位置。因此，异步副本上的读取可以等待它需要看到的写入，而不是强制每次提交都等待备用服务器。

`Gülçin Yıldırım Jelínek (ClickHouse)`

## [有人在没有 PgBouncer 的情况下运行 Postgres 吗？](https://brandur.org/fragments/postgres-without-pgbouncer)
对 20 家托管提供商的调查显示，几乎所有提供商都默认捆绑 PgBouncer（或类似工具）。那么，Brandur 问道，连接池难道不应该成为 Postgres 的一部分吗？

`Brandur Leach`

💬 不过，在 [Hacker News 讨论](https://news.ycombinator.com/item?id=49277952)中有很多反对意见，有些人认为应用端连接池就足够了。

📄 [期待 Postgres 19：语法大杂烩](https://www.pgedge.com/blog/looking-forward-to-postgres-19-syntax-potpourri) – 快速浏览各种语法优化。*Shaun Thomas*

📄 [为什么 Postgres 会破坏 Kubernetes 的 `container_memory_working_set_bytes` 指标](https://ardentperf.com/2026/08/18/why-postgres-breaks-kubernetes-container_memory_working_set_bytes-metric/) *Jeremy Schneider*

📄 [为您的 Postgres 数据库构建安全的 MCP 服务器](https://blog.pamelafox.org/2026/08/building-safe-mcp-servers-for-your.html) *Pamela Fox (Microsoft)*

📄 [将多语言全文搜索从 SQL Server 迁移到 Postgres](https://aws.amazon.com/blogs/database/migrate-multilingual-full-text-search-from-sql-server-to-postgresql/) *Zhang and Ahmed (AWS)*

### 📰 分类广告：

在 Postgres 上的实时机器数据流上构建实时仪表板。免费研讨会，东部时间 9 月 9 日中午 12 点。[预留您的席位](https://www.tigerdata.com/events/workshop-ignition-meets-tiger-cloud?utm_source=content-syndication&utm_medium=referral&utm_campaign=postgres-weekly-newsletter)。

---

❄️ [归档数据上的 GDPR 删除](https://github.com/pgEdge/coldfront)：一条 SQL，而不是恢复循环。ColdFront 的冷层是可写的。[开源](https://github.com/pgEdge/coldfront)。

---

## 🛠 代码和工具

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/z4ycqvi9jvlvyttgn7ii.jpg)

## [pg_statviz 1.2：Postgres 统计的时间序列分析和可视化](https://github.com/vyruss/pg_statviz)
一个扩展和工具配对，用于对各种统计数据（包括 I/O、锁、WAL、缓冲区使用等）进行时间序列分析和可视化。v1.2 添加了 Postgres 19 支持、阻塞锁分析模块，并支持使用兼容 OpenAI 的端点对结果进行 AI 分析。

`Jimmy Angelakos`

## [pgbot：用于 AI 代理和应用的 Postgres 智能](https://pgbot.dev/)
一个基于 Go 的单二进制只读工具，连接到 Postgres 服务器并打印分级健康报告以及自上次运行以来的更改。只有两周历史，所以还处于早期阶段。[GitHub 仓库](https://github.com/pgrundev/pgbot)。

`Alex Shapalov`

- 🔎 [pg_textsearch 1.4](https://github.com/timescale/pg_textsearch) – Tiger Data 的 BM25 排名文本搜索扩展现在支持中文，并且在使用 `WHERE` 过滤器的 top-K 查询上有巨大的速度提升。

- [pgGraph 1.2](https://github.com/Evokoa/pgGraph/releases/tag/v1.2.0) – 在普通表上进行图索引、搜索和遍历。不再有 254 个标签上限；图现在可以包含多达 100 万种不同类型。

- [pg_stat_ch 0.4](https://github.com/ClickHouse/pg_stat_ch) – 捕获每个查询的执行遥测数据并将其导出到 ClickHouse 进行实时分析。

- 🌐 [PostGIS 3.7.0 RC1](https://postgis.net/2026/08/PostGIS-3.7.0rc1/) – 流行的地理空间数据扩展。修复了错误并针对 Postgres 19 Beta 3。

- [pgBackRest 2.59.1](https://github.com/pgbackrest/pgbackrest/releases/tag/release%2F2.59.1) – 流行的可靠备份和恢复解决方案。它现在也支持 Postgres 19 Beta 3。

- [PGSync 7.3](https://github.com/toluaina/pgsync) – 用于将数据从 Postgres 同步到 Elasticsearch 的中间件。

- [PostgREST 16.2](https://github.com/PostgREST/postgrest/releases/tag/v16.2) – 从现有数据库提供完全 RESTful API。