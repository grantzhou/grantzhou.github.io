---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-1-30
---
### PostgreSQL每周新闻#586 - 2025年1月30日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/586)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/utglhkoflyljfsouu4xb.jpg)
## [停机时间的 Aurora Postgres 重大升级](https://postgresweekly.com/link/165033/web)
受到 Lyft 数据库团队早期博客文章的启发，两位工程师着手升级他们规模虽小但使用率很高的 Aurora Postgres 实例，而不会影响他们的应用程序 — 以下是完整的故事以及遇到的问题。（请注意，数据库确实会停机几秒钟，但他们的应用程序不需要丢弃任何请求。）

`Parunashvili and Woelfel`

## [用于全文搜索的全新 Postgres 块存储布局](https://postgresweekly.com/link/165035/web)
pg_search 是 Postgres 扩展，提供 BM25 驱动的全文搜索，但到目前为止仍需要使用外部非 Postgres 文件。现在不再需要了。它现在完全使用 Postgres 块存储 — 原因和方法如下。


`Ming Ying (ParadeDB) `
## [PostgreSQL 性能监控备忘单](https://postgresweekly.com/link/165032/web)
使用我们方便的备忘单开始跟踪 PostgreSQL 数据库中的重要资源和活动指标。您将获得有用的 psql 命令，并获得使用 Datadog 监控 PostgreSQL 性能的快速入门指南。


`Datadog  `

### 本周摘要：

* PostgreSQL 项目再次参与 Google Summer of Code。[Pavlo Golub 分享了一些参与方式的信息](https://postgresweekly.com/link/165037/web)。

* 🤖 Bruce Momjian 分享了他最新演讲的 [PDF 幻灯片 📄 AI 战壕中的数据库](https://postgresweekly.com/link/165038/web)。它涵盖了向量、文本嵌入、语义搜索、转换器、检索增强生成 (RAG) 等。

* PostgreSQL 贡献者团队公布了 [24 位新成员](https://postgresweekly.com/link/165039/web)，他们因在 Postgres 社区和代码库中的工作而受到认可。

* 🎤 Postgres 贡献者 [Daniel Gustafsson 在 Talking Postgres 播客上讨论了他是如何进入编程领域的](https://postgresweekly.com/link/165040/web)，尤其是 Postgres。

* 🇩🇪 [德国 PostgreSQL 会议的 CFP](https://postgresweekly.com/link/165041/web)（今年 5 月在柏林举行）将于本周六结束，如果您想发言，请立即提交您的提案。

* [Tembo Cloud 现在支持 Postgres 17](https://postgresweekly.com/link/165043/web)。


## [Postgres 中的登录触发器](https://postgresweekly.com/link/165044/web)
在 Postgres 17 中，您可以创建一个在登录时发生的触发器，您可以使用它来审计甚至以创造性的方式保护数据库。


`Hans-Jürgen Schönig `
## [VACUUM（INDEX_CLEANUP OFF）被认为有害](https://postgresweekly.com/link/165046/web)
“除非您确定自己知道自己在做什么（即您处于环绕点紧急情况），否则请假装此选项不存在。真的。”


`Christophe Pettus `


* 📄 [分区表索引灾难](https://postgresweekly.com/link/165047/web)——如果您曾经遇到过索引命名冲突，那么这篇文章可能会引起您的兴趣 - Henrietta Dombrovskaya

* 📄 [等待 Postgres 18：允许更改 autovacuum_max_workers 而无需重新启动](https://postgresweekly.com/link/165048/web) -  Hubert depesz Lubaczewski


### 📰 分类广告
[在 pganalyze 中引入查询调优工作簿](https://postgresweekly.com/link/165049/web)！安全地对生产中的 Postgres 查询进行基准测试、实验和优化。

🐘 [POSETTE：Postgres 活动将于 6 月 10 日至 12 日举行](https://postgresweekly.com/link/165050/web)。[征集提案](https://postgresweekly.com/link/165050/web)截止日期为 2 月 9 日。鼓励新手和经验丰富的演讲者提交提案！


### 代码和工具：

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/dgzt4x65ox9vqxub1ujl.jpg)

## [Mathesar：Postgres 数据库的电子表格界面](https://postgresweekly.com/link/165051/web)
一个开源 (GPLv3) 工具，为您选择的 Postgres 数据库提供表格样式的界面，旨在使开发人员能够更直接地向最终用户开放数据库。我们两年前首次链接到它，但 v0.2 刚刚发布。GitHub 存储库。

`Mathesar`

## [pgwatch 3.0：灵活的 Postgres 监控解决方案](https://postgresweekly.com/link/165053/web)
v3.0 增加了对 Postgres 17 的支持（包括新指标）、Windows 支持、改进的 Docker 支持、更新的文档、对并行接收器的支持等。GitHub repo。
`CYBERTEC`

## [pg_squeeze 1.8：自动表膨胀清理的扩展](https://postgresweekly.com/link/165056/web)
虽然不能替代清理，但此扩展更进一步，获得了更多的空间改进，现在支持 Postgres 17。

`CYBERTEC`