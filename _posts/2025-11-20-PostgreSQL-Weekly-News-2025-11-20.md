---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-11-20
---
### PostgreSQL每周新闻#625 - 2025年11月20日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/625)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/ddacvvudkcpt1aousimk.jpg)
## [RegreSQL：Postgres 查询的回归测试](https://postgresweekly.com/link/177305/web)
深入了解基于 Go 语言的工具，可将 Postgres 本身的回归测试方法套用至 SQL 查询，以验证对查询或模式的变更是否会破坏查询的预期运作方式（例如，是否仍使用正确的索引或扫描类型？）。

`Radim Marek`


## [Agentic Postgres：开发者导向的 AI 就绪型 Postgres](https://postgresweekly.com/link/177304/web)
Tiger Data 的 Agentic Postgres 将原生 Postgres 资料库转换为 AI 原生资料库。您可以建立资料库分支、分配代理内存，并透过 REST 或 CLI 进行查询。它非常适合使用 Claude、Cursor 或自订代理程式建立的 Go 后端。免费试用，无需信用卡。

`Tiger Data`

## [微软推出全新 PostgreSQL 服务：Azure Horizo​​nDB](https://postgresweekly.com/link/177306/web)
Azure 已有 Azure Database for PostgreSQL，但 Horizo​​nDB 提供“更高水平的效能和可扩展性”，支援跨节点最多 3072 个虚拟核心 (vCore)，资料库容量高达 128TB，可满足企业级工作负载的需求。目前该服务处于「早期预览」阶段，估计需要相当的预算。

`Microsoft`

## **本周摘要**

* [Amazon RDS for PostgreSQL 现在支援 Postgres 18](https://postgresweekly.com/link/177308/web)，具体来说是 Postgres 18.1。 [pgcollection](https://postgresweekly.com/link/177309/web) 以及其他常用扩充功能的最新版本也已包含在内。

* 🏴研再读形体形体许​​数许力许​​L重量壳许种种种种记号 Jimmy Angelakos 宣布将于 12 月 11 日在苏格兰爱丁堡举办[第一届 PostgreSQL 聚会](https://postgresweekly.com/link/177310/web)。

* 如果您使用 Docker 的官方 Postgres 映像，在进行[小版本升级时请务必小心](https://postgresweekly.com/link/177311/web)，因为底层 Debian 版本也可能会更新，从而强制资料库进行不必要的排序规则更新。

* [create_pg_super_document](https://postgresweekly.com/link/177312/web) 是一个使用 LLM 为 Postgres 程式码库中的每个符号建立文件的项目。如果您正在开发扩展或深入研究 Postgres 实现，这将非常有用。

* Pavlo Golub 从 Postgres 的角度[回顾了今年的 Google Summer of Code 活动](https://postgresweekly.com/link/177313/web)，以及参与者所做的工作。


## [在 Postgres 中储存产品、价格和订单](https://postgresweekly.com/link/176988/web)
解决在储存产品资讯时因过度乐观的标准化而导致的问题。

`Hans-Jürgen Schönig`


## [PostGIS效能优化：交集谓词和叠加层](https://postgresweekly.com/link/176989/web)
这是一系列关于如何最大限度发挥PostGIS效能的文章中的最新一篇。

`Paul Ramsey`

📄 [MD5 密码支援已弃用，如何更新密码](https://postgresweekly.com/link/177317/web)？ ——这项工作虽然枯燥，但总得有人做。 Dan Langille

📊 [PlanetScale PostgreSQL 与 Hetzner Local Postgres 的比较——当然，两者并不完全可比](https://postgresweekly.com/link/177318/web)。 Muhammad Azeez

📄 [如何在 Python、Django 和 Postgres 中使用 UUIDv7](https://postgresweekly.com/link/177319/web)？ Paolo Melchiorre

## **发布**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/vrzffuhfvpzthygmedjw.jpg)


## [PgManage 1.4：资料库管理 Web 工具](https://postgresweekly.com/link/177320/web)
一个开源的基于 Web 的介面，以 Postgres 为中心，但也支援 MySQL、SQLite 和 Oracle。您可以同时操作多个资料库，检视表格、检视、函数等，检视查询计划，并取得 SQL 自动补全功能以建立查询。

`Command Prompt, Inc.`

## [🌐 Martin 1.0：快速轻量级的 PostGIS、MBtiles 和 PMtiles 切片伺服器](https://postgresweekly.com/link/177321/web)
一个地理空间切片伺服器及工具集，能够从大型 PostGIS 资料库动态产生向量切片，​​并提供来自 PMTiles 和 MBTiles 档案的切片。经过八年的开发，现已发布 v1.0 版本。您可以在其主页上查看演示。

`MapLibre Contributors`


## **📰 分类广告**


停机并非不可避免。了解 pgEdge + CloudNativePG 如何在 Kubernetes 上实现高可用性 Postgres。[了解更多并立即注册](https://postgresweekly.com/link/177324/web)！

🛣️ [《Next.js 之路》](https://postgresweekly.com/link/177325/web)是由 Robin Wieruch 主讲的课程，旨在教授使用 Next.js 15 和 React 19 进行全端 Web 开发。对于准备超越前端的 JavaScript 开发人员来说，这是理想之选。

## [pg_flo：即时串流、转换和路由 Postgres 资料](https://postgresweekly.com/link/177321/web)
提供一系列过滤器和转换功能，可简化在生产资料库和测试资料库等之间移动资料的操作，支援三种模式：复制并串流、仅串流或一次性复制。使用 NATS 和 Postgres 的复制功能。

`Shayon Mukherjee`

## [Spock：逻辑多主 PostgreSQL 复制](https://postgresweekly.com/link/177326/web)

`pgEdge`

[🐶 PgDog 0.1.15](https://postgresweekly.com/link/177327/web) – 为 Postgres 提供水平扩展和自动分片功能。现已支援基于模式的分片。

[PGSync 6.0](https://postgresweekly.com/link/177328/web) – 将 Postgres（现在也支援 MySQL/MariaDB）资料同步到 Elasticsearch/OpenSearch。

[QuestDB 9.2](https://postgresweekly.com/link/177329/web) – 基于 Java 的时序资料库，相容于 Postgres 的 wire 协定。

[PgParty 1.10](https://postgresweekly.com/link/177330/web) – 使用 Active Record（在 Ruby 和 Rails 中）建立和管理 Postgres 分割区。

[River 0.27](https://postgresweekly.com/link/177331/web) – 适用于 Go 的快速可靠的基于 Postgres 的后台任务系统。

[pg-boss 10.4](https://postgresweekly.com/link/177332/web) – 适用于 Node.js 的基于 Postgres 的任务伫列系统。