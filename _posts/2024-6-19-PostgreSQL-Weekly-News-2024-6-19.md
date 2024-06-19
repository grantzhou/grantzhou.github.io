---
layout: post
title: PostgreSQL 每周新闻 2024-6-19
---
### PostgreSQL每周新闻#556 - 2024年6月19日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/559)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/o0qwrjfokr5qhbwfmqhg.jpg)
## [PGConf.dev 2024 回顾](https://postgresweekly.com/link/156490/web)
在最近的 Postgres 开发者大会上，Postgres 可能[没有提交任何commits](https://postgresweekly.com/link/156491/web)，但确实发生了很多事情。对于参加和未参加的人来说，这都是一份非常简洁而全面的总结。

`ANDREAS 'ADS' SCHERBAUM `
💡 David Wheeler 还分享了他参加上周微软举办的 [POSETTE 活动](https://postgresweekly.com/link/156493/web)的[一些笔记](https://postgresweekly.com/link/156492/web)。

## [▶ Postgres 扩展生态系统的现状](https://postgresweekly.com/link/156494/web)
David Wheeler 正在大力推动 Postgres 扩展的编目、发布和分发方式，他在 POSETTE 上发表了演讲，介绍了原因和方法，以及一些历史。他还撰写了关于在 PGConf․dev 举行的扩展生态系统峰会的文章。


`DAVID WHEELER (TEMBO) `
## [带翅膀的 Redis。性能更佳。开销更少](https://postgresweekly.com/link/156489/web)
Dragonfly（24k GitHub 星）是完全兼容的嵌入式 Redis 替代品。Dragonfly 的性能比 Redis 高出 25 倍，并且在单个实例上支持数百万 QPS。下载并自行部署或免费试用 Dragonfly Cloud。


`DRAGONFLY `
## [使用 ON CONFLICT 减少清理](https://postgresweekly.com/link/156496/web)
如果减少由于插入操作失败而导致的死元组数量，那么还可以减少 Postgres 清理表的需要。双赢。


`SHANE BORDEN `
## [身份危机：序列与 UUID 作为主键](https://postgresweekly.com/link/156497/web)
“如果谨慎使用，整数和 UUID 都可以提供相当可行的解决方案，（在我看来）适当利用的 UUID 略胜一筹。”


`BRANDUR LEACH `


**本周摘要：**


* [Postgres Ibiza](https://postgresweekly.com/link/156498/web) 将于今年 9 月回归，他们正在寻找[演讲嘉宾和赞助商](https://postgresweekly.com/link/156499/web)。（CFP 将于 6 月 23 日结束。）

* 遗憾的是，RDS 上 Postgres 的自动调优服务 [OtterTune](https://postgresweekly.com/link/156500/web) 在收购合约失败后不久就关闭了。

* 本周 PostgreSQL 人物的受访者是 [EDB 的 William Ivanski](https://postgresweekly.com/link/156502/web)。

## [如何在 macOS 上升级 Postgres.app](https://postgresweekly.com/link/155421/web)
Postgres.app 是一种在 macOS 上快速运行 Postgres 实例的流行方法，但如何在不丢失现有数据的情况下更新它呢？


`SIMON WILLISON `

📄 [从 Microsoft SQL Server 到 PostGIS](https://postgresweekly.com/link/156505/web) – 即使 Postgres 本身不足以吸引 SQL Server 用户，PostGIS 在空间数据集方面可能也足够吸引人！ FLORIAN NADLER

📄 [编译最新的 gcc](https://postgresweekly.com/link/156507/web) 以测试更多架构 – 这里没有太多要学的东西，但很高兴看到 Postgres 的测试有多彻底 - ROBINS THARAKAN

📄 [UUIDv7 以 20 种语言实现](https://postgresweekly.com/link/156508/web) – 是的，甚至包括 SQL - ANTON ZHIYANOV

📄 [使用 LLVM 编译 Postgres](https://postgresweekly.com/link/156509/web) - DAVID WHEELER

📺 面向 Python 开发人员的 [pgvector](https://postgresweekly.com/link/156510/web) - PAMELA FOX


**📰 机密：**


🚀 受益于 [Rocketadmin](https://postgresweekly.com/link/156511/web) 的高级数据库自检技术，该技术可检索所有相关元数据，以无缝创建您的[管理面板](https://postgresweekly.com/link/156511/web)。

最快的生产路径。借助 Render，您可以[轻松构建、部署和扩展您的应用程序](https://postgresweekly.com/link/156556/web) - 从您的第一个用户到您的第十亿个用户。

您错过了 [POSETTE：Postgres 活动吗](https://postgresweekly.com/link/156513/web)？这是所有 42 场演讲的[播放列表](https://postgresweekly.com/link/156513/web)。分享并点赞您的最爱！


[POSETTE](https://postgresweekly.com/link/155425/web)做好准备！ Postgres 的免费虚拟开发者活动（6 月 11 日至 13 日）。收听 4 个直播中的 42 场演讲中的一场或多场


**🛠 代码和工具**


## [pg_bestmatch.rs：使用 BM25 提升您的文本查询](https://postgresweekly.com/link/156514/web)
BM25 是一种流行的排名函数，可以改进大量文档的全文搜索。pg_bestmatch.rs 是一个扩展，它将 BM25 相关函数和统计数据生成引入 Postgres。


`JINJING ZHOU `

[ActiveRecord::PostgresEnum 2.1](https://postgresweekly.com/link/156517/web) – 将 Postgres 的枚举类型集成到 Ruby 和 Rails 的 Active Record 中。

[River 0.7](https://postgresweekly.com/link/156518/web） – 适用于 Go 的快速可靠的 Postgres 后台作业。

[无状态 Postgres 查询路由器 (SPQR) 1.4](https://postgresweekly.com/link/156519/web) – Yandex Cloud 的水平分片方法。

[pgwire 0.23](https://postgresweekly.com/link/156520/web) – Rust 库中的 Postgres 线路协议。现在支持 COPY。

[Piccolo 1.11](https://postgresweekly.com/link/156521/web) – 用户友好的 Python ORM 和查询生成器。