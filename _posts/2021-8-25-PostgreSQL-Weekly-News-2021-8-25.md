---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2021-8-25
---
### PostgreSQL每周新闻#419 - 2021年8月25日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/419)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/uood2wvg03lmyw6by1nj.jpg)
## [使用CREATE INDEX：操作符表，索引类型等](https://postgresweekly.com/link/112750/web)
创建索引是一回事，但创建索引以及另一回事。Lukas 着眼于使用的实用性，CREATE INDEX并演示了如何分析您的查询以找出要创建的最佳索引。


`Lukas Fittl `
## [pg_timetable v4 已发布](https://postgresweekly.com/link/112815/web)
pg_timetable是 Postgres 的高级调度系统，可让您按照您选择的时间表执行功能或进程，例如吸尘。现在有更好的日志记录、更高的性能和一个配置文件。


`Pavlo Golub `
## [使用 Datadog 实时监控自定义 Postgres 指标](https://postgresweekly.com/link/112752/web)
在上下文中端到端监控和可视化 Postgres 性能以及堆栈的其余部分。创建自定义的拖放仪表板以快速查看任何 Postgres 指标的分析。免费试用 Datadog。


`Datadog `
## [Postgres vs Redis vs Memcached 性能](https://postgresweekly.com/link/112751/web)
这些数据存储中的每一个都有不同的用例，但如果你跳过缓存并直接访问数据库，它的性能如何？Kaarel 运行了一些基准测试并分享了他们的想法。


`Kaarel Moppel `
## [修复不同步的序列](https://postgresweekly.com/link/112753/web)
我们最近链接到了一个关于Postgres 在序列中“跳过”值的故事，但你知道有一个用于修复不同步的序列的扩展吗？


`Hans-Jürgen Schönig `
## [Apache AGE 0.5.0 发布](https://postgresweekly.com/link/112756/web)
Apache AGE（ A Graph Extension）是一个 Postgres 扩展，它添加了图形数据库功能（完整的 openCypher 查询支持）并受到 AgensGraph 的启发。


`The Apache Software Foundation `
## [比较 Amazon RDS 数据库的升级方法](https://postgresweekly.com/link/112757/web)
快速了解使用 AWS 托管 Postgres 产品时进行版本升级的四种不同方法的优缺点。


`Arumugam Petchimuthu `
## [使用pglogical升级一个RDS数据库](https://postgresweekly.com/link/112758/web)
在上面展示了“最少的停机时间”后的直接后续使用升级方法pglogical进行复制。


`Arumugam Petchimuthu `
## [如何查看用户的继承权限](https://postgresweekly.com/link/112759/web)
如果我们在本周运行一周提示，这将是一个理想的提示！


`Richard Yen `
## [🐘如何以及为何成为 Postgres 贡献者：技巧和最佳实践](https://postgresweekly.com/link/112760/web)
l,null,"en


`Timescale `
## [通过在 Amazon RDS 上分区表来加速时间序列数据摄取](https://postgresweekly.com/link/112761/web)
了解分区表如何以及为何有助于数据摄取。虽然这主要集中在 RDS 上，但由于作者在亚马逊工作，其中大部分也具有普遍价值。


`Vinicius Schmidt and Andy Katz `
## [pgdiff：比较两个时间点之间的数据变化](https://postgresweekly.com/link/112762/web)
想想git diff但是针对postgres。


`Denver Smith `
## [sqlc 1.9：从 SQL 生成类型安全的 Go(lang)](https://postgresweekly.com/link/112763/web)
你编写 SQL 查询，运行sqlc以生成这些查询的代码和接口，然后编写调用上述代码的 Go 代码。v1.9.0添加了对s 中的视图pgx/v4、 和子查询SELECT的支持。


`Kyle Conroy `
# 💡本周提示


**🗓即将举办的Postgres活动**
