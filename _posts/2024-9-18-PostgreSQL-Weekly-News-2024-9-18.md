---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-9-18
---
### PostgreSQL每周新闻#570 - 2024年9月18日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/570)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/gmgpd26qifvuz9s4kgro.jpg)
## [优化数据库以进行分析](https://postgresweekly.com/link/159925/web)
您的数据库可能非常适合日常操作，但当您需要运行一些复杂的分析查询时，就会出现一些重大决策。您可以复制数据以各种方式在其他地方进行分析，或者调整 Postgres 以更好地处理事情。对所涉及的概念进行了全面的高层次了解。[还有 ▶️ 视频版本](https://postgresweekly.com/link/159926/web)。

`Karen Jex `

## [为什么要停止在 Postgres 中使用 SERIA](https://postgresweekly.com/link/159927/web)
SERIAL 是一种常用的生成自动递增 ID 列的便利方法，但它有各种怪癖，并且是 Postgres 特有的。替代方案？标识列，它们都是 SQL:2003 标准的一部分，并受 Postgres 支持。


`Naiyer Asif `
## [亲身体验 Postgres 17：新功能和性能影响](https://postgresweekly.com/link/159924/web)
加入我们，参加 Postgres 17 版本的独家网络研讨会。探索新的增强功能 — 更快的 B 树扫描、自适应真空策略和流式 I/O 更新 — 以及它们对数据库性能和监控的影响。立即注册！


`pganalyze  `
## [Postgres 17 RC1 与 sysbench 在小型和大型服务器上的比较](https://postgresweekly.com/link/159929/web)
如果您像我们一样焦急地等待下周发布的 Postgres 17，那么您可能想知道它在性能方面的表现如何。Mark 在 15.8、16.4、17 beta 3 和 17 RC1 上运行了一些基准测试，虽然有一些细节需要仔细研究，但总结是“17rc1 看起来很棒 - 没有大的倒退和几个大的改进。”


`Mark Callaghan  `

### 本周摘要：

* 🗣️ [Andrew Atkinson](https://postgresweekly.com/link/159930/web) 是本周 PostgreSQL 人物的受访者。Andrew 最著名的作品可能是他的[《High Performance PostgreSQL for Rails》](https://postgresweekly.com/link/159931/web)一书，这可能是迄今为止该系列中最详细、最全面的采访。

* David Wheeler [分享了 PGXN v2 项目的新功能](https://postgresweekly.com/link/159932/web)，这是一项大胆的尝试，旨在重新思考 Postgres 扩展背后的生态系统和分发。

* Stefan Fercot 介绍了上周 [PGDay UK 2024 的最新情况](https://postgresweekly.com/link/159933/web)以及那里发生的事情。


## [使用 Postgres 和 pgvector 实现混合搜索](https://postgresweekly.com/link/159934/web) 
Jonathan 开始向我们展示如何使用 pgvector 实现混合搜索系统，但他指出他还不想回答您是否应该这样做 — — 这是未来文章的主题。


`Jonathan Katz`
## [Postgres 数据分析的窗口函数](https://postgresweekly.com/link/159935/web)
当您想要对查询中已检索到的行进行分组或比较时，窗口函数非常有用 - 例如，计算累计总数、执行排名或计算滚动平均值。它们本质上提供了更高阶的查询。


`Elizabeth Christensen (Crunchy Data)`


### 📰 分类广告
* 在西雅图的 [PASS 数据社区峰会上与数千名数据专业人士交流](https://postgresweekly.com/link/159936/web)。浏览日程安排，了解 170 多个会议。

* [Dagster+](https://postgresweekly.com/link/159937/web) 让使用嵌入式 ELT 从 Postgres 提取和复制数据变得更加容易。立即开始使用 [Dagster+ 免费试用版](https://postgresweekly.com/link/159937/web)进行构建。

* 🐘 您是那些对 PostgreSQL 没有意见的开发人员之一吗？没错。在 [2024 年 PostgreSQL 调查中告诉我们您的真实想法](https://postgresweekly.com/link/159938/web)！

📄 [英特尔展示了针对 AVX-512 优化的 Postgres 高达 48% 的改进](https://postgresweekly.com/link/159939/web) - Phoronix

📄 [数据库中的 AI 代理：与 Pgai 一起教 Claude 使用工具](https://postgresweekly.com/link/159940/web) - Haziqa Sajid (Timescale)

📄 [从 Temporal 迁移到基于 Postgres 的任务编排器](https://postgresweekly.com/link/159941/web) - Robin Guldener (Nango)

📄 [使用复合和部分索引优化 Postgres](https://postgresweekly.com/link/159942/web) - Semab Tariq

📄 [使用零 ETL 在 S3 中使用 Parquet 实现 Postgres 物化视图](https://postgresweekly.com/link/159943/web) – 特别是使用 Crunchy Bridge for Analytics。 - Marco Slot (Crunchy Data)


### 🛠 代码和工具

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/c4wakjbajwvmy8owq9yc.jpg)

## [🐸 Rainfrog：Postgres 的新数据库管理 TUI](https://postgresweekly.com/link/159944/web)
我们和其他人一样喜欢 psql，但总是渴望看到新的东西，而这个由 Rust 驱动的终端 UI 非常优雅。您将获得一个具有突出显示、Vim 式快捷方式的查询编辑器，并且可以在模式之间快速切换。


`Carl Liu `
## [📱 Selectable：正在开发的 Android Postgres 客户端](https://postgresweekly.com/link/159945/web)
一款用于与 Postgres 交互的全新免费 Android 应用，诚然，它仍处于“早期阶段”，但现在可以在 Google Play 商店中试用。


`Selectable Software`

[🌐 PostGIS 3.5.0 Beta 1](https://postgresweekly.com/link/159946/web) – 流行地理空间扩展的最新版本已为 Postgres 17 做好准备。我们预计最终版本将在 Postgres 17 之后很快发布。

[E-Maj 4.5.0](https://postgresweekly.com/link/159947/web) – 数据库子集上的细粒度写入日志和时间旅行。

[Pongo 0.14.4](https://postgresweekly.com/link/159948/web) – Node.js 的 Postgres 驱动程序，以 MongoDB 样式 API 的形式呈现。

[Good Job 4.3](https://postgresweekly.com/link/159949/web) – Postgres 支持的 Ruby on Rails 作业队列。

[pgmoneta 0.14](https://postgresweekly.com/link/159950/web) – 备份/恢复工具。