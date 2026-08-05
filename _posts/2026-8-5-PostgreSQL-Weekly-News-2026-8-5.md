---
layout: post
title: PostgreSQL 每周新闻 2026-8-5
---
### PostgreSQL每周新闻#660 - 2026年8月5日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/660)

今年 [PGConf.dev](https://postgresweekly.com/link/188823/rss) 的大量视频现已在 YouTube 上发布，我在本期末尾整理了一些精彩内容！  
__  
*您的编辑，Peter Cooper*

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/tc2t4spvc1sswnkypuh3.jpg)

**[`COUNT(DISTINCT)` 太慢？快速近似计算指南](https://postgresweekly.com/link/188825/rss)** — 深入实践 Postgres 的近似和采样能力，涵盖 `TABLESAMPLE`、`hll` 和 [Apache DataSketches](https://postgresweekly.com/link/188842/rss) 等方法的优缺点和性能特征，基于 1000 万行测试表。

Elizabeth Garrett Christensen (Snowflake)


**[评估 Oracle 迁移到 Postgres 的成本](https://postgresweekly.com/link/188824/rss)** — 考虑从 Oracle 迁移？EDB 的免费计算器可让您按数据库层级和支持级别建模成本。在承诺之前，只需几分钟即可对迁移进行压力测试。

EDB *赞助商*


**[Postgres 11-18 中的 SQL 改进：个人精选](https://postgresweekly.com/link/188826/rss)** — 来自八个版本的 SQL 功能，由长期贡献者按主题分组挑选。仅使用 `tstzmultirange` 和 `range_agg()` 对乐队成员随时间变化建模的部分就值得一看，还有更多精彩内容。

Dimitri Fontaine


**[揭示 Postgres 级联复制中一个 13 年的 Bug](https://postgresweekly.com/link/188827/rss)** — Postgres 9.3 中为流复制添加的保护可能会在回退到归档恢复后锁定级联备用服务器，使其无法从上游进行流复制。此问题已修复，将在下一个次要版本中发布：18.5、17.11 等。

Gabriele Bartolini (EDB)


**[🤖 '将 Claude 变成 Postgres，这样我就能融资 A 轮'](https://postgresweekly.com/link/188828/rss)** — 当你将 LLM 放在 Postgres 线协议后面，让它随心所欲地处理查询时会发生什么？显然就是这个。是的，这有点好玩，但他真的为它实现了实际的存储 API！😅

Jacob Jackson


**[等待 Postgres 19：SQL 属性图查询 (SQL/PGQ)](https://postgresweekly.com/link/188829/rss)** — 如果你想知道 SQL 属性图查询相比普通连接能给你带来什么，你并不孤单！

Hubert depesz Lubaczewski


📄 [Andy Pavlo 加入 ClickHouse 建立 ClickHouse Labs](https://postgresweekly.com/link/188830/rss) – *"我们将研究的一个更大问题是像 ClickHouse 和 PostgreSQL 这样的 DBMS 如何适应新兴的 AI 和代理技术。"* Andy Pavlo (ClickHouse)

📄 [Postgres 和 `pgvector` 的混合搜索模式](https://postgresweekly.com/link/188831/rss) – 迭代索引扫描带来的优势。Christopher Winslett

📄 [Postgres 中的 TDE（透明数据加密）性能](https://postgresweekly.com/link/188832/rss) Zsolt Parragi (Percona)


**📺 PGCONF.DEV 视频精选：**

[PGConf.dev 2026](https://postgresweekly.com/link/188823/rss) 于今年 5 月在温哥华举行，如果您没有参加，[这个 YouTube 播放列表](https://postgresweekly.com/link/188833/rss)中有多达 47 个视频可供欣赏。一些精彩内容：

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/oxow9lzcakncxbgh5sne.jpg)

- ▶️ **[PostgreSQL 30 周年回顾](https://postgresweekly.com/link/188834/rss)（Momjian、Wieck、Chen、Lockhart、Lane 和 Mikheev）** – 一个由 Postgres 先驱组成的小组*（上图）*回顾技术决策、决定性时刻以及多年来的经验教训。由 Melanie Plageman 和 Jonathan Katz 主持。

- ▶️ **[Postgres 缺少什么？](https://postgresweekly.com/link/188837/rss)（Bruce Momjian）** – 审视"缺失"的功能，包括分片、TDE、全局索引和多主复制。如果您更喜欢，还有[幻灯片](https://postgresweekly.com/link/188838/rss)可供参考。

- ▶️ **[构建下一代 Postgres 贡献者](https://postgresweekly.com/link/188835/rss)（Claire Giordano）** – [Talking Postgres](https://postgresweekly.com/link/188836/rss) 主持人反思如何让更多人参与该项目。

- ▶️ **[实时 Postgres 补丁创意评估](https://postgresweekly.com/link/188840/rss)（Freund、Linnakangas、Lane 和 Haas）** – 主要提交者现场评估"惊喜补丁创意"，由 Robert Haas 主持。

- ▶️ **[为什么 Postgres 很糟糕？](https://postgresweekly.com/link/188839/rss)（Christophe Pettus）** – 首先承认 Postgres *并不*糟糕，Christophe 仍然检查了现实世界的痛点、缓解措施和改进机会。

- ▶️ **[分析 Postgres 的陷阱](https://postgresweekly.com/link/188841/rss)（Andres Freund）** – 误导性基准测试、分析陷阱和反直觉性能结果的导览。

或者，[查看播放列表](https://postgresweekly.com/link/188833/rss)以找到吸引您眼球的任何内容 – 远不止上述这些。