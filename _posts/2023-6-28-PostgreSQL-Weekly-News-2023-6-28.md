---
layout: post
title: PostgreSQL 每周新闻 2023-6-28
---
### PostgreSQL每周新闻#512 - 2023年6月28日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/512)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,e_trim,w_380,h_100/e_make_transparent/co_white,e_outline:7/dm8pbpm4svdu3ggeoyqk.png)
## [Vector 是 Postgres 中的新 JSON](https://postgresweekly.com/link/141737/web)
当 JSON 作为一种交换格式迅速普及的时候，每个人都在构建面向文档的数据库时，Postgres 明智地添加了本机 JSON 支持，并逐渐引入了强大的使用方法。 随着机器学习和语言模型嵌入现在使 vector 成为流行的数据结构，Postgres 在这里也有一个新的机会（到目前为止 pgvector 在处理方面做得很好）。


`Jonathan Katz `
## [memory context：Postgres 如何分配内存](https://postgresweekly.com/link/141739/web)
C 中的内存管理是出了名的有趣……棘手且容易泄漏。 Postgres 使用一种称为“memory context”（在某些场景中称为“竞技场”）的方法，其中内存由大的预分配块提供，当所述内存的 context结束时，这些块可以立即释放。 这篇文章介绍了这个想法、它如何影响 Postgres 以及如何监控它们的使用。


`Laurenz Albe `
## [让您的团队从每周 1 次部署增加到每天 100 次部署](https://postgresweekly.com/link/141740/web)
你好奇 Atlassian、谷歌和 Netflix 这样的公司是如何如此频繁地部署的吗？他们使用了什么策略来实现如此高的效率？别担心，本指南为您提供了一些关于这些公司如何扩大部署的有用提示和技巧。你自己去看看吧。


`None`
## [加密 Amazon RDS 或 Amazon Aurora Postgres 数据库](https://postgresweekly.com/link/141742/web)
如果您的基于 AWS 的数据库未加密，而您希望对其进行加密，则需要在复制和快照方面做一些工作，以尽量减少停机时间。


`Bhupathi and Sakhuja (AWS) `
## [在 Django 4.2 中编写流式聊天应用程序](https://postgresweekly.com/link/141748/web)
这很有趣，原因有两个：首先，流行的 Python 框架的最新版本现在直接支持流式 HTTP 响应。 其次，您可以使用 Postgres 的 LISTEN / NOTIFY pub/sub 机制将实时事件流式传输到最终客户端。


`Víðir Valberg Guðmundsson `
## [外部数据包装器的性能提示](https://postgresweekly.com/link/141750/web)
“你不能只让 Postgres 为你做决定，你需要亲自动手。”


`Christopher Winslett `
## [在 Postgres 中使用 iCalendar RRULE](https://postgresweekly.com/link/141751/web)
iCalendar 是一种用于表示日历和日程表的数据格式，而 RRULE 是其定义重复事件的方式。 这对于许多应用程序来说都是有用的，您也可以使用一点 Python 将其引入 Postgres。


`Adrian Klaver `
## [按年、月或日对结果进行分组](https://postgresweekly.com/link/141753/web)
向 DATA_TRUNC()、EXTRACT() 和 TO_CHAR() 打个招呼。


`Mohamed Mayallo `
## [在任何云上运行完全托管的相同 Postgres。 现在免费开始和享有 $300 美元积分](https://postgresweekly.com/link/141754/web)


`EDB BigAnimal `
## [用 Apache Doris 替换 Apache Hive、Elasticsearch 和 Postgres](https://postgresweekly.com/link/141755/web)
我在这里看不到一篇关于用基于 Java 的 MySQL 兼容数据库替换 Postgres 的文章，但为了公平起见.. 😆 另外它叫做 Doris，它 太棒了。


`Apache Doris Team `
## [查找未使用的索引](https://postgresweekly.com/link/141756/web)
未使用的索引会在插入数据、迁移模式以及使用的存储方面产生成本，因此值得了解它们何时潜伏。


`RapidLoop / pgDash `
## [OrioleDB 存储引擎现已进入测试版](https://postgresweekly.com/link/141757/web)
OrioleDB 是 Postgres 的替代现代存储引擎（这是架构文档），针对可能存在高事务吞吐量、大量更新、锁定瓶颈等的用例。不建议用于生产使用， 但团队有足够的信心建议您在测试工作负载上进行测试。 


`Alexander Korotkov `