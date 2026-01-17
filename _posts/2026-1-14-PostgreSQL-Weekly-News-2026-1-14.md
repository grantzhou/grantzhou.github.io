---
layout: post
title: PostgreSQL 每周新闻 2026-1-14
---
### PostgreSQL每周新闻#631 - 2026年1月14日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/631)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/f4ghzsfvl60ofh3glscl.jpg)

## [Postgres 数组的隐藏成本](https://postgresweekly.com/link/179209/rss)
如果你曾在表中使用数组数据类型，但没有深入思考它与其他方法的权衡，Radim 分享了一些见解，可以帮你避免生产环境中的一些微妙问题。

`Radim Marek`

## [面向 Agentic AI、高可用性等企业级 Postgres](https://postgresweekly.com/link/179207/rss)
pgEdge 是领先的开源企业级 Postgres 公司，它让开发者能够轻松构建和部署可在全球网络中高度扩展和分布式的数据库应用程序。

`pgEdge` **赞助商**

## [序列生成主键中的整数溢出](https://postgresweekly.com/link/179210/rss)
如果你使用 `bigint` 作为序列，即使每秒生成一百万条记录，也可以持续近 30 万年而不会出现问题。但如果使用 `serial`/`integer`，在这样的速率下几小时就会溢出！虽然大多数表不会包含数十亿行，但 Laurenz 提供了一个巧妙的查询来查找这个问题，以及一些解决步骤。

`Laurenz Albe`

**本周摘要：**

