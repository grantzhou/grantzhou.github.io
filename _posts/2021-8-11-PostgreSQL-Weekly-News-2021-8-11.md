---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2021-8-11
---
### PostgreSQL每周新闻#418 - 2021年8月11日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/418)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/qvdzgew7zremkq8iegut.jpg)
## [使用 ROLLUP 和 CUBE 分组集](https://postgresweekly.com/link/112230/web)
分组集是在 GROUP BY 子句中使用的一组列，可以在 OLAP 查询中派上用场。 这篇文章有一些方便的例子。


`Hans-Jürgen Schönig `
## [网络和游标对查询性能的影响](https://postgresweekly.com/link/112231/web)
当我们考虑数据库或查询性能时，通常不会考虑网络相关的开销，但意识到这一点是值得的。 游标也被考虑在内，因为它们可以减少大结果集的初始延迟。


`Jobin Augustine `
## [CYBERTEC TDE：PostgreSQL 的透明数据加密](https://postgresweekly.com/link/112232/web)
TDE 是 PostgreSQL 的自定义补丁。它是目前唯一完全支持透明和加密安全数据（集群）级加密的实现，独立于操作系统或文件系统加密。 在此处下载 TDE。


`CYBERTEC `
## [使用 Postgres 和 Cloudflare Workers 实现 REST API 的现代化](https://postgresweekly.com/link/112236/web)
PostgREST 是一种为 Postgres 数据库生成 REST API 的工具，在这里我们了解如何使用 Cloudflare Tunnel 让 Worker 实例与托管在私有网络上的 PostgREST 实例通信.


`Kristian Freeman (Cloudflare) `
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/gcyjh2i69o04nyrfkhwt.jpg)

## [LATERAL Join 用例的一个简单示例](https://postgresweekly.com/link/112238/web)
一个月前，我们链接到了一篇关于理解 LATERAL joins 的文章，但这是一个实际用例。


`Luca Ferrari `
## [Citus 10 发布在 Hyperscale (for Postgres on Azure)](https://postgresweekly.com/link/112233/web)
仅适用于你们中的 Azure 用户，但 Azure 自己的超大规模 Postgres 服务现在支持最新的 Citus 版本。


`Nik Larin (Microsoft) `
## [Citus 如何分发 PostgreSQL](https://postgresweekly.com/link/112234/web)
▶如果您一直看到对 Citus 的引用（如上），但不确定它如何帮助分发 Postgres，Marco Slot 做了一个性能提升，让您了解最新情况。 幻灯片非常棒，其中包含大量 Citus 操作的图表和示例。


`Marco Slot `
## [Postgres_fdw Postgres 14 中的增强功能](https://postgresweekly.com/link/112240/web)
外部数据包装器 (FDW) 中预期的一些更改的预览，用于处理存储在外部 Postgres 服务器中的数据。


`Ibrar Ahmed `
## [📈如何使用 Postgres、Python 和 TimescaleDB 分析股票数据](https://postgresweekly.com/link/112242/web)


`Timescale `
## [使用 Postgres 类型](https://postgresweekly.com/link/112241/web)
作者一直在尝试在 Postgres 函数之间共享类型。


`Jon Udell `
## [10 个常见的 Postgres 错误](https://postgresweekly.com/link/112243/web)
一些需要注意的快速常见错误和警告，以及症状和解决方案，围绕内存、磁盘空间和权限等问题。 （这是一个较旧的项目，但最近再次出现在我们的雷达上。）


`Ibrar Ahmed `
## [PureORM：用于编写原生 SQL 查询产生纯业务对象的 Node.js SQL 工具包](https://postgresweekly.com/link/112244/web)
允许您编写常规的原生 SQL 并接收正确结构化（嵌套）的纯业务对象，而不是典型的 ORM来实现其他地方构建查询的方法。


`Craig Martin `

