---
layout: post
title: PostgreSQL 每周新闻 2022-12-21
---
### PostgreSQL每周新闻#485 - 2022年12月14日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/486)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/v1671539436/zmiwjsscjhodpe461fzf.jpg)

## 2022年最佳 Postgres 周刊
这是今年的最后一期（我们将于 2023 年 1 月 4 日回归），因此我们将重新审视 2022 年最受欢迎的那些文章。我们已经涵盖了主要的热门文章，但也对其他内容进行了一些细分（例如视频). 我们希望您有一个美妙的假期。

___

`Peter Cooper，您的编辑`

## 1：[😱 一个毛茸茸的 Postgres 事件](https://ardentperf.com/2022/02/10/a-hairy-postgresql-incident/)
一个升级到 Postgres 11 的团队，他们的应用程序开始遇到问题。作者以一种相当重要的方式来拯救。这是一个解决问题的奇妙故事，也是一个例子，说明看似简单的问题可以变得多么复杂，或者正如一位评论者所说： “写得非常非常有趣。故事讲述也很棒。”

`JEREMY SCHNEIDER`

## 2: [Postgres 15，10亿事务之后](https://kmoppel.github.io/2022-11-09-postgres-v15-a-billion-transactions-later/)
作者通过 10 亿次事务压力测试将 Postgres 10 与 Postgres 15 进行对比，并进行了一些观察，包括 v15 改进的存储效率。

`KAAREL MOPPEL `

> [**10 月发布的 Postgres 15**](https://www.postgresql.org/about/news/postgresql-15-released-2526/)可以说是今年最大的 Postgres 新闻，但发布公告往往不是我们最受欢迎的链接:-)

> **在 Datadog 中使用上下文可视化关键 PostgreSQL 性能指标**
> 通过精细的 Postgres 分析以及堆栈的其余部分快速识别运行缓慢的查询、瓶颈和错误，以解决性能问题。构建自定义的拖放式仪表板，以快速查看任何 Postgres 指标的分析。
> 
> `DATADOG *赞助商*`

## 3：[Postgres 15 的MERGE功能](https://www.postgresql.org/docs/devel/sql-merge.html)
在 Postgres 文档中看到一个全新的页面总是好的，10 月份我们得到了一个 Postgres 15 的新功能MERGE（您可能在 SQL Server 或 Oracle 中看到过的 SQL 语句）支持。
基本思想是来自查询或源表的数据可以在可定义的条件下一起合并到目标表中。

`POSTGRESQL 文档`

## 4：[Postgres 如何选择用于查询的索引](https://pganalyze.com/blog/how-postgres-chooses-index)
4月1日的发布日期起初让我们担心，但事实证明 Lukas 在直接查看 Postgres 的查询计划器如何开始工作时并不是在开玩笑。
它直接深入到 Postgres 的源代码，但也包括一个实际示例，说明为什么这是有用的知识

`LUKAS FITTL `

## 5：[在 Postgres 中获取查询“进度条” ](https://www.brianlikespostgres.com/postgres-query-progress-bar.htmlb)
这是我们今年链接的所有帖子中最喜欢的标题图，最终结果也很整洁。这个想法是使用序列作为一种计数器来跟踪查询的进度。这有点hack，但你会在这里学到一些东西

`BRIAN 喜欢 POSTGRES`

## 6：[Retool 如何将其 4TB Postgres 数据库升级到 v13](https://retool.com/blog/how-we-upgraded-postgresql-database/)
4TB 可能不是“大数据”，但它处于 SaaS 主数据库大小的通用范围，因此在从 Postgres 9.6 升级到 13 的过程中，你对Retool的故事和技巧可能会有兴趣。

`PETER JOHNSTON (RETOOL)`

## 7：[“我们如何将 Postgres 查询优化 100 倍”](https://towardsdatascience.com/how-we-optimized-postgresql-queries-100x-ff52555eabe)
当谈到 Postgres 查询优化时，“兔子洞很深”，Vadim 说，他遇到了一些非常具体的痛点。
这是对他如何解决一些性能问题并获得一些相当轻松的胜利的很好的了解。

`VADIM MARKOVTSEV`

## 📺 Top Videos of 2022
* Sehrope Sarkuni - [**高级 Postgres 架构设计**](https://www.youtube.com/watch?v=lkWiyEe2RUQ)。
* Andres Freund - [**PostgreSQL 中的 IO: 过去、现在和未来 **](https://www.youtube.com/watch?v=3Oj7fBAqVTw)。
* Jimmy Angelakos - [**慢下来才会比较快**](https://www.youtube.com/watch?v=YvUTsl0isyc) 。
* Robert Treat - [**从INT到BIGINT的高级转换**](https://www.youtube.com/watch?v=qYIVyoZkhCo)。
* Magnus Hagander - [**PostgreSQL - 相关性比以往任何时候都高**](https://www.youtube.com/watch?v=rz6XvfqNa7Q)。

## 🛠 2022 年顶级代码和工具
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/drrysvatyyxrwiv2hims.jpg)

## 1：[pg_activity 3.0：类似htop的活动监控工具](https://github.com/dalibo/pg_activity)
就像您可能使用 top 或 htop 来监控进程和 CPU 使用率一样，pg_activity让您在 Postgres 的幕后看到类似的视图，查看正在运行的查询、最新的性能统计信息等.

`dalibo`

> [**RDS 到 Crunchy Bridge：一个关于迁移的客户案例研究**](https://www.crunchydata.com/case-studies/brandscope?utm_source=cppg-link-1221)
> CRUNCHY BRIDGE _赞助商_

## 2：[Pagila 3.0：Postgres 示例数据库](https://github.com/devrimgunduz/pagila/)
最初是 MySQL 的“Sakila”示例数据库的一个移植，Pagila 提供了一个完整而真实的模式和数据，可用于教程、演示、学习 SQL 或测试。
来自 Sakila 的 DVD 租赁店隐喻得以保留，但许多额外的功能已经发挥作用，包括 JSONB 列和触发器

`DEVRIM GÜNDÜZ`
> 昨天刚刚发布了一个[**新版本**](https://github.com/devrimgunduz/pagila/releases/tag/pagila-v3.1.0)。

## 3：[OrioleDB：一个新的 Postgres 云原生存储引擎](https://github.com/orioledb/orioledb)
该项目仍处于公共 alpha 阶段，但它的想法是它是一个扩展，旨在为表的访问方式带来一些现代理念，包括undo logs、行级 WAL 和无锁页面读取。

`ALEXANDER KOROTKOV 等人`

## 4：[用于 Postgres 的 Citus 11完全开源](https://www.citusdata.com/blog/2022/06/17/citus-11-goes-fully-open-source/b)
Citus 是 Postgres 的横向扩展扩展，于 2016 年首次开源，采用扩展的“企业”付费版本的商业模式。
然而，从2022 年 6 月开始只会有一个 Citus 版本，并且全部开源。

`MARCO SLOT (CITUS DATA)`

## 5：[很棒的 Postgres：库、工具和资源的精选列表](https://dhamaniasad.github.io/awesome-postgres/)
好吧，我们在作弊，因为这是它自己的完整列表。这个偶尔更新的存储库涵盖了从备份到 GUI 客户端、托管服务到 Docker 映像、博客等所有领域。您还可以通过[**这个代码库**](https://github.com/dhamaniasad/awesome-postgres)贡献您自己的建议。

`ASAD DHAMANI 和其他贡献者`

圣诞快乐、光明节快乐、新年快乐，或者只是..我们明年再见，祝你好运 ;-)

