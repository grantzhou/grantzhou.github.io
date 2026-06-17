---
layout: post
title: PostgreSQL 每周新闻 2026-6-17
---
### PostgreSQL每周新闻#653 - 2026年6月17日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/653)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/rl7yc3sauxvwjkycdstt.jpg)

## [将 Postgres 扩展至 226k TPS：圣诞节回顾](https://postgresweekly.com/link/186644/rss)

一篇详细的事后分析和战术演练文章，讲述一家数字相框公司如何从 2024 年假期期间 Postgres 部署崩溃，到 2025 年顺利处理流量的历程。

`Andrew Atkinson`


## [了解 CERN 如何在减少 95% 存储的同时实现 40% 更快的查询](https://postgresweekly.com/link/186643/rss)

CERN 的 800 多个 SCADA 系统每天生成数百 GB 的时间序列数据。了解他们的工程师如何使用 TimescaleDB 实现 95% 的存储减少和 40% 的查询加速 — 在 Postgres 内部。6 月 25 日，美国东部时间上午 9 点。

`Tiger Data (creators of TimescaleDB)` **赞助商**


## [Postgres 中唯一可扩展的删除是 `DROP TABLE`](https://postgresweekly.com/link/186645/rss)

提醒大家，大型 `DELETE` 操作的成本比你想象的要高，以及在某些情况下如何通过重构为 `DROP` 或 `TRUNCATE` 来提供帮助。

`Tom Pang (PlanetScale)`


## 本周摘要：

- Claire Giordano 呈现了一份精彩的综述，介绍了过去一年 [Microsoft 在 Postgres 方面的所有新进展](https://postgresweekly.com/link/186646/rss)，从其托管服务到团队成员对 Postgres 19 的贡献。

- 📺 Microsoft 的 [POSETTE 2026](https://postgresweekly.com/link/186647/rss) 虚拟 Postgres 会议将在*本周*举行，如果你想观看直播的话。

- [PgDog](https://postgresweekly.com/link/186648/rss)（一个开源连接池/分片工具）已经[获得了 550 万美元的融资](https://postgresweekly.com/link/186649/rss)。

- 🇺🇸 [Postgres Summit US](https://postgresweekly.com/link/186650/rss) 将于今年 9 月 30 日至 10 月 2 日在纽约举行。如果你想帮忙，他们正在[寻找志愿者](https://postgresweekly.com/link/186651/rss)。

- 🇬🇧 下周的 [London PostgreSQL Meetup Group](https://postgresweekly.com/link/186652/rss) 会议还剩七个名额。


## [🕒 不列颠哥伦比亚省、时区和 Postgres](https://postgresweekly.com/link/186653/rss)

不列颠哥伦比亚省在今年 3 月[切换到永久夏令时](https://postgresweekly.com/link/186654/rss)，这说明了一个微妙的 `timestamptz` 陷阱：在 `tzdata` 更新*之前*存储的未来本地时间会出现一小时的错误！以下是如何避免陷入困境。

`Christopher Winslett (Crunchy Data)`


## [▶  我是如何开始运营 Postgres 用户组的](https://postgresweekly.com/link/186655/rss)

Jeremy Schneider 与 Claire Giordano 讨论了为什么本地 Postgres 用户组是职业*"快车道"*，以及为什么运营用户组的辛勤工作是值得的。[完整文字记录。](https://postgresweekly.com/link/186656/rss)

`Talking Postgres Podcast` **播客**

💡 Postgres 网站维护了一个[官方本地用户组列表](https://postgresweekly.com/link/186658/rss)，如果你想在你所在的地区找到一个。

📊 [大型服务器上的写入密集型 `sysbench` 测试：Postgres vs MySQL](https://postgresweekly.com/link/186661/rss) – Mark 怀疑最近的 Postgres 版本存在性能回归，正在试图找出问题。*Mark Callaghan*

📄 [1 美元购买一千个 Postgres 分支](https://postgresweekly.com/link/186664/rss) – Xata 如何大幅改进他们的数据库配置和分支时间。*Tudor Golubenco (Xata)*


## 分类广告：

🧩 [pgEdge Control Plane 的新功能](https://postgresweekly.com/link/186667/rss)：在数据库旁部署 MCP、RAG 和 PostgREST… + systemd 预览。

当 AI 编写数据层更改时，代码审查不再是一个清单问题。[AgentField](https://postgresweekly.com/link/186670/rss) 分解了在 AI 原生工程团队中审查变成了什么。[→ 阅读文章](https://postgresweekly.com/link/186670/rss)。


## 🛠 代码和工具

## [pg_durable：Postgres 内部的持久执行](https://postgresweekly.com/link/186673/rss)

Microsoft 已经开源了它在 [Azure HorizonDB](https://postgresweekly.com/link/186674/rss) 中使用的持久工作流引擎。有两个运行在 Postgres 17/18 上的 [Docker 镜像](https://postgresweekly.com/link/186675/rss)可供实验，[完整文档在这里。](https://postgresweekly.com/link/186676/rss)

`Microsoft`


## [pg_ducklake 1.0：Postgres 中的原生 Lakehouse](https://postgresweekly.com/link/186677/rss)

一个扩展，将列式存储、向量化执行和 lakehouse 架构（带目录的数据湖）引入 Postgres，使用 DuckDB 和 [DuckLake](https://postgresweekly.com/link/186678/rss) 构建。

`Relyt`


- [Nandi 3.0](https://postgresweekly.com/link/186679/rss) – 一个用于 *Ruby on Rails* 的迁移工具，防止常规的架构更改在大表上导致数据库宕机。

- [PostgreSQL Anonymizer 3.1](https://postgresweekly.com/link/186680/rss) – 现在具有本地差分隐私（LDP）以提供更强的隐私'噪声'。还包括一个关键的安全更新，指示所有现有用户尽快升级。

- [pgstream 1.1](https://postgresweekly.com/link/186681/rss) – 基于逻辑复制构建的架构更改跟踪和 CDC 工具。

- 🌐 [osm2pgsql 2.3](https://postgresweekly.com/link/186682/rss) – 将 OpenStreetMap 数据导入 Postgres/PostGIS。