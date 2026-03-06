---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-2-20
---
### PostgreSQL每周新闻#589 - 2025年2月20日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/589)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/umlwap0o1lqpb2vcpgzp.jpg)
## [怪物硬件时代的 Postgres](https://postgresweekly.com/link/165885/web)
您可能认为您的 M4 Max 速度非常快，但想象一下拥有一个 AMD EPYC，每个插槽有 192 个内核和 10 TB 的 RAM，其基准测试速度比 15 年前的 Xeon 服务器快 160 倍！现代 CPU 能力（更不用说更快的存储）让我们不禁要问，在现代，我们如何扩展数据库服务器。

`Lætitia Avrot`

## [PostgreSQL 17.3、16.7、15.11、14.16 和 13.19 已发布](https://postgresweekly.com/link/165886/web)
对所有维护的 Postgres 系列进行了一系列更新，以解决一个安全漏洞和许多较小的错误。作为小更新，升级过程很简单，不需要任何转储和重新加载。


`PostgreSQL Global Development Group `
## [Postgres，现在具有内置仓库功能](https://postgresweekly.com/link/165884/web)
一个数据库就可以完成所有工作，为什么要管理两个数据库？Crunchy Data Warehouse 可让您的事务数据库平稳运行，同时添加仓库功能，如查询对象存储、BI 工具连接等。使用您信赖的 Postgres 高效扩展，无需担心复杂性。


`Crunchy Data `
## [PostgreSQL 兼容性指数用于比较实现](https://postgresweekly.com/link/165887/web)
Postgres 发现自己处于一种令人羡慕但又复杂的境地，即成为数据库中的通用语言，其中完全不包含 Postgres 代码的数据库试图以各种方式与其“兼容”。但兼容程度如何？Postgres 兼容性指数是一种测试和监控众多方面的尝试。


`Mayur `
## [看看 Postgres 18 中的虚拟生成列](https://postgresweekly.com/link/165888/web)
Postgres 18 正在获得“虚拟生成列”的能力，其中虚拟列的表达式是在读取时计算的，因此它们不会像当前所有生成的列那样存储在磁盘上。


`Daniel Westermann `

### 本周摘要：

* 🔒 研究人员称，去年 12 月，[psql 中的一个漏洞被用来入侵美国财政部](https://postgresweekly.com/link/165890/web)。

* 📕 [《面向数据专业人士的 PostgreSQL 简介》](https://postgresweekly.com/link/165891/web)是 Ryan Booz 和 Grant Fritchey 的新书，由 Redgate 出版。该书可在“填写您的详细信息”墙后面免费获取。

* 🇪🇺 PostgreSQL Europe 已决定退出 Twitter/X，但在此分享了其[替代社交媒体渠道列表](https://postgresweekly.com/link/165892/web)，以及他们组织的所有会议。此外，您知道 [PostgreSQL Europe 有一个多元化工作组吗](https://postgresweekly.com/link/165893/web)？Karen Jex 对此进行了详细介绍。

* [ClickPipes 的 Postgres CDC 连接器现已公开测试](https://postgresweekly.com/link/165894/web)。


## [在 Postgres 中表示图形](https://postgresweekly.com/link/165895/web)
Postgres 不是图形数据库，但您可以模拟所涉及的概念。或者，如果您需要类似 Cypher 的图形查询支持，则可以使用 Apache AGE 之类的扩展。


`Richard Towers`
## [从 Postgres 到 Parquet 的增量归档](https://postgresweekly.com/link/165897/web)
Crunchy Data 的 pg_parquet 和 pg_incremental 扩展可用于设置可靠的管道，将行范围导出为 S3 上的列式 Parquet 格式。


`Marco Slot`


* 📄 等待 Postgres 18：[为 VACUUM/ANALYZE（VERBOSE）和 Autovacuum 日志添加延迟时间](https://postgresweekly.com/link/165898/web) - Hubert depesz Lubaczewski

* 📄 [Cloudflare、Unikernels 和 Bare Metal：Prisma Postgres 查询的生命周期](https://postgresweekly.com/link/165899/web) - Nikolas Burk (Prisma)

* 📄 [需要了解的重要 Postgres 配置参数](https://postgresweekly.com/link/165900/web) Semab Tariq


### 代码和工具：

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/ufgvhucqem3c5ibe7sla.jpg)

## [扩展 pgai Vectorizer](https://postgresweekly.com/link/165901/web)
pgai 是 Timescale 的工具套件，可让您更轻松地使用 Postgres 的 AI 功能，包括自动创建和同步数据的向量嵌入。现在，他们通过 SQLAlchemy 支持和通过 LiteLLM 支持更多嵌入模型（更多详细信息请点击此处）提高了标准。

`Timescale`

[dynamodb_fdw 1.4](https://postgresweekly.com/link/165903/web) – DynamoDB Foreign Data Wrapper for Postgres. Now supporting Postgres 17.

[Stateless Postgres Query Router (SPQR) 2.4](https://postgresweekly.com/link/165904/web) – An approach to horizontal sharding, originally built at Yandex Cloud.

[River 0.17](https://postgresweekly.com/link/165905/web) – Fast and reliable Postgres-powered background jobs for Go.

[📊 pgwatch v3.1.0](https://postgresweekly.com/link/165906/web) – Postgres metrics monitor/dashboard.

[Prisma 6.4](https://postgresweekly.com/link/165907/web) – Popular ORM for Node.js and TypeScript.