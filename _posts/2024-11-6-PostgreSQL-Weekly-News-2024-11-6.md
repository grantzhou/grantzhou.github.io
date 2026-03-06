---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-11-6
---
### PostgreSQL每周新闻#576 - 2024年11月6日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/576)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/hp4tf2174usd9lpqvgmo.jpg)
## [堵住 Postgres 升级漏洞？](https://postgresweekly.com/link/161846/web)
作者声称社区讨论经常提出 Postgres 难以升级的观点——但这是一个公平的观点吗？Shaun 研究了 Postgres 如何进行升级、pg_upgrade 方法的局限性，并考虑了如何使事情变得更好。

`Shaun Thomas (Tembo)`
## [从 Postgres 就地迁移到 MySQL – (!)](https://postgresweekly.com/link/161848/web)
这不是我们在这里讨论的典型迁移！但 Yelp 作为 MySQL 的重度用户，在需要集成他们收购的 Postgres 网站时发挥了重要作用。由于 Postgres 特定的功能，他们不得不做出一些妥协，但由于内部缺乏 Postgres 技能，他们认为这是必要的牺牲。


`Alex Toumazis (Yelp) `
## [以一半的成本将 GitHub Actions 运行速度提高 2 倍](https://postgresweekly.com/link/161845/web)
Blacksmith 通过在现代游戏 CPU 上运行 GitHub Actions，可显著提高运行速度。集成 Blacksmith 只需更改一行代码。Ashby、Superblocks 和 Slope 等 100 多家公司使用 Blacksmith 帮助开发人员更快地合并代码。


`Blacksmith  `
## [Amazon Aurora PostgreSQL 无限数据库正式发布](https://postgresweekly.com/link/161849/web)
一种水平扩展/分片 Amazon Aurora 的新方法，可将数据库扩展到 Aurora 的典型存储和写入吞吐量限制之外，同时仍然看起来和感觉像一个数据库。它现在是 GA，兼容 Postgres 16.4。


`Channy Yun (AWS)`

### 本周摘要：

[postgres-contrib.org](https://postgresweekly.com/link/161850/web) 是一个博客，主要每周汇总对 Postgres 项目的贡献。

[🗓️ PostgreSQL 事件日历](https://postgresweekly.com/link/161851/web)是一个跟踪 Postgres 导向事件的网站，还托管一个 ICS / iCalendar 文件，您可以将其添加到自己的日历应用程序中。

[EDB 的 Rushabh Lathia](https://postgresweekly.com/link/161852/web) 是本周 PostgreSQL 人物的受访者。


## [向量数据库是错误的抽象](https://postgresweekly.com/link/161853/web) 
对于语义搜索，Timescale 认为从外部生成嵌入向量然后将其放入数据库是错误的方法，而嵌入应该更像数据库索引并由数据库处理。Pgai Vectorizer 是他们实现这一目标的尝试。


`Arye and Sewrathan (Timescale)`
## [Postgres 与 MariaDB 和 MySQL 的基准测试](https://postgresweekly.com/link/161855/web) 
使用定制的基准测试工具 Reserva，作者发现 Postgres 在性能方面处于领先地位。关于基准测试和获取准确结果的麻烦等的常见免责声明。


`Cal Mitchell`
## [如何使用 OpenAI CLIP、Postgres 和 JavaScript 构建图像搜索应用程序](https://postgresweekly.com/link/161588/web) 
本教程将许多想法汇集在一起​​。CLIP 用于将图像转换为文本描述。Postgres 用作矢量数据库。JavaScript 为前端（使用 React）和后端（Node.js）提供了粘合剂。


📄 [探索 Postgres 全文搜索：入门指南](https://postgresweekly.com/link/161857/web) – 重点介绍经典的 tsvector/tsquery 方法和相关函数。Rémi Mercier

📄 [避免在 Postgres 名称中使用大写字母](https://postgresweekly.com/link/161858/web) – 这样可以省去很多麻烦。Wei Yen

📄 [SQL Server 和 Postgres 之间的 5 大主要区别](https://postgresweekly.com/link/161859/web) Klaus Aschenbrenner

📄 [为什么您不想使用 C/POSIX 语言环境](https://postgresweekly.com/link/161860/web) Christophe Pettus

📄 [为什么 pg_dump 很棒](https://postgresweekly.com/link/161861/web) Robert Haas


![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/mj8pvyxrgdnaf7mqntet.jpg)



## [pg_flo：实时流式传输、转换和路由 Postgres 数据](https://postgresweekly.com/link/161862/web)
提供一组过滤器和转换功能，可以使用以下两种模式之一轻松在生产数据库和暂存数据库之间移动数据：复制和流式传输或仅流式传输。使用 NATS 和 Postgres 的复制。


`Shayon Mukherjee`
## [OneSparse：用于 Postgres 的加速稀疏线性代数](https://postgresweekly.com/link/161863/web)
就像 JSON/JSONB 类型对非结构化数据的作用一样，OneSparse 希望使密集和稀疏矩阵和向量成为完全原生的 Postgres 类型，同时优化并行矩阵乘法和其他操作，如归约、选择、分配、提取、逐元素联合和交集。


`Michel Pelletier`
## [pgCompare：一款用于检查复制后数据一致性的 Java 应用程序](https://postgresweekly.com/link/161864/web)
例如，如果您将数据从一个数据库移动到另一个数据库，则可以使用它进行比较来检查迁移的完整性。


`Crunchy Data`
## [ProxySQL 将数据库支持扩展到 Postgres](https://postgresweekly.com/link/161865/web)
ProxySQL 是一个开源 MySQL 代理，现在，它在其 v3.0 版本发布之前引入了 Postgres 支持。v3.0.0-alpha 现在可以供测试。


`ProxySQL LLC`


### 📰 分类广告

🧐 正在为 Postgres 查询速度慢而苦恼？[加入我们 11 月 13 日的网络研讨会](https://postgresweekly.com/link/161868/web)，了解 pganalyze 如何简化 EXPLAIN 计划比较以调试常见问题。


## [pg-dump-parser：将 Postgres 转储文件解析为模式对象数组](https://postgresweekly.com/link/161869/web)
获取 Postgres 数据库转储，将其拆分，并将表和视图结构转换为您可以更轻松地从代码处理的格式（或仅用作参考或检查版本控制）。


`Gajus Kuizinas`

[rusty_psql：用于从 Azure Key Vault 获取凭据的 psql 包装器](https://postgresweekly.com/link/161870/web)
`Claus Guttesen`

[pgwire 0.26](https://postgresweekly.com/link/161871/web) – 在 Rust 库中实现的 Postgres 线路协议。

[Rest 0.2](https://postgresweekly.com/link/161872/web) – 从 SQL 数据库提供完全 RESTful API。

[PeerDB 0.19](https://postgresweekly.com/link/161873/web) – 将数据从 Postgres 流式传输到数据仓库、队列和存储引擎。

[PostgreSQL-OCaml 5.1](https://postgresweekly.com/link/161874/web) – OCaml 的 Postgres 绑定。

[PostgreSQL Build Farm Client v18](https://postgresweekly.com/link/161875/web)