---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2023-8-16
---
### PostgreSQL每周新闻#519 - 2023年8月16日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/519)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/bkyfe6xg3lvivijiskcj.jpg)
## [Postgres 何时变得很酷？](https://postgresweekly.com/link/143922/web)
Postgres 刚刚跨过了开源项目 25 周年的里程碑，但它并不总是“酷孩子”，也并不总是有一个由公司和活动组成的大型生态系统为其欢呼。 Craig 回顾了 Postgres 的一些历史。


`Craig Kerstiens `
## [Postgres 15.4、14.9、13.12、12.16、11.21 和 16 Beta 3 已发布](https://postgresweekly.com/link/143923/web)
当您可以将大量 Postgres 版本压缩到一个中时，为什么还要写几篇博客文章来介绍一系列 Postgres 版本呢？ 😁 所有受支持的 Postgres 版本（包括 v16 的测试版）都已发布版本来修复错误和两个安全漏洞。 需要注意的是，“如果您使用 BRIN 索引来查找 NULL 值，则升级后需要重新索引它们。”


`PostgreSQL Global Development Group `
## [2023 年 PostgreSQL 状况调查现已开放！](https://postgresweekly.com/link/143921/web)
呼叫所有 PostgreSQL 用户！ 立即参加调查，分享您最喜欢的扩展、首选框架、社区体验等。

`Timescale `
## [早期了解 pgvector 的 HNSW 性能](https://postgresweekly.com/link/143924/web)
Postgres 作为矢量数据存储的作用在新兴的机器学习时代只会继续增长，而 HNSW（分层可导航小世界 - 📄 相关论文）提供了一种进行相似性搜索的新方法，该方法具有一些优势。 pgvector 的下一个版本将支持 HNSW，但 Jonathan 已经成功地通过了它的测试 - 简而言之，它的性能非常好。


`Jonathan Katz `
**本周摘要：**
*   🔊 如果您想在接下来的几周我们不在的时候听点什么，可以收听 [Path to Citus](https://postgresweekly.com/link/143926/web) Con 播客或 Postgres.fm？ 更喜欢视频？ ▶️ [Scaling Postgres](https://postgresweekly.com/link/143928/web)频道有很多很棒的东西。


*   [PostgreSQL 16 Beta 3](https://postgresweekly.com/link/143929/web) 现已在 Amazon RDS 数据库预览环境中推出。


*   📄 [Mastering PostgreSQL Administration](https://postgresweekly.com/link/143930/web) 是 Bruce Momjian 制作的一个方便的 PDF 片子。


*   Graphite 是 Amazon Aurora Postgres 的重度用户，他撰写了有关切换到 [Aurora I/O Optimized](https://postgresweekly.com/link/143931/web) 为他们带来巨大节省的文章。


## [使用角色和权限保护您的数据库](https://postgresweekly.com/link/143932/web)
如果您从未建立过一个系统，其中有多个角色访问单个数据库中的内容，那么这是一个很好的快速入门指南。


`Romario López `
## [充分利用现有系统](https://postgresweekly.com/link/143933/web)
当您的数据库服务已经位于尽可能最大的实例上时，您是否需要重新考虑一切？ 丹说，没那么快，通常有一种方法可以榨取更多的资源。


`Dan Slimmon `
## [SQL 样式指南](https://postgresweekly.com/link/143935/web)
方便的 SQL 样式指南，可确保查询清晰且可维护。


`Simon Holywell `
## [Postgres 谜题的更多乐趣：带动画的递归函数](https://postgresweekly.com/link/143936/web)
我们一直很喜欢 Greg 的系列，展示了他如何在 Postgres 中解决各种“Advent of Code”谜题，而这个系列在递归函数和渲染基本终端动画方面走得相当远。


`Greg Sabino Mullane `
## [PlanetScale 与 Neon：MySQL 和 Postgres 之间的延续传奇](https://postgresweekly.com/link/143937/web)
比较 MySQL 和 Postgres 是一回事，但您也可以比较以无服务器方式提供这两种服务的最新平台。


`Bytebase `
`说到 Neon，他们最近在 [B 轮融资中筹集了 4600 万美元](https://postgresweekly.com/link/143939/web)。`

[▶ 您可能已经在使用 Postgres：您需要了解 Chelsea Dole 和 Floor Drees 的知识
通向 CITUS CON 播客之路](https://postgresweekly.com/link/143940/web)

`PATH TO CITUS CON PODCAST`

[如何使用 psql 从 SQL 文件执行查询](https://postgresweekly.com/link/143941/web)

`SALMAN AHMED`

[在 WASM 中使用 tree-sitter 解析 pgSQL](https://postgresweekly.com/link/143942/web)

`SPLITGRAPH`


## [supavisor 0.9：supabase的邮政连接池](https://postgresweekly.com/link/143943/web)
它是由长生不老药建造的，是专门为多租赁设计的。这篇文章包括一组有趣的基准测试，Supabase最多可以连接100万个基准。V0.9添加上游和下游SSL支持，每个租户指标终点以及限制每个租户连接的能力。Github仓库。

**代码和工具**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/ujoixxrsbe2aoqhha9rm.jpg)

## [Supavisor 0.9：来自 Supabase 的 Postgres 连接池](https://postgresweekly.com/link/143943/web)
它是用 Elixir 构建的，专为多租户而设计。 这篇文章包含一组有趣的基准，Supabase 将其连接数提高到了 100 万。 v0.9 添加了上游和下游 SSL 支持、每个租户指标端点以及限制每个租户的连接的能力。 GitHub repo.Supavisor 0.9：来自 Supabase 的 Postgres 连接池 - 它是用 Elixir 构建的，专为多租户而设计。 这篇文章包含一组有趣的基准，Supabase 将其连接数提高到了 100 万。 v0.9 添加了上游和下游 SSL 支持、每个租户指标端点以及限制每个租户的连接的能力。


`Supabase `
## [pgsql-http 1.6：Postgres 的 HTTP 客户端](https://postgresweekly.com/link/143946/web)
例如，您希望能够从触发器调用 Web 服务吗？ 这是你的机会。


`Paul Ramsey `

## [在任何云上运行相同的开源 Postgres。 仅需 300 美元积分即可免费开始](https://postgresweekly.com/link/143947/web)

`Adab Biranimal`

[PostGIS 3.4.0](https://postgresweekly.com/link/144069/web)

[PL/R 8.4.6  - 用R语言编写Postgres过程](https://postgresweekly.com/link/143948/web)


[PLPGSQL_CHECK 2.4  -  PL/PGSQL的Linter工具]


[Slonik 34.1](https://postgresweekly.com/link/143950/web) 
↳ Node.js Postgres 客户端，具有运行时和构建时类型安全性。

[Postgresml 2.7.4](https://postgresweekly.com/link/143952/web)


![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/ioiweeadbnvenrczuqku.jpg)

## [用 SQL 渲染 Mandelbrot 集](https://postgresweekly.com/link/143953/web)
我们上次链接这个是几年前的事了，但重新审视一下作为开始我们暑假的轻松方式似乎是合适的。 这是一个值得您理解的有趣查询，甚至符合 SQL:2008。 SQLite 在其文档中也有自己的版本。


`PostgreSQL Wiki `