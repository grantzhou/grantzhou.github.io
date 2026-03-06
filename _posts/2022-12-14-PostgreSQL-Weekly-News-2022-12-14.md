---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2022-12-14
---
### PostgreSQL每周新闻#485 - 2022年12月14日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/485)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,w_350,h_90/e_make_transparent/co_white,e_outline:7/vpntubykyv5ujmbzw501.png)
## [pg_crdt：一个实验性的 CRDT 扩展](https://postgresweekly.com/link/132977/web)
Supabase 开源了一个新的扩展（他们非常热衷于强调它是“实验性的”），用于支持分布式和协作系统中常用的无冲突复制数据类型（CRDT），以允许多个用户同时进行更改，然后进行协调。


`Paul Copplestone (Supabase) `
## [Postgres中的面处理大型结果集](https://postgresweekly.com/link/132978/web)
当谈到搜索和查询界面时，“faceting”是通过应用越来越多的条件（例如，一件衬衫..那是红色的..尺寸）。可以更高效地计算一组特定方面的所有匹配行，如此处所示


`Ants Aasma (Cybertec) `
## [Timescale在Amazon S3上推出新的对象存储层](https://postgresweekly.com/link/132976/web)
借助 Timescale 的新功能，了解您现在如何在 Timescale Cloud 中存储无限量的数据，只需为您存储和访问的数据付费，就好像它们都存在于一个连续的 PostgreSQL 表中一样.


`Timescale `
## [“一切都使用Postgres”](https://postgresweekly.com/link/132979/web)
在这里向合唱团布道，我们同意大部分观点，但这篇简短的评论文章也很有趣，部分原因是推测它是由ChatGPT编写的（！）


`Stephan Schmidt `
## [Postgres中的枚举与检查约束](https://postgresweekly.com/link/132987/web)
枚举或检查约束，哪个更好？Craig 建议检查约束提供更多选择。


`Craig Kerstiens `
## [Postgres 16中的pg_dump压缩规范](https://postgresweekly.com/link/132988/web)
创建的转储pg_dump可以pg_dump通过使用各种命令行标志自行压缩。Postgres 16 让您通过标志指定压缩级别和压缩方法，让事情更进一步


`Pavlo Golub `
## ['我用LiteFS从Postgres集群迁移到分布式SQLite'](https://postgresweekly.com/link/132989/web)
这不是典型的数据库迁移，但随着对面向文件的 SQLite 数据库的关注，我认为我们将继续看到它获得更多可能具有的用例传统上属于 Postgres 或 MySQL。


`Kent C Dodds `
## [通过EXPLAIN成为更好的开发人员](https://postgresweekly.com/link/132990/web)
▶这不是新的，而是一个经典的 40 分钟演讲，深入探讨了查询解析和规划的世界，以及如何分析使用EXPLAIN命令创建的查询计划。继续相关和有用。


`Louise Grandjonc `
## [“我们如何为分析构建最快的Postgres数据库”](https://postgresweekly.com/link/132991/web)
一个大胆的主张。Hydra 是一个开源（此处为代码）数据仓库，它构建在 Postgres 之上，用于 OLAP 和混合工作负载，通过完全托管的平台实现商业化。除了预期的有利基准之外，这篇文章还深入探讨了 Hydra如何解决性能问题。


`Joe Sciarrino (Hydra) `
## [PGTracer:EBPF为Postgres提供的跟踪工具](https://postgresweekly.com/link/132993/web)
当你想要深入时。使用 Linux 的 eBPF 工具（简而言之，一种检查内核中活动的方法，它最初是作为数据包过滤工具使用的）附加到正在运行的 Postgres 后端、监控查询和检测事物。


`Aiven `
## [Dynaboard：专为开发人员设计的Pro Code Web App Builder](https://postgresweekly.com/link/132994/web)


`Dynaboard `
## [Neon上Postgres的“边缘兼容”无服务器驱动程序](https://postgresweekly.com/link/132995/web)
一个无服务器 PostgreSQL 驱动程序，用于从 Cloudflare Workers 和其他支持 WebSockets 的环境连接到Neon（一个新的“无服务器 Postgres”平台）数据库。


`George MacKerron (Neon) `
## [Redis FDW:Redis的Postgres外部数据包装器](https://postgresweekly.com/link/132998/web)
标榜自己是一个“风险自负”的项目，但显然已用于生产。


`Andrew Dunstan and Dave Page `
# 💡本周提示


**🗓即将举办的Postgres活动**
