---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2022-6-15
---
### PostgreSQL每周新闻#459 - 2022年6月15日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/459)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/zzhrk1f0an8shljgb29z.jpg)
## [模糊文本搜索：从不太模糊到最模糊](https://postgresweekly.com/link/124789/web)
如果你有其他人提供的自由格式文本数据，它不会是完美的（错别字、俚语、奇怪的格式等），所以支持一点“模糊性” 当查询数据可以走很长一段路。 这是一个很好的浏览 Postgres 为您提供的一些选项，从最不“模糊”到完整的 Fozzie Bear。


`Brendan Scullion `
## [⚠️ 即将更新 Postgres 14 以避免索引的无声损坏](https://postgresweekly.com/link/124790/web)
⚠️在 Postgres 邮件列表中，已于 6 月 16 日（明天）预先宣布了一个重要的“非周期”版本，该版本将修复可能导致索引无声损坏的 Postgres 14 问题 如果您同时使用 CREATE INDEX 或 REINDEX。 邮件列表上也有关于这个问题的完整讨论。


`Gilles Darold `
## [2022 年 PostgreSQL 现状调查](https://postgresweekly.com/link/124793/web)
2022 年 PostgreSQL 现状调查现已开放！ 分享您对 PostgreSQL 数据库、您最喜欢的扩展、首选框架、社区体验等的看法。


`Timescale `
## [从 pg_cron 将计划作业迁移到 pg_timetable](https://postgresweekly.com/link/124794/web)
pg_timetable 是 Postgres 的高级作业调度扩展，与更新频率较低（但仍然非常有用）的 pg_cron 相比，它提供了更多开箱即用的功能。 如果你想迁移，这里是如何。


`Pavlo Golub `
## [在 Postgres、Citus 和 Azure 上构建 IoT 应用程序](https://postgresweekly.com/link/124797/web)
如果您正在创建一个应用程序来处理来自设备的不间断时间序列数据，那么扩展很快就会成为一个问题，并且依赖于托管服务，例如 Azure 提供的服务， 可以帮助轻松扩展。


`Suryanarayana and Srirampur `
## [使用 Postgres schema](https://postgresweekly.com/link/124798/web)
我总是很难简洁地描述 Postgres schema/命名空间，但是“以最小的开销，它们可以在数据库中实现表的分段和隔离”是一个不错的尝试。 Aaron 向我们介绍了这里的一些好处。


`Aaron O. Ellis `
## [升级 Postgres 版本时要研究的内容](https://postgresweekly.com/link/124799/web)
关于如何研究在切换 Postgres 版本时可能影响您的更改的一些快速提示。 为什么要升级 PostgreSQL？ 也是一个方便的资源。


`Bruce Momjian `
## [不区分大小写的模式匹配](https://postgresweekly.com/link/124801/web)
您可能会感觉到与模糊文本搜索项（如上所示）的一些呼应，但 Laurenz 涵盖的内容略有不同，特别是在处理排序规则中区分大小写的复杂性以及为什么 German 的 ß 使事情变得有趣方面。


`Laurenz Albe `
## [从 Oracle 迁移到 Postgres 时处理空字符串](https://postgresweekly.com/link/124802/web)
我从来没有将数据库从 Oracle 迁移到 Postgres，但 AWS 非常希望您这样做，因此正试图教育我们了解可能出现的问题。


`Pattanayak, Mahto, and Paladi (AWS) `
## [使用 NUMERIC 处理尾随零](https://postgresweekly.com/link/124803/web)
在进行 Oracle 到 Postgres 迁移时可能会遇到的另一个怪问题。

`Jagadeesh Panuganti `
## [6 月 16 日的网络研讨会：如何推理索引 Postgres 数据库](https://postgresweekly.com/link/124804/web)


`pganalyze `
## [pg_graphql：为 Postgres 带来 GraphQL 支持](https://postgresweekly.com/link/124807/web)
几个月前对我们来说是一个最重要的功能，但不是一个可以轻忽的项目。


`Supabase `
## [pguint：无符号整数类型扩展](https://postgresweekly.com/link/124808/web)
将有符号 8 位整数和无符号 8、16、32 和 64 位整数类型引入 Postgres 9.1+。


`Peter Eisentraut `

