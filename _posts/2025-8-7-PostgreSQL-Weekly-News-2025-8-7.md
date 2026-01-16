---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-8-7
---
### PostgreSQL每周新闻#611 - 2025年8月78日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/611)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/rjikvpj3fqkuniwzqb6n.jpg)
## [Postgres 复制槽：确认刷新 LSN 与重启 LSN](https://postgresweekly.com/link/172818/web)
复制槽阻止 Postgres 丢弃 WAL（预写日志）段，直到所有消费者都读取完毕。消费者通过日志序列号 (LSN) 跟踪进度，但 Postgres 会公开多个 LSN，其含义略有不同。Gunnar Morling 解释了它们的区别，以及为什么它们在生产环境中都很重要。

`Gunnar Morling`

## [快速发现并修复 PostgreSQL schema漂移](https://postgresweekly.com/link/172819/web)
厌倦了schema意外？pgCompare 可以精确显示不同环境之间的更改，直至 SQL 行。快速生成脚本以同步更改并快速修复问题。非商业用途免费。快来体验吧！

`Redgate   `

### **本周摘要**

* 🇺🇸 [PGConf NYC](https://postgresweekly.com/link/172820/web) 将于 9 月 29 日至 10 月 1 日举行。[日程安排](https://postgresweekly.com/link/172821/web)已经公布，精彩演讲精彩纷呈。

* 🇬🇧 [PGDay UK](https://postgresweekly.com/link/172822/web) 回归，将于 9 月 9 日在伦敦举行。以下是目前的[日程安排](https://postgresweekly.com/link/172823/web)。

* PGDay Lowlands 的组织者希望鼓励您测试 [PostgreSQL 18 Beta 2]https://postgresweekly.com/link/172824/web)，请将您的名字列入“测试者墙”，并参加抽奖，赢取 PGDay Lowlands 门票。

* PlanetScale 解释了▶️他们如何将 MySQL 平台的热门功能 [PlanetScale Insights](https://postgresweekly.com/link/172825/web) 引入到他们的新 Postgres 产品中。

* 🇫🇮 2026 年[北欧 PGDay](https://postgresweekly.com/link/172826/web) 将于明年 3 月 24 日在芬兰赫尔辛基举行。CFP 将于 9 月开放，但如果您有兴趣加入项目委员会，他们正在寻找[志愿者](https://postgresweekly.com/link/172827/web)。

* [富士通的 Shlok Kumar Kyal](https://postgresweekly.com/link/172828/web) 是本周 PostgreSQL 人物的采访对象。


## [不，您不一定需要扩展来压缩 Postgres 表](https://postgresweekly.com/link/172829/web)
假设您无法在服务器上使用 pg_squeeze 或 pg_repack，那么在没有完全清理数据的情况下，该如何减少大表的膨胀呢？Kaarel 提供了一种方法。


`Kaarel Moppel `

## [高可用性和 Postgres 完全同步复制](https://postgresweekly.com/link/172832/web)
Multigres 是一个旨在构建 Vitess for Postgres 适配版的项目，用于实现多租户、高可用性扩展。在这篇文章中，Multigres 和 Vitess 的创建者解释了所涉及的问题以及他们计划如何解决这些问题。


`Sugu Sougoumarane `


📄 [使用 stack trace 调试 Postgres 错误](https://postgresweekly.com/link/172834/web)——一种巧妙的技巧。Phil Eaton

📄 [当 Postgres 性能下降时，首先要检查的地方是](https://postgresweekly.com/link/172835/web) Umair Shahid (Stormatics)

📄 [《精通 PostgreSQL 17》快速书评](https://postgresweekly.com/link/172836/web) Dave Stokes

📄 [你知道 SQL 中的横向连接 (LATERAL JOIN)](https://postgresweekly.com/link/172837/web) 吗？Mohamed Mayallo


### **发布**

## [pg_squeeze 1.9：自动表膨胀清理的扩展](https://postgresweekly.com/link/172830/web)
虽然不能替代清理，但此扩展更进一步，可以获得更多空间改进，现在支持 Postgres 18。

`CYBERTEC`

## [plpgsql_check 2.8.2：PL/pgSQL 代码检查器](https://postgresweekly.com/link/172838/web)
当您想要查找隐藏在 PL/pgSQL 函数中的任何错误时使用的专用工具。

`Pavel Stehule`


[Pigsty 3.6](https://postgresweekly.com/link/172839/web) – 一款流行的 Postgres“元发行版”，现已支持 Postgres 18。

[pgrx 0.16](https://postgresweekly.com/link/172840/web) – 一种使用 Rust 构建 Postgres 扩展的方法，现已支持 Postgres 18 beta 2。

[PeerDB 0.31](https://postgresweekly.com/link/172841/web) – 将数据从 Postgres 流式传输到数据仓库、队列和存储引擎。

[tbls 1.87](https://postgresweekly.com/link/172842/web) – 自动以 Markdown 格式（例如在 CI 中）记录数据库。

[ChartDB 1.14](https://postgresweekly.com/link/172843/web) – 基于图表的开源数据库编辑器。

[Martin 0.18](https://postgresweekly.com/link/172844/web) – 基于 Rust 的快速 PostGIS 地图瓦片服务器。