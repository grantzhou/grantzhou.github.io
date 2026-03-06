---
layout: post
title: PostgreSQL 每周新闻 2026-2-11
---
### PostgreSQL每周新闻#635 - 2026年2月11日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/635)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/v1770818766/x4lxggckbr96igv3cbko.jpg)

## [📈 'Postgres Postmaster Does Not Scale'](https://postgresweekly.com/link/180539/rss)
一个案例研究揭示了Postgres单线程`postmaster`进程在突发工作负载下的瓶颈。Elliot带来了图表和示意图来说明问题，以及他的团队如何提高吞吐量。不过在大多数情况下，连接池或代理可以缓解这个问题，如果你把`max_connections`设置得很高，是时候检查你的连接管理策略了。

**Elliot Levin**


## [Enterprise Grade Postgres for Agentic AI, High Availability and More](https://postgresweekly.com/link/180540/rss)
pgEdge为Agentic AI和需要高可用性、可靠性和数据主权的企业应用提供开源、100% Postgres基础设施。我们让大规模构建、部署和管理企业级Postgres应用变得简单。

**pgEdge** 赞助商


## [🔒 Postgres Locks Explained](https://postgresweekly.com/link/180541/rss)
*"这是我刚开始学习锁时希望存在的资源"*，作者（Supabase的工程师）说。这个网站专注于以易于理解的方式解释Postgres中使用的不同类型的锁，还配有[交互式图表](https://postgresweekly.com/link/180542/rss)来查看哪些类型的查询使用哪些类型的锁。

**TheOtherBrian1**


**简讯：**

- 🗣️ 世界各地有许多[Postgres用户组](https://postgresweekly.com/link/180543/rss)，他们正在寻找演讲者。你也可以远程演讲。这里是[如何注册你的兴趣](https://postgresweekly.com/link/180544/rss)。

- 🇹🇭 [FOSSASIA PGDay 2026](https://postgresweekly.com/link/180546/rss)（3月10日在泰国曼谷）的[日程](https://postgresweekly.com/link/180545/rss)已经发布。

- 下个月在加州帕萨迪纳举行的[SCALE 23x](https://postgresweekly.com/link/180548/rss)将有[PostgreSQL实践培训日](https://postgresweekly.com/link/180547/rss)。

- Microsoft分享了[涵盖*Azure Database for PostgreSQL*的1月月度更新](https://postgresweekly.com/link/180549/rss)。


## [Reading Buffer Statistics in `EXPLAIN` Output](https://postgresweekly.com/link/180550/rss)
`EXPLAIN`的缓冲区统计帮助你找出时间花在哪里（I/O是延迟的臭名昭著的原因！），当你调查查询时。了解共享命中、磁盘读取、临时溢出和计划缓冲区实际上意味着什么，以及如何使用这些数字来诊断真实的性能问题。

**Radim Marek**


## [▶ Postgres FM: A Weekly Postgres Podcast](https://postgresweekly.com/link/180551/rss)
Michael Christofides和Nik Samokhvalov近四年来几乎每周都会出现，通常还会邀请令人印象深刻的嘉宾，并且越来越好。例如：[他们最近与PgDog的Lev Kokotov的对话](https://postgresweekly.com/link/180552/rss)。

**Postgres FM** podcast


## [Supporting ChatGPT on Postgres in Azure](https://postgresweekly.com/link/180553/rss)
OpenAI最近分享了[用Postgres扩展到8亿用户的故事](https://postgresweekly.com/link/180554/rss)。现在，Microsoft分享了他们这方面的故事。

**Affan Dar (Microsoft)**


📄 [Recreating PlanetScale's `pg_strict` in Rust: A Build Log](https://postgresweekly.com/link/180555/rss) – 一种在运行前捕获危险UPDATE和DELETE语句的方法。*Mohd Kamran Tahir*

📄 [Building Personalized Search Without Leaving Postgres](https://postgresweekly.com/link/180556/rss) – 构建个性化推荐引擎的实用指南。*Ankit Mittal (ParadeDB)*


## 🛠 代码和工具

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/v1770814087/dkqqzxypd0gfudnkrfoh.jpg)

## [😍 ErwinDB: A Postgres Expert in a TUI App](https://postgresweekly.com/link/180557/rss)
这让我很高兴！这是一个TUI，用于浏览和查询Postgres贡献者Erwin Brandstetter的Stack Overflow答案。它离线工作，涵盖了他多年来数千个高质量的答案，配有语义搜索。

**Ara Hacopian**


## [pgstream 1.0: Postgres Replication with DDL Changes](https://postgresweekly.com/link/180558/rss)
这个CDC工具现在通过直接将DDL事件发送到WAL中来复制模式更改，使用DDL语句作为事实来源。如果你处理过模式漂移或CDC在模式演化时中断的问题，这是一个巧妙的方法。[GitHub仓库。](https://postgresweekly.com/link/180559/rss)

**Xata**


## [PGMQ: A Lightweight Message Queue Extension](https://postgresweekly.com/link/180560/rss)
类似AWS SQS，但在Postgres内部，没有后台工作进程或外部依赖。你可以获得消息的"正好一次"交付保证、与SQS的API一致性、FIFO队列等。[GitHub仓库。](https://postgresweekly.com/link/180561/rss)

**Tembo**


- [VectorChord 1.1](https://postgresweekly.com/link/180562/rss) – 高效的向量相似度搜索扩展，现在支持8位和4位RaBitQ量化向量类型，因此你可以使用更少的存储空间。

- [Oban 0.5](https://postgresweekly.com/link/180563/rss) – Python作业编排框架，由Postgres支持。

- [pgrx v0.17](https://postgresweekly.com/link/180564/rss) – 用Rust构建Postgres扩展的框架。

- [PostGIS Patch Releases](https://postgresweekly.com/link/180565/rss) – PostGIS 3.0-3.6的bug修复版本。

- [squawk v2.40](https://postgresweekly.com/link/180566/rss) – Postgres迁移和SQL的linter。

- [pgAdmin 4 v9.12](https://postgresweekly.com/link/180567/rss)