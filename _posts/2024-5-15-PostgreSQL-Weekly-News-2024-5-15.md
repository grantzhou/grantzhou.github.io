---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-5-15
---
### PostgreSQL每周新闻#555 - 2024年5月15日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/555)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/srgba651kvcwksgtdc4o.jpg)
## [Postgres 17 发行说明草案](https://postgresweekly.com/link/155107/web)
Bruce 刚刚宣布他已经完成了 Postgres 17 发行说明的初稿（将于今年晚些时候发布）。目前它主要是低级改进的要点列表，但它让发布感觉更接近了！第一个测试版即将到期。

`BRUCE MOMJIAN `
## [将 Postgres 查询速度提高 1,000 倍](https://postgresweekly.com/link/155109/web)
如果您想引起博客文章的关注，那么您需要写这样的标题！但你还需要用一个故事、一个解决方案、一些有用的见解，也许还有一点幽默来支持它——值得庆幸的是，所有这些元素都在这里。


`ALEJANDRO GARCÍA MONTORO `
## [任何规模的 Postgres 性能](https://postgresweekly.com/link/155106/web)
通过智能索引和 VACUUM 顾问以及持续的数据库分析提供一致的数据库性能和可用性。 pganalyze 与 Amazon Web Services、Google Cloud Platform、Microsoft Azure 等集成。


`PGANALYZE `
## [Postgres 16.3、15.7、14.12、13.15 和 12.19 已发布](https://postgresweekly.com/link/155110/web)
Postgres 团队按计划发布了每个维护的发行版的新次要版本。 Bug 修复是焦点，但 Postgres 14-16 还修复了 pg_stats_ext 和 pg_stats_ext_exprs 的安全问题。 （请注意，Postgres 12 从今年 11 月起将停止接收修复。）


`PGANALYZE `

**本周摘要：**

* David Wheeler 最近做了一项民意调查，询问 PGXN v2 Postgres 扩展项目的新服务是否应该用 Go 还是 Rust 编写：[Rust 是明显的赢家](https://postgresweekly.com/link/155111/web)。


* 在 Google I/O 大会上，Google 推出了 [Firebase Data Connect](https://postgresweekly.com/link/155112/web)，这是一种将 Firebase 与托管在 Cloud SQL for PostgreSQL 上的 Postgres 实例结合使用的方法。

* Postgres 领域的招聘人员 Philip Marks 是[本周的 Postgres 人物](https://postgresweekly.com/link/155113/web)

* 🇧🇪 Stefan Fercot 有一些近期 [PGConf 比利时活动的笔记](https://postgresweekly.com/link/155114/web)。


## [Microsoft 2024 版 Postgres 的新增功能](https://postgresweekly.com/link/155115/web)
部分归功于购买 Citus Data，部分归功于 Azure，微软如今成为 Postgres 生态系统的重要贡献者，这是对他们最近发生的一切的令人惊讶的全面总结。


`MICROSOFT `
## [使用 coproc 进行高级 psql 脚本编写](https://postgresweekly.com/link/155116/web)
coproc 是一个 shell 命令，可在子 shell 中异步运行进程。如果您用它调用 psql，仍然可以从远处与它交互，具体方法如下。


`DANIEL VÉRITÉ `


**📰 机密：**


📚 通过 Simple Talk 编辑 Louis Davidson 推荐的[学习资源列表](https://postgresweekly.com/link/155117/web)，随时了解数据库技术和行业趋势。

您最快的生产途径。[借助 Render，您可以无比轻松地构建、部署和扩展您的应用程序](https://postgresweekly.com/link/155128/web) - 从第一个用户到第十亿个用户。


📄 使用 [pg_repack 扩展删除膨胀](https://postgresweekly.com/link/155118/web) – pg_repack 是一个扩展，用于在线删除表和索引的膨胀，而无需持有独占锁 - MUHAMMAD ALI

📄 [何时为 Postgres 拆分补丁](https://postgresweekly.com/link/155119/web) – 对于那些积极为 Postgres 做出贡献的人 - PETER EISENTRAUT

📄 [处理从 Oracle 到 Postgres 的迁移中的不可见索引](https://postgresweekly.com/link/155120/web) - DEEPAK MAHTO



**🛠 代码和工具：**


## [pg_lakehouse：从 Postgres 查询任何数据湖](https://postgresweekly.com/link/155121/web)
一个扩展，可让您查询 S3 等对象存储和 Delta Lake 等表格式。查询被推送到 Apache DataFusion。很快将支持 Google Cloud Storage 和 Azure Blob Storage。


`PARADEDB `

[ParadeDB 0.7](https://postgresweekly.com/link/155122/web) – 用于搜索和分析的 Postgres。

[PostgREST 12.0.3](https://postgresweekly.com/link/155123/web) – 适用于任何 Postgres 数据库的 REST API。

[Prisma 5.14](https://postgresweekly.com/link/155124/web) – 适用于 Node.js 和 TypeScript 的流行 ORM。

[ScalikeJDBC 4.3](https://postgresweekly.com/link/155125/web) – Scala 的数据库客户端库。

[DoltgreSQL 0.7](https://postgresweekly.com/link/155126/web) – 类似 Postgres 的版本控制。

[pspg 5.8.6](https://postgresweekly.com/link/155127/web) – 用于表格数据的 Unix 终端寻呼机。