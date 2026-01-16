---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-12-18
---
### PostgreSQL每周新闻#582 - 2024年12月18日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/582)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/vmbtuivmasdxjezkw6xn.jpg)
## [我最喜欢的一些东西 - Postgres 查询](https://postgresweekly.com/link/163587/web)
本周实际上没有什么重大的 Postgres 新闻，所以为什么不享受这份节日礼物呢？Shane 使用一些（相当复杂的）SQL 查询来以各种方式跟踪数据库使用情况、查看未使用的索引、生成清理报告等等。

`Shane Borden`

## [在 Postgres 上构建 AI 应用程序？从 pgai 开始](https://postgresweekly.com/link/163586/web)
pgai 是 PostgreSQL 的扩展，它为 PostgreSQL 带来了更多 AI 工作流，例如嵌入创建和模型完成。pgai 为开发人员提供 AI 超能力，使他们更容易构建搜索和检索增强生成 (RAG) 应用程序。


`Timescale  `
## [pg_incremental：Postgres 中的增量数据处理](https://postgresweekly.com/link/163588/web)
Marco 引入了一个新的 Postgres 扩展，提供自动化、增量批处理，以创建可靠的处理管道。GitHub repo。


`Marco Slot `

📄 [通过从头编写 HTTP 服务器来探索 Postgres 的 Arena Allocator](https://postgresweekly.com/link/163590/web) – 这不是胆小者能完成的冒险！Phil Eaton

📄 [Postgres 17 中大型对象转储改进的快速基准](https://postgresweekly.com/link/163591/web) - Michael Banck

📄 [缩小 Postgres 表](https://postgresweekly.com/link/163592/web) - John Nunemaker

### 本周摘要：

* 🗓️ 现在预订航班可能还为时过早，但如果您想参加 [2025 年欧洲 PostgreSQL 大会](https://postgresweekly.com/link/163593/web)，您需要计划于 2025 年 10 月 21 日至 24 日前往拉脱维亚里加。

* 今年，Timescale 的年度 Postgres 社区调查吸引了数百人参与，他们提供了对[调查结果的预览](https://postgresweekly.com/link/163594/web)，以及 📄 一份[完整的（设计相当精良的）PDF 报告](https://postgresweekly.com/link/163595/web)。

* 🇩🇰 [2025 年北欧 PGDay 现已开放报名](https://postgresweekly.com/link/163596/web)。它将于明年 3 月在哥本哈根举行，其 CFP 开放至 12 月 31 日。

* Regina Obe [思考了“巴士因子”问题](https://postgresweekly.com/link/163598/web)（一种衡量项目对“失去”核心贡献者的弹性的略显病态的方法）以及如何准备根据需要添加新的核心团队成员。

* 🎧 [Postgres FM 播客](https://postgresweekly.com/link/163599/web)刚刚采访了 [jOOQ 的 Lukas Eder](https://postgresweekly.com/link/163600/web)。

## 🥇 2024 年的热门发展和项目

2024 年是 Postgres 的又一个丰收年。回顾过去，以下是一些亮点，以及一个令人遗憾的发展：

* 今年开局强劲，DB Engines 将 Postgres [评为“2023 年度 DBMS”](https://postgresweekly.com/link/163601/web)。我想知道我们是否也会在 2024 年获得它？

* [Tembo 聘请了 PGXN 创始人 David Wheeler](https://postgresweekly.com/link/163602/web)来研究如何改善 Postgres 扩展生态系统——他一整年都在努力推进这项工作。这是[最新更新](https://postgresweekly.com/link/163604/web)。

* [Postgres 17 于 9 月发布](https://postgresweekly.com/link/163605/web)，具有彻底改进的内存管理、增量备份支持、更快的 B 树索引扫描、MERGE 改进等。[这是一个很棒的版本。](https://postgresweekly.com/link/163606/web)

* [pgvector](https://postgresweekly.com/link/163607/web) 继续进入所有领域，并发布了一些重要版本（最近是 [v0.8.0](https://postgresweekly.com/link/163608/web)），[性能不断增强](https://postgresweekly.com/link/163609/web)。

* ElectricSQL 推出了 [PGLite](https://postgresweekly.com/link/163610/web)，这是一种在 WebAssembly 环境（包括浏览器）中运行完整 Postgres 数据库的方法。

* Postgres 创始人 Mike Stonebraker 公布了[他的新公司 DBOS](https://postgresweekly.com/link/163611/web)。

* 🗓️ 微软的虚拟 Citus Con 活动更名为 [POSETTE](https://postgresweekly.com/link/163612/web)，并在 2024 年取得了巨大成功。[2025 年的版本](https://postgresweekly.com/link/163613/web)将于 6 月举行，其 [CFP 已开放](https://postgresweekly.com/link/163614/web)。[PGConf.dev](https://postgresweekly.com/link/163615/web) 也进展顺利，您可以在[此处观看演讲](https://postgresweekly.com/link/163616/web)。

* 亚马逊两周前刚刚发布了其[新的 Aurora DSQL 数据库](https://postgresweekly.com/link/163617/web)。

* 当然，这不是什么亮点，但值得认识和记住的是，我们遗憾地[告别了 3 月份去世的 Postgres 维护者 Simon Riggs](https://postgresweekly.com/link/163618/web)。愿他安息。

现在，根据读者参与度列出今年排名前 5 的链接：

* [SQL 查询优化：全面的开发人员指南](https://postgresweekly.com/link/163619/web) — 一篇内容丰富的文章，深入探讨了 SELECT、INSERT 和 DELETE 查询的优化，涵盖了使用索引、分页结果、避免连接以及窗口函数如何提供帮助（或不提供帮助）等领域。并非只针对 Postgres，而是以 Postgres 为中心编写的。

`Francesco Tisiot`

* [优化 Postgres 表布局以实现最高效率](https://postgresweekly.com/link/163620/web) — 长期以来，更广泛的数据结构中的数据对齐一直是低级编程优化的重要因素，但它也会影响您的 Postgres 表。 Renato 研究了表布局如何影响存储效率和查询性能。

`Renato`

* [Postgres 可以替代 Redis 作为缓存吗？](https://postgresweekly.com/link/163621/web)— Redis 是一种流行的高性能内存数据存储服务器，通常用于缓存，但如果我们可以将 Postgres 用于所有事情，那么 Postgres 是否可以代替它完成这项工作？

`Raphael De Lio`

* [pgPedia：Postgres 百科全书](https://postgresweekly.com/link/163623/web) — 一本有趣、格式清晰的 wiki 式参考指南，介绍 Postgres 的功能和设置，与官方文档相得益彰。值得一看。

`Postgrespedia`

* [PostgreSQL 补丁贡献真的很难](https://postgresweekly.com/link/163624/web) — Robert 多年来一直是 Postgres 的前十名提交者，但今年他反思了为 Postgres 做贡献的过程有多么令人生畏，尤其是对于新手来说。

`Robert Haas`

👋 我们现在放假两周，享受圣诞假期。如果你也庆祝圣诞，祝你圣诞快乐。我们将于 2025 年 1 月 9 日星期四回归（是的，我们将在新年更改 Postgres Weekly 的发布日期——让事情变得有趣！）
