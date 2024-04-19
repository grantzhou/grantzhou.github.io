---
layout: post
title: PostgreSQL 每周新闻 2024-4-17
---
### PostgreSQL每周新闻#551 - 2024年4月17日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/551)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/qrnxqrhzcdpmtmn11slw.jpg)
## [我最期待的 Postgres 17 功能](https://postgresweekly.com/link/153913/web)
距离发布还有几个月的时间，但 Postgres 17 正在成为另一个伟大的版本。 今天的问题中有很多内容都是关于 Postgres 17 的 - 每个人都感到兴奋！


`Henrietta Dombrovskaya `
## [📊 Postgres 优化器的十年改进](https://postgresweekly.com/link/153914/web)
“我决定在 PostgreSQL 8 到 16 上运行连接顺序基准 (JOB)1。我记录了每个数据库版本的第90个百分位数的查询延迟。”


`Ryan Marcus `
## [使用 OtterTune 提高 Postgres 性能并降低成本](https://postgresweekly.com/link/153912/web)
自动调整和优化旋钮，并获取索引和查询建议，以及表和 autovacuum 见解。 客户的性能提高了 90% 以上，并节省了数千美元的数据库劳动力成本。 进行 30 天免费试用。


`OtterTune `
## [Supabase 宣布“全面可用”](https://postgresweekly.com/link/153915/web)
我没有注意到 Supabase 一直处于“测试版”状态，但 Postgres、身份验证、实时和边缘功能平台已经决定 - 大约 100 万个数据库进入了他们的旅程 -现在他们“ 一切准备就绪！

在 Supabase 的其他新闻中，Oriole 团队已加入 Supabase。 如果您还记得，OrioleDB 是为 Postgres 创建新的“云原生”存储引擎的努力。

`Supabase `

**本周摘要：**

*   📈 在 [2024 年 4 月最新的 DB-Engines 数据库排名中](https://postgresweekly.com/link/153918/web)，Postgres 的受欢迎程度增幅最大。

*   🚀 [Neon 的无服务器 Postgres 平台](https://postgresweekly.com/link/153919/web)现已全面可用。 该消息在 Hacker News 上引起了不小的[讨论](https://postgresweekly.com/link/153920/web)。


*   🪙 您知道 Postgres 项目会向贡献者[赠送礼物](https://postgresweekly.com/link/153921/web)吗？ 这是 Luca Ferrari 新收到的 [Postgres 16 硬币](https://postgresweekly.com/link/153922/web)的样子。 😍


*   🎧 Hacking Postgres 播客第二季回归，并以对 High-Performance PostgreSQL for Rails 的作者 [Andrew Atkinson 的采访](https://postgresweekly.com/link/153923/web)开始。


*   ✍️ Christoph Berg 分享了上周 [PGConf.de 2024 的快速报告](https://postgresweekly.com/link/153924/web)。

*   🙏 [SQL/JSON 会“回归”Postgres 吗](https://postgresweekly.com/link/153925/web)？ 我们希望如此。


## [Postgres 角色和权限](https://postgresweekly.com/link/153926/web)
一种遵循教程风格的指导，帮助您了解角色和权限如何工作。


`Raminder Singh (Supabase) `
## [Postgres 17 中使用最小锁定合并和拆分分区的用例](https://postgresweekly.com/link/153927/web)
Postgres 17 中将提供一些有关管理分区表的有趣新功能。


`Andrew Atkinson `
## [Postgres 17 和 Psycopg 3.2 中改进的查询取消](https://postgresweekly.com/link/153928/web)
Postgres 17 将获得一些改进的查询取消功能，Python 用户有望从第一天起就能够利用这一功能。


`Denis Laxalde `


📄 [我在 Rust 中构建 Postgres 扩展所学到的知识](https://postgresweekly.com/link/153929/web) GOODNESS DURU

📄 [PL/pgSQL 转换陷阱：如何处理冲突变量](https://postgresweekly.com/link/153930/web) DEEPAK MAHTO

📄 [使用 pg_repack 在线重建表](https://postgresweekly.com/link/153931/web) MANISNKAR K 

📄 [Postgres 逻辑解码的五个技巧](https://postgresweekly.com/link/153932/web) SAI SRIRAMPUR

📄 [Postgres 会使用我的索引吗？](https://postgresweekly.com/link/153933/web) 丹尼斯·玛格达

📄 [伟大的技术博客的要素是什么](https://postgresweekly.com/link/153934/web) PHIL EATON


**机密：**


在 Simple Talk 的这个由[三部分组成的系列中](https://postgresweekly.com/link/153935/web)，了解如何使用 PostgreSQL 促进数据转换和分析过程。

📧 如果您从事浏览器技术、CSS、HTML、Web API 等方面的工作，请务必查看 [Frontend Focus](https://postgresweekly.com/link/153936/web)，这是我们涵盖前端所有内容的姊妹通讯。


## [这个由简单谈话的三部分系列](https://postgresweekly.com/link/153935/web)
了解如何使用PostgreSQL IN增强数据转换和分析过程。

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/pbbhelns7nz6fq0bnyz2.jpg)

## [Vasco：MIC 和 MINE 统计扩展](https://postgresweekly.com/link/153937/web)
最大信息系数 (MIC) 和基于最大信息的非参数探索 (MINE) 是统计度量，可用于探索多维数据集并查找其中的重要关系。


`Florents Tselai `
## [Postgres + SQLite = pglite？](https://postgresweekly.com/link/153939/web)
不要与 Postgres 的 PGlite WASM 版本混淆，这是一个由 Go 支持的快速概念证明，可将 Postgres 有线协议置于 SQLite 之前。


`viggy28 `
## [trdsql：对基于文本的数据执行 SQL 查询的工具](https://postgresweekly.com/link/153941/web)
一种 CLI 工具，可以对 CSV、LTSV、JSON、YAML 和 TBLN 文件执行 SQL 查询（采用 Postgres 或 MySQL 语法）。 它还可以用作 Go 应用程序中的库。


`Noboru Saito `
## [PERST 1.5](https://postgresweekly.com/link/153943/web)
 - 一个安息的API坐在Postgres数据库前。


[perst 1.5](https://postgresweekly.com/link/153943/web) – 位于 Postgres 数据库前面的 RESTful API。

[pg_graphql 1.5.3](https://postgresweekly.com/link/153944/web) – 为 Postgres 提供 GraphQL 支持。

[Bytebase 2.15](https://postgresweekly.com/link/153945/web) – 团队的数据库开发和 CI/CD 系统。

[RisingWave 1.8.1](https://postgresweekly.com/link/153946/web) – 兼容 Postgres 的流数据库。

[DoltgreSQL 0.6](https://postgresweekly.com/link/153947/web) – 版本控制的 Postgres。

[pspg 5.8.4](https://postgresweekly.com/link/153948/web) – 用于表格数据的 Unix 终端寻呼机。
