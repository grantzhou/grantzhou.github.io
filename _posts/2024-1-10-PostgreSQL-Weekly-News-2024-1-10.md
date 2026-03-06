---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-1-10
---
### PostgreSQL每周新闻#537 - 2024年1月10日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/537)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/h0xbupjdciyomnzbp002.jpg)
## [PostgreSQL：2023 年度 DBMS](https://postgresweekly.com/link/149707/web)
🏆数据库引擎< a i=4> 是一个历史悠久的网站，收集有关（480 且还在增加）数据库系统的信息，跟踪它们的相对受欢迎程度，并分享哪个数据库获得了成功与上一年相比最受欢迎的。这次是 Postgres！


`Gelbmann and Andlinger (DB Engines) `
## [2024 年对 Postgres 的思考](https://postgresweekly.com/link/149710/web)
Jonathan 表示，Postgres 处于一个很好的位置，他涉及与 Postgres 短期未来相关的大量主题，包括复制、非阻塞架构更改、并行重播更改的能力以及社区建设工作。


`Jonathan Katz `
## [Neon Serverless Postgres 上的更改数据捕获](https://postgresweekly.com/link/149741/web)
Neon 上现在可以使用通过逻辑复制进行的标准 Postgres CDC。将更改同步到 OLAP 数据库，将更新流式传输到 Kafka，与 WAL 一样，可能性是无穷无尽的！


`Neon Serverless Postgres `
## [Postgres 17 添加了对增量备份的支持](https://postgresweekly.com/link/149711/web)
Postgres 17 还需要几个月的时间，但很高兴看到这样的功能被提交。 Robert Haas 分享了关于用例的一些想法。


`Hubert (depesz) Lubaczewski `
**本周摘要：**
*   🇮🇳PGConf India刚刚分享了 2024 年的日程安排并开始售票。它于二月底在班加罗尔举行。


*   🇪🇺 2024 年 FOSDEM PGDay 日程已发布。时间为 2 月 2 日，比利时布鲁塞尔 - 门票可售。


*   🇧🇪 同样在比利时，有一个“保存日期” PGConf.BE 将于 5 月 7 日举行。


*   📅如果您想在 Postgres 活动中发言，Claire Giordano 写信告诉我们芝加哥 PGDay 和 PGConf.dev 的 CFP 将于下周一结束。


*   Peter Eisentraut 分享了他使用 clangd 与 Emacs 处理 Postgres 代码库的经验。


*   pgAnalyze 已创建VACUUM 模拟器。这是他们商业产品的一部分，但这篇文章本身很有趣。


*   AWS 已宣布 Amazon Aurora Serverless v1（尤其可以缩减至零）在 2024 年之后将不再受支持。


*   The Register 有一篇关于 Postgres 先驱 Michael Stonebraker 的专题文章，讲述了他如何“承诺颠覆数据库”。再一次。


## [我的 Postgres 愿望清单](https://postgresweekly.com/link/149722/web)
我们喜欢 Postgres，但它总是可以变得更好[需要引用] 😏。 Ryan 希望围绕他所提出的一些改进想法展开对话 - 这里没有太多争议，这是一个可靠且有趣的列表。


`Ryan Guill `
## [如何“复制并粘贴” 5 分钟内创建新的 Postgres 开发环境](https://postgresweekly.com/link/149723/web)
主要针对那些想要查看 Postgres 源代码并使其快速启动并运行的人们，尤其是在 EC2 上。


`Jeremy Schneider `
## [pg_rman：备份和恢复管理工具](https://postgresweekly.com/link/149726/web)
Postgres 备份和恢复工具有很多，但 pg_rman 的功能包括支持时间点恢复 (PITR) 及其方式可以管理和编目多个备份版本。


`NTT OSS Center DBMS Development and Support Team `
## [pg_savior：防止危险删除的扩展](https://postgresweekly.com/link/149728/web)
防止因不带 子句的 DELETE 查询导致意外数据丢失限制范围。 实现非常简单（如果其工作原理有点天真），但这是一个可爱的想法，可能会对您自己的类似扩展产生启发。实现非常简单（如果其工作原理有点幼稚）。


`Vignesh Ravichandran `
## [gptsql：LLM 与您的 Postgres 数据库聊天 ](https://postgresweekly.com/link/149730/web)
🤖一个实验性工具，它将 OpenAI 的 GPT 模型和您的 Postgres 数据库结合在一起，以便询问关于/“到”的问题实时（嗯，实时-ish）。自述文件中有一个演示视频展示了这个想法。


`Tatari `
## [介绍prometheus_fdw：Postgres 中的无缝监控](https://postgresweekly.com/link/149731/web)
“您拥有的是：所有监控数据和分析都存储在Prometheus 中。 您想要的：您的 Postgres 数据库中的所有数据...”


`Owens and Ankenman (Tembo) `
## [Parquet S3 FDW 1.1](https://postgresweekly.com/link/149732/web)
 -  适用于 Amazon S3 上的 Parquet 文件的 FDW。

## [pg_easy_replicate 2.0](https://postgresweekly.com/link/149733/web)
 -  一种设置逻辑复制和复制的方法切换。

## [sqlc 1.25](https://postgresweekly.com/link/149734/web)
 -  从 SQL 生成类型安全的 Go 代码。

## [PGSync 3.1](https://postgresweekly.com/link/149735/web)
 -  Postgres 到 Elasticsearch/OpenSearch 同步。

## [pgwatch2 1.12](https://postgresweekly.com/link/149736/web)
 -  Postgres 指标监视器/仪表板。

## [pgBadger 12.4](https://postgresweekly.com/link/149737/web)
 -  快速 Postgres 日志分析工具。

## [pgwire 0.19](https://postgresweekly.com/link/149738/web)
 -  Rust 库中的 Postgres 线路协议。

## [pg_dbms_metadata v1.0.0](https://postgresweekly.com/link/149739/web)

## [InfluxDB FDW 2.1.0](https://postgresweekly.com/link/149740/web)



# 💡本周提示


**🗓即将举办的Postgres活动**
