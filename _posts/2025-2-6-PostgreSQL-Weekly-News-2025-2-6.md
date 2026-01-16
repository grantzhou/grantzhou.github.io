---
layout: post
title: PostgreSQL 每周新闻 2025-2-6
---
### PostgreSQL每周新闻#587 - 2025年2月6日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/587)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/na8hucfslyi8dzrshv3h.jpg)
## [仅仅因为您进行了索引扫描，并不意味着您不能做得更好](https://postgresweekly.com/link/165372/web)
如果您在查看查询计划时看到索引扫描，您可能会认为自己正走在实现高性能查询的正确道路上，但 Michael 表示，还有更多的潜力可以挖掘。这里有一些有用的提示。

`Michael Christofides`

## [DocumentDB：微软为 Postgres 带来更多 NoSQL](https://postgresweekly.com/link/165373/web)
不要与专有的 Amazon DocumentDB 混淆，这个 DocumentDB 是一个 MIT 许可的基于文档的 NoSQL 引擎，建立在 Postgres 之上，微软在内部将其用于 Azure Cosmos DB for MongoDB。


`Microsoft `
## [POSETTE 2025：征集提案 (CFP) 将于 2 月 9 日截止！](https://postgresweekly.com/link/165371/web)
POSETTE：Postgres 活动，一场免费的虚拟开发者活动，将于 6 月 10 日至 12 日举行。CFP 将于太平洋标准时间 2 月 9 日晚上 11:59 截止。鼓励新手和经验丰富的演讲者提交提案！查看建议主题、演讲者资源和提交详情。


`Microsoft `

### 本周摘要：

* FOSDEM PGDay 2025 于上周举行，Stefanie Janine Stölting [分享了会议的简短片段](https://postgresweekly.com/link/165376/web)，包括一张与真实 Slonik 的合影！🐘

* 📊 [JSONBench](https://postgresweekly.com/link/165377/web) 尝试对不同的数据库（包括 Postgres）进行基准测试，以便大规模处理 JSON。

## [🤖 使用 Claude 自动执行 Postgres 中的数据汇总](https://postgresweekly.com/link/165378/web)
Timescale 展示了如何将 pgvector 与其 pgai 工具结合起来，让 Postgres 无需任何外部脚本即可与 Anthropic 的 Claude AI 联系以执行汇总任务。


`Timescale`
## [commit_delay 以获得更好的性能：Postgres 基准测试](https://postgresweekly.com/link/165380/web)
Laurenz 分享基准测试结果，强调了通过使用 commit_delay 和 commit_siblings 参数对 WAL 刷新进行分组并最终优化事务工作负载所获得的性能提升。


`Laurenz Albe`
## [用 pg_hint_plan 替换 Oracle 提示：最佳实践](https://postgresweekly.com/link/165381/web)
Oracle 数据库用户可以使用“提示”来指导查询优化器的决策过程，并且您可以使用 pg_hint_plan 在 Postgres 中重现该想法。Lukas 解释了何时可以使用提示以及如何将 Oracle 提示映射到 Postgres。

`Lukas Fittl`


* 📄 [使用 pgvector 和 Next.js 构建语义电影搜索演示](https://postgresweekly.com/link/165384/web) - Fatih Altinok

* 📄 [避免 pgBackRest 中的 WAL 档案保留陷阱](https://postgresweekly.com/link/165385/web) - Stefan Fercot

* 📄 [在 Postgres 中索引物化视图](https://postgresweekly.com/link/165386/web) - Elizabeth Christensen

* 📄 [在 Postgres 中调试死锁](https://postgresweekly.com/link/165387/web) - Louis Heath


### 代码和工具：

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/vwe4ezurybqd9ndhwktw.jpg)

## [DB Fiddle：在线 SQL 数据库游乐场](https://postgresweekly.com/link/165388/web)
自从我链接到这个有用的工具以来，已经过去了几年，它在各种在线沙箱中提供了众多数据库系统（包括 Postgres 9.4 到 17 版）。虽然本地数据库对于大型实验来说总是更好的选择，但如果您想在版本之前检查语法更改或快速测试针对旧 Postgres 版本的查询（甚至针对 MySQL），这是一种快速简便的方法。

`Status200`

## [ChartDB：开源数据库架构图编辑器](https://postgresweekly.com/link/165390/web)
从头创建新架构或快速导入现有架构。支持 Postgres、MySQL、SQL Server、SQLite 等，并内置于 TypeScript 中。您可以自行部署它，也可以在此处试用在线演示。AGPL 许可。

`ChartDB Team`

[PeerDB 0.24](https://postgresweekly.com/link/165392/web) – 将数据从 Postgres 流式传输到数据仓库、队列和存储引擎。

[PG Back Web 0.4](https://postgresweekly.com/link/165393/web) – 具有用户友好型 Web 界面的 PostgreSQL 备份。

[🤖 pgai 0.8](https://postgresweekly.com/link/165394/web) – Timescale 的工具，用于在 Postgres 中使用 RAG 和 LLM。