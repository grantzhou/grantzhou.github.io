---
layout: post
title: PostgreSQL 每周新闻 2024-7-24
---
### PostgreSQL每周新闻#564 - 2024年7月24日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/564)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/a9erkdqglxbpiucfetlk.jpg)
## [psql 的魔术技巧：设置、预设、回显和已保存的查询](https://postgresweekly.com/link/157910/web)
“我想分享一些最喜欢的东西，它们可以让你更好地使用 Postgres。如果你刚刚开始使用 psql，或者还没有尝试太多默认设置，那么这篇文章适合你。”


`ELIZABETH CHRISTENSEN `

## [▶ PGConf.dev 2024 的所有演讲](https://postgresweekly.com/link/157911/web)
如果您没有参加 5 月份在加拿大举行的 [PGConf.dev](https://postgresweekly.com/link/157912/web) 会议，那么您现在至少可以了解舞台上发生的一切，包括有关[自动清理出错](https://postgresweekly.com/link/157913/web)、[PB 级部署](https://postgresweekly.com/link/157914/web)、[Amazon RDS 如何扩展](https://postgresweekly.com/link/157915/web)以及[如何让您的 Postgres 博客文章产生更大影响](https://postgresweekly.com/link/157916/web)的演讲。


`POSTGRESQL DEVELOPMENT CONFERENCE `
## [Render 是您最快的生产途径](https://postgresweekly.com/link/157909/web)
无论您的堆栈是什么，您都可以轻松构建、快速部署、更新和自信地扩展您的应用，从第一个用户到第十亿个用户。开始免费使用 Render 进行构建 — 面向开发人员的现代云。


`RENDER `
## [加快 Postgres 中的索引创建速度](https://postgresweekly.com/link/157917/web)
索引对于最大限度地提高查询性能至关重要，但在大型数据集上创建新索引可能需要很长时间。Hans-Jürgen 正在研究一种显著加快该过程的方法。


`HANS-JÜRGEN SCHÖNIG `
## [你说的很有道理！](https://postgresweekly.com/link/157918/web)
Postgres SAVEPOINT — 你知道吗，在事务中可以定义事务剩余部分可以回滚到的点？它们被称为SAVEPOINT。


`ANDREW ATKINSON `

### 本周摘要：

* 更正：上周，我们错误地说 PostgreSQL 全球开发小组拥有 PostgreSQL 商标，但 Jonathan Katz 善意提醒我们，它实际上是由加拿大 PostgreSQL 社区协会拥有的。这确实是一个愚蠢的错误，因为我们在每期杂志的页脚中都包含了这些信息！🫢

* 但是，关于商标的话题，如果您想了解有关 Postgres 商标的更多信息，[有一个官方页面专门介绍这一点](https://postgresweekly.com/link/157920/web)。

* 🤖 在 X/Twitter 上，快速了解一下 [Facebook 的新 Llama 3.1 模型在针对 Postgres 的文本到 SQL 任务中的表现](https://postgresweekly.com/link/157940/web_。

## [将行模式识别引入 Postgres](https://postgresweekly.com/link/157921/web)
SQL 标准包括基于定义的模式搜索表中行序列的功能。Tatsuo 也希望将其引入 Postgres。他向我们展示了它的工作原理和他的工作进展。


`TATSUO ISHII `
## [Postgres 与 Pinecone 在矢量存储和查询方面的比较](https://postgresweekly.com/link/157922/web)
对 Pinecone 最近的一篇文章的回应，该文章比较了 Pinecone 和 Postgres 在矢量搜索任务方面的比较。


`NAREK GALSTYAN `

### 机密：

通过 [Redgate 101 网络研讨会[(https://postgresweekly.com/link/157924/web)系列提升您的 PostgreSQL 技能，该系列由专家主持，简单易懂。这是简化版的 PostgreSQL。


🐿️ Go 开发人员？我们有一份时事通讯！查看我们的姊妹时事通讯之一 [Golang Weekly](https://postgresweekly.com/link/157941/web)。


## [寻找 Postgres 面临分区时的隐藏障碍](https://postgresweekly.com/link/157925/web)
Andrei 遇到了一个奇怪的情况，对表进行分区会引发一些棘手的性能问题。


`ANDREI LEPIKHOV`
## [哪些云提供商支持 auto_explain？](https://postgresweekly.com/link/157926/web)
auto_explain 是一个 Postgres 模块，用于自动记录慢查询的执行计划，但并非每个云平台都支持它。


`MICHAEL CHRISTOFIDES`

📄 [为自己和为他人运行 Postgres 之间的区别](https://postgresweekly.com/link/157928/web)——毫不奇怪，构建平台与为自己启动数据库服务器完全是两码事 - BURAK YUCESOY

📄 [高级 Postgres 性能调优和监控方法](https://postgresweekly.com/link/157929/web)——您可能采用的工具和技术列表 - NIALL OHIGGINS

📄 在 Node.js 中使用[行级安全性](https://postgresweekly.com/link/157930/web) - KRISTIAN DUPONT



### 🛠 代码和工具
## [PLV8ify：将 JavaScript 文件转换为 PLV8 函数](https://postgresweekly.com/link/157931/web)
捆绑 TS/JS 输入并使用 PLV8 扩展（允许在 Postgres 中使用 JavaScript 作为过程语言）编写包含 Postgres 函数的 SQL。


`DIVYENDU SINGH`

[ActiveRecordExtended 3.3](https://postgresweekly.com/link/157933/web) – 为 ActiveRecord / Ruby on Rails 应用程序添加额外的 Postgres 功能。

[无状态 Postgres 查询路由器 (SPQR) 1.5](https://postgresweekly.com/link/157934/web) – 一种水平分片方法，最初在 Yandex Cloud 上构建。（GitHub repo）

[River 0.10](https://postgresweekly.com/link/157936/web) – 适用于 Go 的快速可靠的 Postgres 后台作业。

[Piccolo 1.14](https://postgresweekly.com/link/157937/web) – 用户友好的 Python ORM 和查询生成器。

[PGSync 3.2](https://postgresweekly.com/link/157938/web) – Postgres 到 Elasticsearch/OpenSearch 同步。

[Mikro ORM 6.3](https://postgresweekly.com/link/157939/web) – 适用于 Node.js 的 TypeScript ORM。