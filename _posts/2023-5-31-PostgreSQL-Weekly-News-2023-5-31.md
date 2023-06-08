---
layout: post
title: PostgreSQL 每周新闻 2023-5-31
---
### PostgreSQL每周新闻#508 - 2023年5月31日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/508)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,w_524,h_127/e_make_transparent/co_white,e_outline:9/bmhxbsirg1zkckgnwcor.png)
## [从 Postgres 生成 SVG 图像](https://postgresweekly.com/link/140317/web)
pg-svg 是一组用于在 Postgres 中创建 SVG 图形的函数。 它的主要用例是将 PostGIS 几何图形转换为图形，本文包含详细介绍（完整的史诗查询），但您也可以独立于 PostGIS 使用它。


`Martin Davis (Crunchy Data) `
## [Postgres 16 Beta 1 发布](https://postgresweekly.com/link/140320/web)
我们现在真正走在通往 Postgres 16 最终发布的道路上。 发行说明草案对所有更新进行了梳理，特别是对性能、查询并行性、SQL/JSON、安全性、监控等方面的改进。

`PostgreSQL Global Development Group `
## [物化视图：使用 Postgres 进行预计算](https://postgresweekly.com/link/140347/web)
了解在 Postgres 中使用物化视图进行分析的好处、物化视图和常规视图之间的区别，以及优化它们使用的技巧。


`Hydra `
## [如何在 psql 中使用变量](https://postgresweekly.com/link/140323/web)
你可以在 psql 中使用 \set 或通过在命令行中传递它们来设置变量。 Hubert展示了一些用途。


`Hubert depesz Lubaczewski `
## [来自 Node.js / Deno 的“我，尝试了 8 种不同的 Postgres ORM](https://postgresweekly.com/link/140330/web)
▶现代的、快节奏的、有点不敬的浏览后端 JavaScript 开发人员可以与 Postgres 交互的各种方式（在这种情况下由 Neon 无服务器提供。） （9 分钟。）


`Beyond Fireship `
## [使用 jOOQ 和 Postgres 函数进行缓存同步](https://postgresweekly.com/link/140332/web)

`VLAD MIHALCEA`
##[从 IBM Db2 z/OS 迁移到 RDS 或 Aurora 后验证数据库对象](https://postgresweekly.com/link/140333/web)

`PARTHASARADHI, BALASUBRAMANIAN AND GUPTA (AWS)`
## [HypoPG 1.4.0：Postgres 的假设索引](https://postgresweekly.com/link/140334/web)
您可以使用 HypoPG 创建实际上并不存在但可用于确定查询计划程序是否可以使用所述索引来提高性能的索引。 本周的发布使得支持相反的做法成为可能：假设隐藏现有索引。


`Julien Rouhard `
## [pg_dumpbinary v2.11：以二进制格式转储数据库](https://postgresweekly.com/link/140336/web)
如果可以，请使用 pg_dump，但如果您遇到二进制转储会有所帮助的异常情况——这是给您的。


`Gilles Darold `
## [Diesel 2.1：Rust 的可扩展 ORM 和查询生成器](https://postgresweekly.com/link/140339/web)
在不牺牲性能的情况下摆脱 Rust 中数据库交互的样板。 支持 Postgres、MySQL 和 SQLite。


`Diesel `


## Anton Zhiyanov
Anton是一名与Python和Go合作的后端开发人员，他在应用程序级别使用SQL，并用于探索性数据分析和数据管道。他教授Go和SQL课程，著有《SQL窗口函数解释》（前五章可以免费在线阅读——代码POSTGRES可以在付费版本上获得折扣）。


我们问了他几个关于SQL窗口函数的问题：


“窗口函数”是整个子语言的一个名称（可能会引起误解），在某种程度上，它内置于常规SELECT中。窗口功能有助于执行各种数据分析任务，从排名、分割和计算移动聚合到统计、财务分析、聚类和数据清理。


对于大多数数据分析任务，窗口函数往往会生成更简洁、可读和高效的查询。


幸运的是，所有数据库供应商都实现了非常接近SQL标准的窗口函数，因此没有语法差异（尽管某些DBMS中缺少一些高级功能）。Postgres支持该标准定义的几乎所有与窗口相关的功能（除了窗口化的百分位数）。