* 🇨🇦 [PGConf.dev](https://postgresweekly.com/link/179211/rss) 将于 5 月 19-22 日在加拿大温哥华举行，其[征稿](https://postgresweekly.com/link/179212/rss)将于本周五（1 月 16 日）截止。

* PostgreSQL Code of Conduct Committee（行为准则委员会）去年在寻找新成员，[现在他们宣布了三位新成员](https://postgresweekly.com/link/179213/rss)：Semab Tariq (Stormatics)、Karen Riggs (前 EDB) 和 Gary Evans (PGDownUnder)。

* 🏴 如果你能在 2 月 12 日到达苏格兰，[PostgreSQL Edinburgh 将举办第二次聚会](https://postgresweekly.com/link/179258/rss)。

## [使用 Postgres 作为图数据库：谁一起喝了啤酒？](https://postgresweekly.com/link/179214/rss)
实际探讨 [Apache AGE](https://postgresweekly.com/link/179215/rss) 如何将图数据库概念和查询原生地引入 Postgres 所带来的机会。

`Taras Kloba`

📄 [不要给 Postgres 分配过多内存（即使在繁忙系统上）](https://postgresweekly.com/link/179216/rss) `Tomas Vondra`

📄 [为什么 AI 工作负载正在推动回归 Postgres](https://postgresweekly.com/link/179217/rss) `Rob Pankow (The New Stack)`

📺 [Postgres 查询调优的 5 大技巧](https://postgresweekly.com/link/179218/rss) `Janis Griffin`

**代码和工具：**

## [Barman 3.17.0：Postgres 的备份和恢复管理器](https://postgresweekly.com/link/179219/rss)
用于 Postgres 服务器灾难恢复的管理工具，支持多个服务器的远程备份和恢复。[v3.17.0](https://postgresweekly.com/link/179220/rss) 现在支持在非活动/禁用服务器上进行操作，并弃用了 WAL 文件的自定义压缩。

`EnterpriseDB UK Limited`

## [pg_textsearch 0.4：现代排序文本搜索扩展](https://postgresweekly.com/link/179221/rss)
一个将强大的 [BM25](https://postgresweekly.com/link/179222/rss) 排序引入全文搜索的 Postgres 扩展。[v0.4](https://postgresweekly.com/link/179223/rss) 引入了索引压缩，通过 delta 编码和位打包，索引体积减小约 40%。

`Tiger Data`

* 📊 [pg_statviz 0.9](https://postgresweekly.com/link/179224/rss) – 用于 Postgres 内部统计数据的时间序列分析和可视化的极简扩展和实用工具对。

* [pg_partman 5.4](https://postgresweekly.com/link/179225/rss) – 分区管理扩展，扩展了 Postgres 的内置操作以简化分区管理。

* [QuestDB 9.3](https://postgresweekly.com/link/179226/rss) – Java 驱动的时间序列数据库的重大更新，支持 Postgres 线协议兼容性。

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/mhipj2i4num2esyfwpxx.jpg)

* [sqlit 1.2.6](https://postgresweekly.com/link/179227/rss) _(上图)_ – 用户友好的 Python 驱动的 TUI 工具，用于处理众多 SQL 数据库。

* [BemiDB 1.8](https://postgresweekly.com/link/179228/rss) – 开源的 Snowflake 和 Fivetran 替代品。使用其 Postgres 兼容的分析查询引擎运行复杂查询。

* [River 0.30](https://postgresweekly.com/link/179229/rss) – 快速可靠的基于 Postgres 的 Go 后台作业系统。

* [PGSync 7.0.5](https://postgresweekly.com/link/179230/rss) – Postgres 到 Elasticsearch/OpenSearch 的同步。

* [PostgREST 14.3](https://postgresweekly.com/link/179231/rss) – 为任何 Postgres 数据库提供 REST API。

* [neosql.nvim](https://postgresweekly.com/link/179232/rss) – 用于处理 Postgres 的 Neovim 插件。

🗓 **2026 年即将举行的 Postgres 活动**

* 🇨🇿 [Prague Pg Dev Day 2026（1 月 27-28 日，布拉格）](https://postgresweekly.com/link/179233/rss)
* 🇹🇭 [FOSSASIA PGDay 2026（3 月 10 日，曼谷）](https://postgresweekly.com/link/179234/rss) — 与 FOSSASIA Summit 同时举办的年度活动。
* 🇮🇳 [PGConf India 2026（3 月 11-13 日，班加罗尔）](https://postgresweekly.com/link/179235/rss) — 由印度 PostgreSQL 用户组举办的多日活动。
* 🇫🇷 [pgDay Paris 2026（3 月 26 日）](https://postgresweekly.com/link/179236/rss)
* 🇺🇸 [Postgres Conference 2026（4 月 21-23 日，圣何塞）](https://postgresweekly.com/link/179237/rss) — [征稿](https://postgresweekly.com/link/179238/rss)截止至 1 月 30 日。
* 🇩🇪 [PostgreSQL Conference Germany 2026（4 月 21-22 日，埃森）](https://postgresweekly.com/link/179239/rss)
* 🇧🇪 [PGConf.BE 2026（5 月 5 日，比利时）](https://postgresweekly.com/link/179240/rss)
* 🇨🇦 [PostgreSQL Development Conference 2026 – 即 pgconf.dev（5 月 19 日，温哥华）](https://postgresweekly.com/link/179241/rss) — [征稿](https://postgresweekly.com/link/179212/rss)仅剩几天时间。
* 🇺🇸 [PG DATA 2026（6 月 4-5 日，芝加哥）](https://postgresweekly.com/link/179242/rss) — 全新会议系列的首个活动，重点关注教育、开发者社区建设和学术推广。
* 🇺🇸 [PGDay Boston 2026（6 月 9 日，波士顿）](https://postgresweekly.com/link/179243/rss) – [征稿](https://postgresweekly.com/link/179244/rss)截止至 3 月 20 日。
* 🌐 [POSETTE 2026（6 月 16 日，线上）](https://postgresweekly.com/link/179245/rss) — Microsoft 的免费虚拟活动，由 Microsoft Postgres 团队组织。[征稿](https://postgresweekly.com/link/179246/rss)截止至 2 月 1 日。

*注意：此列表并非详尽无遗，我们将继续提及和推广其他活动。*