---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2023-1-25
---
### PostgreSQL每周新闻#490 - 2023年1月25日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/490)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,e_trim,w_350,h_100/e_make_transparent/co_white,e_outline:7/lhwcvgc1asd4fzaahty4.png)
## [来自 PGConf NYC 2022 的 30 多场演讲](https://postgresweekly.com/link/134401/web)
我们在 12 月忘记包括这个，但现在它仍然是一组很好的演讲，无论是与 Bruce Momjian 学习如何保护 Postgres，与 Lætitia Avrot 解决隔离问题，还是学习更多关于 MERGE 命令的信息 与 Simon Riggs（如上图所示）。


`United States PostgreSQL Association `
## [NULL 与一切冲突的唯一约束](https://postgresweekly.com/link/134404/web)
Laurenz 在创建表面上看起来不寻常的唯一性约束时展示了范围数据类型和排除约束。 这里有一些很好的左场思考。


`Laurenz Albe `
## [加入我们的“Postgres 5 分钟”视频系列第 2 季](https://postgresweekly.com/link/134405/web)
在 2022 年超过 50 集之后，我们很高兴开始观看 Postgres 5 分钟第 2 季。 与 pganalyze CEO Lukas Fittl 一起观看关于最值得注意的 Postgres 内容的每周视频。 订阅我们的 YouTube 频道并欣赏明天的剧集！


`pganalyze `
## [令人费解的 Postgres：解决无法重现的性能问题的故事](https://postgresweekly.com/link/134448/web)
深入了解查询计划和准备好的语句。 “我们有一个在生产中特别慢的查询，但它很难重现，因为我们不知道我们的 ORM 在后台使用准备好的语句，而且使用简单的 EXPLAIN ANALYZE 看起来没有任何问题。”


`William Duclot `
## [实施一个简单的 Postgres 补丁的演练](https://postgresweekly.com/link/134406/web)
如果您曾经对直接在 Postgres 上进行黑客攻击所涉及的内容感到好奇，那么这是一个有趣的演练，它调整了 b-tree 搜索的工作方式并将其转化为可用的补丁。 （15分钟。）


`Andrey Borodin `
## [要避免的外键病态](https://postgresweekly.com/link/134411/web)
如果您有一个多对多连接表，其中定义了外键关系，那么在锁定父记录时，大量插入可能会产生意想不到的效果。


`Christophe Pettus `
## [[免费下载] 了解数据库电子书](https://postgresweekly.com/link/134414/web)


`Linode `
## [深入了解 Postgres 15 中的 WAL 压缩和近期改进](https://postgresweekly.com/link/134412/web)
再看一下内置的 WAL 压缩功能，因为 Postgres 15 比以前的版本提供了更多功能。

`Jobin Augustine `
## [更快地调试 Postgres CI 故障](https://postgresweekly.com/link/134415/web)
Postgres 使用 Cirrus CI 作为其持续集成系统。


`Nazir Bilal Yavuz `
## [pg_show_plans：显示所有当前正在运行的语句的查询计划](https://postgresweekly.com/link/134416/web)
让您可以通过 SELECT * FROM pg_show_plans 进行实时访问，或者您可以像 README 中演示的那样针对 pg_stat_activity 加入它。


`CYBERTEC PostgreSQL International GmbH `
## [pg_qualstats：收集有关谓词的统计信息的扩展](https://postgresweekly.com/link/134417/web)
分析在针对您的数据库的查询中最常用的谓词，也许作为创建最有效索引的一种方式。 POWA（PostgreSQL 工作负载分析器）项目的一部分。


`Powa Team `
