---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-11-27
---
### PostgreSQL每周新闻#626 - 2025年11月27日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/626)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/qqnso0ubnlkmlojsw4nf.jpg)
## [Postgres 19 即将迎来超高速聚合](https://postgresweekly.com/link/177659/web)
Postgres 19 距离正式发布还有十个月，但最近的一些提交表明，我们可以期待聚合速度的显著提升，而无需更改查询语句。查询优化器不再采用「先连接后聚合」的模式，而是能够根据实际情况选择先聚合，然后在更合适的时机进行连接。

`Hans-Jürgen Schönig`


## [Tiger Data教会AI编写真正的Postgres程式码](https://postgresweekly.com/link/177658/web)
立即体验－Tiger Data教会AI如何写出道地的Postgres程式码，并将其开源。 pg-aiguide将真正的资料库专业知识带入Claude Code或任何其他支援MCP的工具。。

`Tiger Data`


## **本周摘要**

* 📘 [《Just Use Postgres!》](https://postgresweekly.com/link/177660/web)是 Denis Magda 撰写、Manning 出版的一本书，本月正式发行。本书是对 Postgres 的现代入门介绍，内容超越了典型的关联式资料库管理系统 (RDBMS) 操作，涵盖了 JSON、全文搜寻、pgvector、TimescaleDB、讯息伫列实作等诸多面向。

* 🌐 12 月 9 日，旧金山湾区 Postgres 用户群将[举办一场免费的线上活动](https://postgresweekly.com/link/177661/web)，届时 Christophe Pettus 将介绍 Postgres 18 的新功能。

* 🇧🇪 [FOSDEM PGDay 2026 ](https://postgresweekly.com/link/177662/web)将于 1 月 30 日在比利时布鲁塞尔举行，如果您有意发言，论文征集现已开放，截止日期为 12 月 15 日。

* 旅游报告：Andreas Scherbaum 参加了 [PostgreSQL 日本大会](https://postgresweekly.com/link/177664/web)和 [PostgreSQL 柏林大会](https://postgresweekly.com/link/177665/web)，Henrietta Dombrovskaya 则报道了[草原 PostgreSQL 用户组](https://postgresweekly.com/link/177666/web)的聚会情况。

* [PlanetScale](https://postgresweekly.com/link/177667/web)推出了每月5美元的Postgres托管服务。


## [探索 psql 脚本语言中的斐波那契数列和图灵完备性](https://postgresweekly.com/link/177668/web)
psql 支援多种语法元素，让您可以执行一些在资料库前端可能意想不到的结构化、类似程式设计的任务。 Phil 将进行简报；您可能也能从中了解一些关于 psql 的知识。

`Phil Eaton`


📺 [计算机想要遗失你的资料](https://postgresweekly.com/link/177669/web)－SREcon25 大会上的演讲，以 MySQL 和 Postgres 为例，探讨安全资料储存。 Chris Sinjakli

📄 [PostGIS 效能：资料采样](https://postgresweekly.com/link/177670/web)－Paul 关于 PostGIS 效能系列文章的最新一篇。 Paul Ramsey

📄 [Laravel 的 PostgreSQL 与 MongoDB：选择合适的资料库](https://postgresweekly.com/link/177672/web)－从 Laravel 的角度出发，进行了详尽的比较。 Farhan Hasin Chowdhury

📄 [Postgres 18：跳跃扫描－突破最左索引的限制](https://postgresweekly.com/link/177673/web)。 Ahsan Hadi

📄 [为什么你应该对资料库进行分片](https://postgresweekly.com/link/177674/web)？ Lev Kokotov (PgDog)


## **发布**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/fdv1bgar1zoh5vyodpme.jpg)


## [🤖 pg_ai_query：自然语言查询扩充](https://postgresweekly.com/link/177675/web)
这款有趣的扩充功能能够接收您用自然语言编写的请求，并使用 OpenAI 或 Anthropologie 模型将其即时转换为 SQL。 README 文件中提供了许多范例。

`Sachin Beniwal`

## [IvorySQL 5.0：开源的 Oracle 相容 Postgres](https://postgresweekly.com/link/177677/web)
从 Oracle 迁移到 Postgres 的方法有很多，IvorySQL 的方法是新增相容性元素，例如支援 Oracle 的 PL/SQL 语法和 XML 函数。 [v5.0](https://postgresweekly.com/link/177678/web) 现在基于 Postgres 18，并引入了更多 Oracle 相容性功能以及对更多 Postgres 扩充功能的支援。此外，现在还有一个[线上 Playground](https://postgresweekly.com/link/177679/web)，您可以在其中体验实例。

`IvorySQL`


## **📰 分类广告**

🐘 [pgEdge Enterprise Postgres](https://postgresweekly.com/link/177680/web)：100% 开源、可扩充、设计正常运作时间高达 99.999%，并支援分散式部署。

🛣️ [《通往 Next.js 之路》](https://postgresweekly.com/link/177681/web)是由 Robin Wieruch 主讲的课程，旨在帮助学员使用 Next.js 15 和 React 19 进行全端 Web 开发。对于准备超越前端的 JavaScript 开发人员来说，这门课程堪称完美之选。

## [SynchDB 1.3：用于从其他资料库复制资料的插件](https://postgresweekly.com/link/177684/web)
一款专门用于可靠地从其他资料库系统（例如 MySQL、SQL Server 和 Oracle）复制资料的 Postgres 扩充。 v1.3 引入了一种新的、更快的基于 FDW 的快照引擎，以加快初始快照的效能。

`Hornetlabs Technology Inc`

## [Dbdock：全新的 PostgreSQL 备份与复原解决方案](https://postgresweekly.com/link/177686/web)

`Naheem Olaide`

[PGSync 6.1](https://postgresweekly.com/link/177687/web) – 用于将 Postgres 资料同步到 Elasticsearch/OpenSearch 的版本。现在无需 Redis 即可作为 WAL 消费者运作。

[Pgpool-II 4.6.4、4.5.9、4.4.14、4.3.17 和 4.2.24](https://postgresweekly.com/link/177688/web) – 连接池和负载平衡器。

[pgweb 0.17](https://postgresweekly.com/link/177689/web) – 基于 Web 的跨平台 Postgres 用户端。 （提供萤幕截图。）

[asyncpg 0.31](https://postgresweekly.com/link/177691/web) – 用于 Python 中 asyncio 的 Postgres 用户端函式库。

[Npgsql 10.0](https://postgresweekly.com/link/177692/web) – 用于 PostgreSQL 的 .NET 资料提供者。