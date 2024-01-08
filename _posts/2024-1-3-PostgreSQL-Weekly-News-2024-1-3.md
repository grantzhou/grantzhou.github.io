---
layout: post
title: PostgreSQL 每周新闻 2024-1-3
---
### PostgreSQL每周新闻#536 - 2024年1月3日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/536)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/stx2bxlakxud60tkwb97.jpg)
## [1. 📗《PostgreSQL 14 内部原理》一书](https://postgresweekly.com/link/149394/web)
一本关于 Postgres 14 的书成为 2023 年最受欢迎的链接，这似乎很奇怪，但它是经过长期开发后完成的，与更现代的 Postgres 版本仍然高度相关，并且可用 作为免费的 PDF。 它的 600 多页内容非常深入，并且包含代码驱动的示例和图表，使您可以轻松缩小范围到您感兴趣的主题，例如锁、索引和查询处理。


`Egor Rogov and Liudmila Mantrova `
## [2：使用 Postgres 出错的九种方法](https://postgresweekly.com/link/149395/web)
快速浏览您可能遇到的一些常见错误和陷阱，从过度使用触发器到不向外键添加索引等。


`Phil Booth `
## [使用 AI 自动优化您的 RDS 或 Aurora Postgres 数据库](https://postgresweekly.com/link/149393/web)
需要帮助优化 Postgres 旋钮、查询、索引和 autovacuum？ OtterTune 是您的人工智能数据库副驾驶，可以提高性能、降低成本并保持数据库健康。 获得三个数据库的 30 天免费试用。


`OtterTune `
## [3：向量是 Postgres 中的新 JSON](https://postgresweekly.com/link/149396/web)
Jonathan 的断言在 2024 年只会比 2023 年 6 月变得更加真实。机器学习和 LLM 嵌入使向量成为流行的数据结构，Postgres 对它们的支持逐月增长 （尽管目前主要是通过扩展的方式，例如 pgvector）。


`Jonathan Katz `
## [4：152 个 psql 小技巧](https://postgresweekly.com/link/149397/web)
为久经考验的 psql 客户端提供的长期流行的小技巧。 如果您很快就会有一个 psql 会话，那么值得浏览一下，因为从长远来看，您可能会节省更多时间。 也可以加载单个提示并随机跳转。


`Lætitia Avrot `
## [5：Postgres JSONB 备忘单](https://postgresweekly.com/link/149399/web)
Postgres 中各种 JSON 函数的便捷备忘单，其中包含每个函数的快速示例以及相关运算符。 这是 PDF 的直接链接。


`Aiven `


## 📺 **热门视频**

* [MERGE 命令](https://postgresweekly.com/link/149401/web) - Simon Riggs
* [一起保护 PostgreSQL 免受外部攻击](https://postgresweekly.com/link/149402/web) - Bruce Momjian
* [ACID 里的 I](https://postgresweekly.com/link/149403/web) - Lætitia Avrot
* [实施 Postgres 补丁的演练](https://postgresweekly.com/link/149404/web) - Andrey Borodin
* [Postgres 现在可以做什么](https://postgresweekly.com/link/149405/web) - Vagmi Mudumbai.


## **代码和工具**

## [1：最值得了解的 8 个 Postgres 扩展](https://postgresweekly.com/link/149407/web)
Timescale 的工程师分享了他们使用的、令人兴奋的一系列扩展。 也许我们有点作弊，但这篇综述确实获得了与工具相关的帖子最多的点击次数;-)


`SEWRATHAN AND CLARK (TIMESCALE) `
## [2. PGMQ：基于 Postgres 构建的简单消息队列](https://postgresweekly.com/link/149408/web)
想象一下 AWS SQS，但在 Postgres 数据库中运行。 PGMQ 是用 Rust 编写的，并提供具有可见性超时的“仅一次”传递语义。


`ADAM HENDEL (TEMBO) `
## [3：pgroll：零停机、可逆架构迁移](https://postgresweekly.com/link/149409/web)
Xata 的人员认为数据库迁移应该是简单、无风险且可逆的，因此他们构建了一个工具来实现这一点。 pgroll 包含多种方法，例如使用“扩展和收缩”模式将迁移拆分为多个可逆块，以及仅在短锁定（带超时）下执行操作。


`CARLOS PÉREZ-ARADROS HERCE (XATA) `
## [4：Mathesar：电子表格数据库接口](https://postgresweekly.com/link/149410/web)
一种开源 (GPL) 工具，为您选择的 Postgres 数据库提供网格样式接口，目的是使开发人员能够更直接地向最终用户开放数据库。 它是用 Python 编写的，也位于 GitHub 上。


`MATHESAR `
## [5：PL/Rust 1.0：用 Rust 编写 Postgres 函数](https://postgresweekly.com/link/149412/web)
这是一个令人兴奋的项目的重大发布，该项目将 Rust 编译为本机机器代码，然后作为 Postgres 中的函数运行。 这保证了类似扩展的性能水平，但形式更加动态。 1.2.7是最新版本。 我们预计到 2024 年，Rust 在构建 Postgres 扩展方面的使用将进一步飙升。


`TECHNOLOGY CONCEPTS AND DESIGN, INC. `
## [6：pg_bm25：Postgres 内部的弹性质量全文搜索](https://postgresweekly.com/link/149414/web)
如果您遇到 Postgres 内置全文搜索的任何限制，这是一个基于 Rust 的扩展，引入了 BM25 索引类型，据称“索引速度快了 50 秒” 比 tsvector 并且对结果进行排名快 20 倍。”


`PARADEDB `