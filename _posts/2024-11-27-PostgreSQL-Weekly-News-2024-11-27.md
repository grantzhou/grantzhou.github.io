---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-11-27
---
### PostgreSQL每周新闻#579 - 2024年11月27日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/579)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/zwhhglr0pcibnek7umhs.jpg)
## [pgspot：发现 Postgres 扩展脚本中的漏洞](https://postgresweekly.com/link/162748/web)
一种用于检查漏洞和最佳实践的 SQL 脚本安全分析工具。它由 Timescale 工程师创建，旨在防止 TimescaleDB 中发现的漏洞再次出现，它已经导致发现与扩展相关的漏洞，Postgres 核心团队已修复该漏洞。

`Sven Klemm (Timescale)`
## [GROUP BY 子句重新排序能否提高性能？](https://postgresweekly.com/link/162750/web)
重新排序 GROUP BY 中的列能否显著提高查询性能？查询结构的微小变化确实可以带来巨大的收益。


`Andrei Lepikhov `
## [在 Postgres 上构建 AI 应用程序？从 pgai 开始](https://postgresweekly.com/link/162747/web)
pgai 是 PostgreSQL 的扩展，它为 PostgreSQL 带来了更多 AI 工作流，例如嵌入创建和模型完成。pgai 为开发人员提供 AI 超能力，使他们更容易构建搜索和检索增强生成 (RAG) 应用程序。


`Timescale `
## [使用 INSERT 与 COPY 对批量提取进行基准测试](https://postgresweekly.com/link/162751/web)
将数据批量加载到 Postgres 中的两种最简单方法是使用 INSERT 和 COPY。James 解释了它们各自的优点，对两种方法的多种配置进行了基准测试，并指导了在某些情况下应使用哪种方法。


`James Blackwood-Sewell`

### 本周摘要：

紧随我们上周提到的[有点小问题的 Postgres 版本](https://postgresweekly.com/link/162752/web)之后，[Postgres 17.2、16.6、15.10、14.15、13.18 和 12.22](https://postgresweekly.com/link/162753/web) 现已全部发布。

🦋 如果您是 Bluesky 社交网络的用户，Craig Kerstiens 整理了一个[ ]Postgres 人员“入门包”](https://postgresweekly.com/link/162754/web)，您可以关注。

Amazon Aurora Serverless 2 现在支持[缩减到零容量](https://postgresweekly.com/link/162755/web)。对于容量小或间歇使用的数据库来说，这可能是一笔巨大的节省。


## [为什么 Postgres 主版本升级很难](https://postgresweekly.com/link/162756/web) 
更新二进制文件并重新启动？不，不，不。对底层数据格式的调整和更新需要更结构化的方法 — Peter 解释了原因。


`Peter Eisentraut`
## [▶ PGConf.EU 2024 闪电演讲](https://postgresweekly.com/link/162757/web) 
最近 PGConf EU 活动上 12 场简短演讲的汇总，以及幻灯片和录音的链接。涵盖的主题包括 BM25、Postgres Performance Farm 的更新、pg_duckdb 和 WAL-G。


`Andreas 'ads' Scherbaum`
## [删除操作很困难](https://postgresweekly.com/link/162758/web) 
从概念上讲，从表中删除数据很容易理解。但在实践中，这需要大量的幕后工作，而且性能问题很快就会出现。


`Radim Marek`

📄 [在 SQL 脚本中替换变量](https://postgresweekly.com/link/162759/web) - 例如使用 psql 调用它们时 - Florent Jardin

📄 [使用临时数据库测试 Go 和 Postgres](https://postgresweekly.com/link/162760/web) - Michael Stapelberg

📄 [理解和减少复制延迟](https://postgresweekly.com/link/162761/web) - Ibrar Ahmed

📄 [快速交谈：各种排序规则的速度](https://postgresweekly.com/link/162762/web) - Christophe Pettus


### 🛠 代码和工具

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/okcq9ffd5urluy9olmbc.jpg)

## [Pigsty v3.1：一款“内置电池”的 Postgres 发行版](https://postgresweekly.com/link/162763/web)
Pigsty 是 Postgres 的打包版本，其中包含各种扩展和工具，可在您自己的机器上提供类似 RDS 的体验。v3.1 引入了 Postgres 17 作为默认版本，并包含一种快速启动自托管 Supabase 实例的方法。


`Ruohang Feng`
## [💎 pg_query 6.0：使用 Postgres 自己的解析器解析、反解析和规范化 SQL 查询的 Ruby 库](https://postgresweekly.com/link/162766/web)
使用实际的 Postgres 服务器源来解析 SQL 查询并返回其内部 Postgres 解析树。v6.0 升级为使用 Postgres 17 解析器及其支持的新功能（例如新的 JSON 函数）。

`pganalyze`

[Bytebase 3.1](https://postgresweekly.com/link/162799/web) – 面向团队的数据库 CI/CD 和操作工具。

[pg_partman 5.2](https://postgresweekly.com/link/162800/web) – 分区管理扩展。