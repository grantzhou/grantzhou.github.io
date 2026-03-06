---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-5-1
---
### PostgreSQL每周新闻#598 - 2025年4月3日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/598)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/gm0omqymldqlicv5hgup.jpg)
## [PGlite 0.3：WASM 上的 Postgres，现已基于 Postgres 17](https://postgresweekly.com/link/168701/web)
PGlite 是基于 WebAssembly 的 Postgres 版本，可让您在任何支持 WebAssembly 的环境中运行 Postgres 实例（例如本演示中的浏览器）。v0.3 向升级到 Postgres 17.4 迈出了一大步。（[GitHub 代码库](https://postgresweekly.com/link/168703/web)）

`ElectricSQL`

## [删除列时究竟发生了什么](https://postgresweekly.com/link/168704/web)
运行 ALTER TABLE .. DROP COLUMN 命令时，你可能不会过多思考幕后发生了什么，但有时该过程的细节可能会让你感到不安。简而言之，“删除”的列可能会消失，但不会被遗忘。


`Gwen Shapira`
## [您的应用程序是否已为下一次高流量事件做好准备？](https://postgresweekly.com/link/168700/web)
您是否厌倦了 Postgres 数据库如同黑匣子般烦扰？观看此点播视频，了解 Postgres 专家 Lukas Fittl 如何使用最新的 pganalyze 功能来调优慢查询、捕捉回归问题，并保持 Postgres 的最佳运行状态。


`pganalyze   `
## [Jepsen：Amazon RDS for PostgreSQL 多可用区集群违反了快照隔离](https://postgresweekly.com/link/168705/web)
Jepsen 以其对分布式系统的分析而闻名。经过一些实验，作者发现 Amazon RDS for PostgreSQL 多可用区集群（具体来说）违反了快照隔离，这是所有终端节点支持的最强一致性模型。


`Kyle Kingsbury`
## [为什么所有工作流都应该是 Postgres 行](https://postgresweekly.com/link/168706/web)
DBOS 持久执行/工作流库背后的人们认为将工作流存储在 Postgres 中是个好主意，这可能并不奇怪，但从模式 POV 的角度来看，他们是这样认为的。


`Kraft and Li (DBOS)`

📄 [Postgres planner CTE、DELETE 和 LIMIT 陷阱](https://postgresweekly.com/link/168707/web) – “看似简单的事情，却与查询规划器发生了意想不到的交互。” Shayon Mukherjee

📄 [面向初学者的 Trusted Extensions 讲解](https://postgresweekly.com/link/168708/web) Pavlo Golub

📄 [Postgres 到 ClickHouse：数据建模技巧](https://postgresweekly.com/link/168709/web) Palacin 和 Srirampur (ClickHouse)


### 快速发布：

[DbGate 6.4](https://postgresweekly.com/link/168710/web) – 适用于 SQL 和 NoSQL 数据库的数据库管理应用。现在也支持 DuckDB。

[pgAdmin 4 v9.3](https://postgresweekly.com/link/168711/web) – 广受欢迎且功能丰富的管理工具。

[pspg 5.8.9](https://postgresweekly.com/link/168712/web) – 用于表格数据的 Unix 终端分页器。

[Dbmate 2.27](https://postgresweekly.com/link/168713/web) – 框架无关、基于 Go 语言的数据库迁移工具。

[Good Job 4.10](https://postgresweekly.com/link/168714/web) – 基于 Postgres 的 Ruby on Rails 任务队列。