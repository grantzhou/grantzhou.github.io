---
layout: post
title: PostgreSQL 每周新闻 2026-3-11
---
### PostgreSQL每周新闻#639 - 2026年3月11日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/639)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/nluazltiueyof85sqwog.jpg)

## [pg_plan_advice: Postgres 的计划稳定性和用户规划器控制？](https://postgresweekly.com/link/181918/rss)

多产的 Postgres 贡献者/提交者 Robert Haas 为 Postgres 19 提出了一个**雄心勃勃的**补丁集，让管理员能够在系统范围内控制查询规划器行为，无需触碰应用程序代码，通过存储并自动应用"计划建议"字符串到特定查询。

`Robert Haas`


## [在没有生产数据的情况下获取生产查询计划](https://postgresweekly.com/link/181919/rss)

Postgres 18 有两个新函数使优化器统计信息可移植，这意味着可以从生产数据库导出统计信息并将它们注入测试数据库，这样你就可以在本地重现生产查询计划，**而无需**实际数据！

`Radim Marek (boringSQL)`


## [企业级 Postgres，用于 Agentic AI、高可用性等场景](https://postgresweekly.com/link/181920/rss)

pgEdge 为 Agentic AI 和需要高可用性、可靠性和数据主权的企业应用提供开源的 100% Postgres 基础设施。我们使得大规模构建、部署和管理企业级 Postgres 应用变得容易。

`pgEdge` **赞助商**


## [将生产数据库从 Heroku 迁移到 AWS](https://postgresweekly.com/link/181921/rss)

一篇实用的文章，涵盖了将 300GB 数据库从 Heroku 迁移到 RDS 背后的技术。一个有趣的细节是使用临时 EC2 实例作为桥梁，这是必要的，因为 Heroku 的限制意味着 WAL 归档是唯一的出口，而 RDS 无法直接接收物理 WAL 复制。

`Greg Bergé (Argos)`


**简讯：**

- Supabase 为 Pro 用户[添加了日志排放功能](https://postgresweekly.com/link/181922/rss)，这样你就可以将日志发送到自己的日志后端。

- Bruce Momjian [分享了他新演讲的幻灯片](https://postgresweekly.com/link/181923/rss)，**WAL 的奇妙世界**。


## [使用 PgDog 在无服务器环境中修复连接池问题](https://postgresweekly.com/link/181924/rss)

当 Circleback 的无服务器工作负载遇到 PgBouncer 的单线程限制时，部署时的流量高峰导致了连接问题。多线程连接池工具 [PgDog](https://postgresweekly.com/link/181925/rss) 解决了他们的问题。

`Stephen van Son (Circleback)`


## [使用 Rust 和 Postgres 处理一切](https://postgresweekly.com/link/181926/rss)

从多年生产使用中提炼出的实用模式，用于使用 Rust 和 Postgres 构建后端服务，**"这在硬件价格飙升的世界中可能特别有用。"**

`Sylvain Kerkour`


📄 [就用 Postgres（发挥到极致）](https://postgresweekly.com/link/181927/rss) – 想想 Heroku，除了一切都是数据库。`Andrew Nesbitt`

📄 [MySQL 的阴影](https://postgresweekly.com/link/181928/rss) – Bruce 反思 MySQL 漫长而缓慢的衰落。`Bruce Momjian`

📄 [使用 Iceberg 构建高性能 Postgres 时序堆栈](https://postgresweekly.com/link/181929/rss) `Christensen and Slot (Snowflake)`

📄 [ParadeDB 如何在 Postgres 中优化 Top K](https://postgresweekly.com/link/181930/rss) `Ming Ying (ParadeDB)`


## 🛠 代码和工具

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/zwxzi1qjry1ypl5tm60h.jpg)

## [pg_plan_alternatives: 使用 eBPF 追踪查询计划替代方案](https://postgresweekly.com/link/181931/rss)

`EXPLAIN` 显示最终选择的计划，而不是**考虑过的**计划。这个工具使用 eBPF 来监测 Postgres 的优化器，并在规划阶段追踪替代计划和成本估算。缺点是它仅支持 Linux，并且 Postgres 二进制文件需要调试符号，但这仍然是一篇引人入胜的文章。

`Jan Nidzwetzki`


## [使用 `json_schema_validate` 验证 JSON 的结构](https://postgresweekly.com/link/181932/rss)

Andrew 探讨了在数据库级别验证 JSON 的主题，并分享了他的新 [json_schema_validate](https://postgresweekly.com/link/181933/rss) 扩展，该扩展旨在使验证既简单又快速，相比 [pg_jsonschema](https://postgresweekly.com/link/181934/rss) 更具优势。

`Andrew Dunstan (EDB)`


## [pgconsole: 为团队提供的极简自托管 Postgres 编辑器](https://postgresweekly.com/link/181935/rss)

一个吸引人的基于 Web 的 Postgres 编辑器，具有内置访问控制、审计日志和 AI 辅助功能，你可以通过 Docker 快速部署。如果你想看看它的样子，[这里有一个实时演示](https://postgresweekly.com/link/181936/rss)。请注意，它是**源码可用**的，而不是开源的。

`Bytebase`


- [Marten 8.23](https://postgresweekly.com/link/181937/rss) – .NET 库，在 Postgres 之上提供文档数据库和符合 ACID 的事件存储。

- [Databasus 3.19](https://postgresweekly.com/link/181938/rss) – 用于 Postgres、MySQL 和 MongoDB 的自托管备份工具。

- [psql-wire 0.18](https://postgresweekly.com/link/181939/rss) – Postgres 服务器线协议的纯 Go 实现。

- [PgBulkInsert 9.0](https://postgresweekly.com/link/181940/rss) – 使用二进制 [COPY](https://postgresweekly.com/link/181941/rss) 进行高效批量插入的 Java 库。

- [PostgREST 14.6](https://postgresweekly.com/link/181942/rss) – 从 Postgres 数据库提供完全 RESTful API 的服务。