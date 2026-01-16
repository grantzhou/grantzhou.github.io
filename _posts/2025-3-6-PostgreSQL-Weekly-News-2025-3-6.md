---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-3-6
---
### PostgreSQL每周新闻#591 - 2025年3月6日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/591)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/bi8megyvt00waotwhffn.jpg)
## [FerretDB 2.0：开源 MongoDB 替代品](https://postgresweekly.com/link/166521/web)
MongoDB！？如果我告诉你这是 Postgres 驱动的 MongoDB，你会怎么想？ FerretDB 是 MongoDB 的一个实现，建立在 Postgres 和 Microsoft 的 DocumentDB 扩展之上，与 MongoDB 不同的是，它是 Apache 2.0 许可的。 GitHub 存储库。

`Farkas and Palazhchenko`

## [Postgres 查询计划可视化工具汇总](https://postgresweekly.com/link/166524/web)
EXPLAIN 命令及其众多选项可让您深入了解 Postgres 计划如何执行查询，并且是找出某些查询速度慢的原因的好方法。不过，原始输出可能难以阅读，但有几种工具可以帮助分解。


`Michael Christofides `
## [POSETTE 的时间表已经出炉：Postgres 的活动！](https://postgresweekly.com/link/166520/web)
POSETTE 2025 是一项免费的虚拟开发者活动，将于 6 月 10 日至 12 日举行。演讲者和时间表刚刚公布！通过 4 个直播与专家一起了解世界上最先进的开源关系数据库。获取详细信息。


`Microsoft `
## [PGConf.dev 2025：5 月 13 日至 16 日在加拿大蒙特利尔举行](https://postgresweekly.com/link/166528/web)
PGCon 的后续活动，PostgreSQL 开发大会是社区最大的年度聚会之一，特别注重将 Postgres 的贡献者聚集在一起。注册已开放，但本周的重大新闻是日程安排现已公布，而且日程安排非常紧凑。


`Slonik Events Canada `

👥 2025 年[扩展生态系统峰会](https://postgresweekly.com/link/166530/web)也将作为 PGConf․dev 的一部分举行，[Postgres 扩展日](https://postgresweekly.com/link/166531/web)将于 5 月 12 日举行（但与主要活动无关）。

### 本周摘要：

* 🇦🇹 [PGDay 奥地利](https://postgresweekly.com/link/166532/web)将于今年 9 月在维也纳回归。如果您想发言，请在 6 月 15 日之前提交演讲。

* 🇩🇪 [PGConf 德国](https://postgresweekly.com/link/166534/web)的时间表现已公布。它将于今年 5 月 8 日至 9 日在柏林举行。

* 🇫🇷 完成我们对欧洲活动的报道后，[PG Day 法国](https://postgresweekly.com/link/166535/web)将于今年 6 月 3 日至 4 日在比利时举行！🇧🇪


## [验证半结构化数据加载的数据类型](https://postgresweekly.com/link/166536/web)
Postgres 16 及更高版本提供 pg_input_is_valid 函数，这是一种快速确定提供的值是否可以解析为指定类型的方法。Elizabeth 展示了如何在几种情况下使用此函数进行验证检查。


`Elizabeth Christensen (Crunchy Data)`
## [Postgres 17 中的新随机函数](https://postgresweekly.com/link/166221/web)
Postgres 17 引入了一些新的随机数生成函数，因此获取 1 到 10 之间的整数现在就像 random(1,10) 一样简单。


`Leo Hsu and Regina Obe`


* 📄 [使用 SQL/PGQ 在 Postgres 中表示图表](https://postgresweekly.com/link/166539/web) – 我们最近看到的几种方法之一。John Nevin (EDB)

* 📄 [使用 VectorChord 在 Postgres 中以 10,000 QPS 进行向量搜索](https://postgresweekly.com/link/166540/web) Junyu Chen (VectorChord)

* 📊 [Postgres 17.4 与大型服务器上的 Sysbench](https://postgresweekly.com/link/166541/web) Mark Callaghan

* 📺 [我用 Postgres Fireship 替换了我的整个技术堆栈](https://postgresweekly.com/link/166542/web)

### 代码和工具：

## [sqldef 1.0：数据库的幂等模式管理](https://postgresweekly.com/link/166543/web)
一个基于 Go 的 CLI 工具和 WASM 库，用于区分 SQL 模式（演示在此处）。支持 MySQL、Postgres、SQLite 和 SQL Server。也是由 Ruby 核心团队成员之一构建的。

`Takashi Kokubun`
## [pytest-postgresql 7.0：用于使用 Python 应用程序测试 Postgres 的 Pytest 插件](https://postgresweekly.com/link/166545/web)
用于在针对 Postgres 数据库进行测试时管理设备的 Pytest Python 测试框架的插件。

`Pytest`


[pgroll 0.10](https://postgresweekly.com/link/166547/web) – 零停机、可逆、模式迁移。

[rsql 0.17](https://postgresweekly.com/link/166548/web) – 关系数据库的命令行 SQL 界面。

[Pgpool-II 4.6.0](https://postgresweekly.com/link/166549/web)