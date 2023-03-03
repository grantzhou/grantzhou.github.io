---
layout: post
title: PostgreSQL 每周新闻 2023-3-1
---
### PostgreSQL每周新闻#495 - 2023年3月1日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/495)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,e_trim,w_740,h_100/e_make_transparent/co_white,e_outline:10/d9sktlkk3ipcaszkhybd.png)
## [使用 Postgres 进行欧洲路线规划](https://postgresweekly.com/link/136042/web)
我们喜欢 Mark，因为当他发现欧洲公交路线数据集时，他会启动 Postgres 并使用 pgRouting 构建可视化和路线规划器。 这个方法并没有什么特别新颖的地方，但是当你需要解决相关问题时，它是你会需要的工具。


`Mark Litwintschik `
## [Amazon RDS 现在支持 Postgres 15](https://postgresweekly.com/link/136046/web)
去年 10 月推出的 Postgres 15 现在在 RDS 中得到完全支持，并具有 80 多个扩展。


`Amazon Web Services `
## [Netflix 数据库的历史](https://postgresweekly.com/link/136040/web)
在基础架构层面，如何才能向全球数百万并发用户提供像素完美且无缓冲的流媒体？ 深入了解流媒体巨头成功背后的弹性和架构。


`CockroachDB `
## [152 个 psql 技巧](https://postgresweekly.com/link/136052/web)
当我们第一次包含它时，这最初是 100 个技巧，但是这个针对久经考验的 psql 客户端的的技巧列表还在继续增长。 如果您很快就会有一个 psql 会话，那么值得浏览一下。


`Lætitia Avrot `
## [存储过程入门](https://postgresweekly.com/link/136062/web)
存储过程是某些类型的数据库工作的基础，但如果您根本没有接触过它们，那么这篇介绍适合您。


`Hans-Jürgen Schönig `
## [我们能否让权限管理更加人性化？](https://postgresweekly.com/link/136064/web)
授予和权限随着 Postgres 的新版本不断发展，但仍然存在一些尖锐的边缘和不一致之处。


`Henrietta Dombrovskaya `
## [将树存储为物化路径](https://postgresweekly.com/link/136066/web)
将树存储在数据库中很复杂，但以物化路径的形式存储它们（想想域和子域本质上如何表示树结构——例如 mail.example․com）可以简化查询它们的过程。


`Tobias Petry `
## [ALTER TABLE … SET WITHOUT OIDS：一个大陷阱](https://postgresweekly.com/link/136068/web)
当你删除一个列时，它会被标记为不活动的，就是这样。 除非您使用 SET WITHOUT OIDS，否则最终会重写整个表并可能导致长时间运行的锁定。


`Christophe Pettus `
## [Postgres 栅格查询基础知识](https://postgresweekly.com/link/136070/web)
Paul 向我们介绍了如何使用 PostGIS 存储和查询栅格（想想像素/像元，而不是矢量），以及如何思考它们带来的挑战。


`Paul Ramsey `
## [pgtt 2.10：管理和使用 Oracle 风格的全局临时表](https://postgresweekly.com/link/136074/web)
适用于您想要重现 Oracle 的行为而不是重写代码以使用标准 Postgres 临时表的情况。


`Gilles Darold `
## [Tuple，专为远程开发人员打造的快如闪电的配对工具](https://postgresweekly.com/link/136076/web)


`Tuple `
