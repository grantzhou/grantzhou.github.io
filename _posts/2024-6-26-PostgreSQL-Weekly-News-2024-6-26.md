---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-6-26
---
### PostgreSQL每周新闻#556 - 2024年6月26日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/560)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/ihrht59lk1g6kbuuqgrd.jpg)
## [使 Postgres 可见性地图可见](https://postgresweekly.com/link/156790/web)
如果您从未深入研究过 Postgres 性能或事务，那么您可能从未遇到过可见性地图。这是一种机制，Postgres 通过该机制跟踪表中哪些页面仅包含所有事务都可见的元组。这会对性能产生一些影响。

`LAURENZ ALBE `

## [Postgres 贡献者的指导计划](https://postgresweekly.com/link/156792/web)
资深 Postgres 贡献者 Robert Haas 正在启动一个指导计划，希望为 Postgres 贡献代码的人可以得到当前提交者的指导。目前只对 9 人开放，但对于任何有兴趣的人来说，这都是一个绝佳的机会。


`ROBERT HAAS `
## [Render 是您最快的生产途径](https://postgresweekly.com/link/156789/web)
无论您的应用是什么，您都可以轻松构建、快速部署、更新和自信地扩展您的应用，从第一个用户到第十亿个用户。开始免费使用 Render 进行构建 — 面向开发人员的现代云。


`RENDER `


### 本周摘要：


* EDB 的 Tomas Vondra 对最近的[布拉格 PostgreSQL 开发者日活动](https://postgresweekly.com/link/156793/web)进行了精彩回顾。

* 🎧 [Postgres FM ](https://postgresweekly.com/link/156794/web)播客通过采访三位大幅扩展了 Postgres 的工程师来庆祝其[第 100 期节目](https://postgresweekly.com/link/156795/web)。

* [Adyen 的 Derk van Veen](https://postgresweekly.com/link/156796/web) 是本周 PostgreSQL 人物的受访者。


## [自定义 ENUM 类型列和 ORDER BY](https://postgresweekly.com/link/156797/web)
[枚举类型](https://postgresweekly.com/link/156798/web)可以轻松地对某些列中的内容实施约束，但在排序时可能需要小心。


`CHRISTOPH SCHIESSL `
## [对一些 Postgres‘共享内存不足’错误的事后分析](https://postgresweekly.com/link/156799/web)
太多的锁会把事情搞糟。


`ANDREA BAIDA `


### ▶️ POSETTE 演讲值得一看

微软的 POSETTE 活动于本月初完全在线举行，所有演讲都已在 YouTube 上发布。我一直在观看或浏览尽可能多的演讲，如果您有时间，其中一些演讲肯定会脱颖而出……

▶ [调整参数与调整查询](https://postgresweekly.com/link/156800/web) — 很高兴看到 Postgres 领域的一位知名人士站出来揭穿调整配置参数可以解决所有 Postgres 性能问题的想法。她还通过一个示例介绍了调整查询带来的巨大好处。

`HENRIETTA DOMBROVSKAYA`

▶ [您从未见过的 Postgres 性能技巧 v2.0](https://postgresweekly.com/link/156801/web) — Hans-Jürgen 当然知道如何给演讲起标题来吸引注意力！幸运的是，他也提供了很好的内容。这是一个真正的“大杂烩”，但如果你有 25 分钟，你会学到一些东西。

`HANS-JÜRGEN SCHÖNIG`

▶ [使用 Django、Postgres 和 pgvector 进行语义搜索](https://postgresweekly.com/link/156802/web) — 虽然这确实涵盖了使用嵌入来创建语义搜索系统，但重点完全放在 Django 上。

`PAOLO MELCHIORRE`

当然，这并不是所有值得一看的内容。您可以在[此处](https://postgresweekly.com/link/156803/web)找到完整的播放列表，我们也链接到了之前的一些其他演讲。


## [Postgres 中生成列的介绍](https://postgresweekly.com/link/156804/web)
在 Postgres 中，生成列是在插入或更新行时根据用户定义表达式的结果自动填充的列。


`CRAIG HAFER `
## [通过 DuckDB 更快地从 Postgres 加载到 Postgres](https://postgresweekly.com/link/156805/web)
如何使用 ConnectorX 和 DuckDB 快速将数据从 Postgres 导出和导入到 Postgres。


`SIMON SPÄTI `


### 💫 经典博客：
我时不时会回顾的一些旧帖子：

📄 [模糊文本搜索：从不那么模糊到最模糊](https://postgresweekly.com/link/156806/web) BRENDAN SCULLION

📄 [向量是 Postgres 中的新 JSON](https://postgresweekly.com/link/156807/web) JONATHAN KATZ

📄 [SQL 配方：与邻居进行比较](https://postgresweekly.com/link/156808/web) ANTON ZHIYANOV

📄 [Postgres 索引：BRIN 何时获胜？](https://postgresweekly.com/link/156809/web) PAUL RAMSEY



### 📰 机密：


正在考虑你的职业生涯吗？我们[揭示了 2024 年及以后数据库格局的重大变化](https://postgresweekly.com/link/156810/web) - 以及你可以做些什么来应对这些变化。

🚀 尝试 [Rocketadmin](https://postgresweekly.com/link/156811/web) 无缝生成的数据库管理面板，并受益于其智能记录编辑功能。[无需编码](https://postgresweekly.com/link/156811/web)！

### 🛠 代码和工具

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/fxzqxzecvcxahs3lclpm.jpg)


## [pgModeler：Postgres 数据库建模工具](https://postgresweekly.com/link/156514/web)
一种以更直观的方式创建和编辑数据库模型的简便方法。它被打包为付费产品，但也是开源的（GPLv3 – [存储库](https://postgresweekly.com/link/156813/web)，因此您可以自行构建。


`RAPHAEL ARAÚJO E SILVA `
## [Dalibo Postgres 执行计划可视化工具](https://postgresweekly.com/link/156514/web)
为其提供 EXPLAIN ANALYZE 的输出，并更好地了解 Postgres 计划对您的查询执行的操作。如果您想在本地或应用程序中使用它，它也是[开源](https://postgresweekly.com/link/156815/web)的。


`DALIBO `
## [pg_squeeze：自动清理表膨胀的扩展](https://postgresweekly.com/link/156816/web)
虽然它不能替代清理，但它是一个方便的扩展，可以更进一步，并在现场获得更多空间改进。


`CYBERTEC `

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/bou1pr65zgrgk3bq5ve8.jpg)

## [pspg：专为 Postgres 表设计的 Unix 分页器](https://postgresweekly.com/link/156817/web)
如果您使用 psql，您可能使用 less 来当分页器，但它不直接支持表格数据。这个支持。它也支持 MySQL、CSV 和 TSV。


`PAVEL STEHULE `
## [pg_easy_replicate：以最少的停机时间切换数据库](https://postgresweekly.com/link/156818/web)
一个由 Ruby 驱动的编排器，可简化在两个 Postgres 数据库之间设置逻辑复制的任务，然后让您以最少的停机时间切换到较新的数据库。


`SHAYON MUKHERJEE `

