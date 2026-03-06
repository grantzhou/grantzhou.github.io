---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-9-18
---
### PostgreSQL每周新闻#616 - 2025年9月18日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/616)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/s9qtubbavnoqyklkrzoh.jpg)
## [「数据库不接受指令」：现在该怎么办？](https://postgresweekly.com/link/174454/web)
这个错误你肯定不想遇到，因为这意味著你需要做一些认真的工作来避免交易 ID 重叠。不过，如果你真的遇到了，Laurenz 会提醒我们该怎么做，以及一些需要避免的「低阶措施」。

`Laurenz Albe`

## [亲身体验 Postgres 18：异步 I/O、B 树跳过扫描等](https://postgresweekly.com/link/174453/web)
Postgres 18 将于本月发布，现在是时候了解其以性能为中心的更新了：从异步 I/O 和计划器更改，到 B 树跳过扫描、UUIDv7、VACUUM 更改以及对生产工作负载的增强监控。

`pganalyze  `

## [核心 Postgres 资料库分片（零停机）](https://postgresweekly.com/link/174104/web)
Gadget 是一个线上 JavaScript 开发平台，它将所有内容都保存在一个大型 Postgres 实例中，但最终达到了垂直扩展的极限。以下是他们如何在零停机或零请求的情况下对资料库进行分片的方法。 “分片的意义在于‘硬’！”

`Harry Brundage (Gadget) `


### **本周摘要**

* 🇺🇸 [PGConf NYC ](https://postgresweekly.com/link/174456/web)将于本月稍后在纽约举行，目前仍有门票出售。

* 您能在 Postgres 中储存世界上已知最古老的金融交易日期吗？[事实证明可以](https://postgresweekly.com/link/174457/web)。

* 如果您使用的是 Debian 12 系统，并且在 US/* 时区下运行 Postgres，[那么在升级到 Debian 13 之前，请注意以下几点](https://postgresweekly.com/link/174480/web)。


## [Postgres 逻辑复制的演变：历史概述](https://postgresweekly.com/link/174458/web)
简要介绍过去 20 年采用的方法。多年来，Petr 参与了许多与逻辑复制相关的专案（并在 PostgresOpen 2016 上发表了关于 Postgres 复制的演讲），因此这是一个可靠的观点。


`Petr Jelinek`

## [无需超级使用者的 Postgres 维护](https://postgresweekly.com/link/174460/web)
查看内建的、预先定义的管理角色，这些角色可让您执行许多维护任务而无需超级使用者存取权限。


`Radim Marek`

## [Postgres 18 令人兴奋](https://postgresweekly.com/link/174458/web)
距离 Postgres 18 最终版本发布还有一周时间，但已经有很多值得兴奋的地方，尤其是异步 I/O 的引入，它将为我们许多人带来性能提升。


`Elizabeth Christensen（Crunchy Data）`

📊 [Cyber​​tec PostgreSQL 企业版 (PGEE) 中 TDE 和校验和的成本](https://postgresweekly.com/link/174463/web)——透明数据加密对效能的影响如此之小，我感到很惊喜。 Christoph Berg

📄 [如何在 Go 和 Postgres 中实作寄件匣模式](https://postgresweekly.com/link/174464/web)－一种确保讯息最终到达指定目的地的弹性方法。 Alex Pliutau

📄 [使用 CloudNativePG 让 Postgres 缩放至零](https://postgresweekly.com/link/174465/web) Esther Minano Sanz (Xata)

📺 [使用 PGlite 将 Postgres 编译为 WebAssembly](https://postgresweekly.com/link/174466/web)——30 分钟演讲。 Sam Willis

## 📰 分类广告

🏁 [扩展毫秒速度](https://postgresweekly.com/link/174467/web)。 Redis 8.2 已实现每秒 100 万次以上操作。[免费部署](https://postgresweekly.com/link/174467/web)并在您自己的技术堆叠中进行压力测试。

💌 您知道我们有一系列新闻简报吗？看看 [JavaScript Weekly](https://postgresweekly.com/link/174468/web)、[Go Weekly](https://postgresweekly.com/link/174469/web) 和 [Ruby Weekly](https://postgresweekly.com/link/174470/web)，更全面地了解我们的工作。


## **发布**

## [pgsql_tweaks 1.0.0 发布](https://postgresweekly.com/link/173459/web)
这是作者作为 Postgres 用户在日常工作中使用的一套函数和视图，涵盖检查数据类型、收集统计数据、WAL 监控、查找未使用的索引以及转换函数等领域。官方主页上有每个功能的文件。

`Stefanie Janine Stölting`

## [pgstream：Postgres 复制与 DDL 变更](https://postgresweekly.com/link/174124/web)
一个基于 Go 的变更资料撷取 (CDC) 命令列工具和函式库，支援 Postgres 复制，并支援对其他 Postgres 资料库、Elasticsearch/OpenSearch 或 Webhook 等目标的 DDL 变更。更多资讯请参阅这篇文章。

`Xata`

🌐 [osm2pgsql 2.2](https://postgresweekly.com/link/174475/web) – 将 OpenStreetMap 资料汇入 Postgres/PostGIS 资料库。

[无状态 Postgres 查询路由器 (SPQR) 2.7 ](https://postgresweekly.com/link/174476/web)– 一种水平分片方法，最初由 Yandex Cloud 建构。

[VectorChord 0.5.2](https://postgresweekly.com/link/174477/web) – Postgres 中可扩充、快速且磁碟友善的向量搜寻。

[River 0.25](https://postgresweekly.com/link/174478/web) – 适用于 Go 应用的强大 Postgres 驱动的作业处理系统。

[pgwatch v4 Beta 版](https://postgresweekly.com/link/174479/web)