---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-11-20
---
### PostgreSQL每周新闻#578 - 2024年11月20日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/578)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/xgy2mwq6o3qe9bdghco8.jpg)
## [Postgres 17.1、16.5、15.9、14.14、13.17 和 12.21 发布](https://postgresweekly.com/link/162481/web)
Postgres 每个维护系列的发布汇总，包括错误修复和四个安全问题的修复。12.21 也标志着 Postgres 12 的最终发布。不过，升级到 Postgres 17.1 时要小心，因为存在一些潜在的兼容性问题......请参阅下一个项目！

`PostgreSQL Global Development Group`
## [ResultRelInfo 的更改：Postgres 17.1 的险些失误](https://postgresweekly.com/link/162482/web)
Postgres 17.1 版本中看似微小的更改导致与某些扩展（例如 TimescaleDB 和 Apache AGE - 请参阅 [TimeScale 的 CTO 在此处所说内容](https://postgresweekly.com/link/162483/web)）出现兼容性问题。Craig 解释了问题是什么以及为什么会出现，并提醒我们开发能够适应此类更改的扩展是一项全职工作。


`Craig Kerstiens `
## [Postgres 为数据仓库重新设计](https://postgresweekly.com/link/162480/web)
C​​runchy 数据仓库结合了托管存储、强大的分析引擎和统一的数据管道。使用熟悉的 Postgres 工具无缝查询数据，同时还具有列式存储和性能的额外优势。


`Crunchy Data  `
## [使用 UNNEST 将 INSERT 性能提高 50%](https://postgresweekly.com/link/162484/web)
您可能知道，使用 COPY 通常是将数据大规模导入 Postgres 的最快方法，但 INSERT 因其额外功能而保留了一些优势。INSERT 可以加速吗？UNNEST 的出现将改变现状。


`James Blackwood-Sewell`

### 本周摘要：

📅 微软的虚拟 [POSETTE Postgres 会议](https://postgresweekly.com/link/162485/web)将于 2025 年回归，如果您想发言，现在可以[征集提案](https://postgresweekly.com/link/162486/web)。会议将于 2025 年 6 月举行，但您必须在 2 月 9 日之前提交提案。

📅 [PGConf.dev 2025](https://postgresweekly.com/link/162488/web) 的 [CFP](https://postgresweekly.com/link/162487/web) 将于明年 5 月在蒙特利尔举行，目前也开放至 1 月 1 日。

🗣️ [EDB 的 Ayse Bilge Ince](https://postgresweekly.com/link/162489/web) 是本周 PostgreSQL 人物的受访者。

🧊 [Crunchy Data 推出了 Crunchy Data Warehouse](https://postgresweekly.com/link/162507/web)，这是一项将高性能分析数据库引入 Postgres 的托管服务。


## [使用 Rollup 和 Cube 在 Postgres 中轻松进行总计和小计](https://postgresweekly.com/link/162490/web) 
方便的附加功能，可用于执行更多分析查询。ROLLUP 可以创建分层小计以及总计，而 CUBE 可以针对分组列的每种可能组合生成小计。


`Elizabeth Christensen`
## [加载世界：不到 4 小时即可导入 OpenStreetMap](https://postgresweekly.com/link/162491/web) 
您是否知道 OpenStreetMap 的数据库大小高达 750GB，您可以获取它并自行设置，作为对 Postgres 进行压力测试的一种方式？Greg 研究了提取所需的时间、如何加快速度以及多年来的性能改进。（轻微剧透：在这个基准测试中，Postgres 17 比 Postgres 16 快 3%。）


`Greg Smith`
## [在 Spot VM 上运行 Postgres？🤯](https://postgresweekly.com/link/162492/web) 
在 PGConf Europe 的一次演讲中，Kaarel 研究了在可能随时消失的实例上运行 Postgres 的可行性。pg-spot-operator 是他为实现这一目标而构建的实用程序。


`Kaarel Moppel`
## [Postgres 的厄运：当排序规则改变时](https://postgresweekly.com/link/162494/web) 
当提供区域设置的库从现有 Postgres 数据库下更改时会发生什么？情况不太妙……


`Christophe Pettus`

📄 [当您在 Postgres 中修改一行时，幕后会发生什么](https://postgresweekly.com/link/162495/web)？ Semab Tariq

📄 [将数据分组为总和数组 - 使用自定义聚合的乐趣](https://postgresweekly.com/link/162496/web)。 Hubert depesz Lubaczewski

📄 [从 Postgres 访问大型语言模型](https://postgresweekly.com/link/162497/web) - 了解几种方法。 Paul Ramsey


### 🛠 代码和工具

## [pglite-fusion：在 Postgres 表中嵌入 SQLite 数据库](https://postgresweekly.com/link/162498/web)
这是一种扩展，它使您能够通过一种特殊的新 SQLITE 列类型将 SQLite 数据库嵌入到 Postgres 表中（因此，表中的每一行本身都可以有一个嵌入的 SQLite 数据库..）


`frectonz`
## [DBngin：Mac 和 Windows 上的简单 Postgres、MySQL 和 Redis](https://postgresweekly.com/link/162499/web)
您可以使用 Docker，可以使用 Postgres.app......但如果您想使用简单的 UI 启动几个常见数据库的不同版本，那么这可能符合要求。


`DBngin`
