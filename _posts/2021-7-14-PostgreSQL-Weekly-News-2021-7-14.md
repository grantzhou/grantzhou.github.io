---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2021-7-14
---
### PostgreSQL每周新闻#414 - 2021年7月14日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/414)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/bpbqpcvh8bvxpryrj0tv.jpg)
## [理解Postgres中的LATERAL连接](https://postgresweekly.com/link/111030/web)
您可以认为lateral连接有点像for-each循环，在该循环中，为初始结果集的每一行运行子查询。当然，这是非常有用的！


`Hans-Jürgen Schönig `
## [Timescale添加“超函数”以改进时间序列查询](https://postgresweekly.com/link/111031/web)
TimescaleDB是Postgres的一个面向时间序列的扩展/分发，他们用各种“超函数”扩展了Postgres的SQL支持，用于处理时间序列数据（如时间加权平均值、超日志计数和数据集平滑）。


`Lockerman, Kohn, and Rowe `
## [无需操作、可扩展且灵活的Postgres替代方案](https://postgresweekly.com/link/111034/web)
Fauna将Postgres的操作完整性和关系建模与一个界面和架构结合起来，这个界面和架构更适合云计算中的现代应用程序开发。拥有Postgres的优点但没有它的操作瓶颈-了解更多关于Fauna。


`Fauna `
## [LIMIT与FETCH FIRST ROWS。。。WITH TIES](https://postgresweekly.com/link/111035/web)
我仍然记得，当我第一次得知LIMIT/OFFSET不是标准SQL（尽管许多系统支持它）时，我是多么惊讶。FETCH FIRST可能可移植性更高，但是关于它的使用还有一些要考虑的事情。


`Hans-Jürgen Schönig `
## [DBCritic：对你的Postgres Schema的建设性批评](https://postgresweekly.com/link/111036/web)
Channable的团队构建DBCritic作为一种在Schema中发现问题的方法，因为在他们自己的模式中遇到了各种各样的问题（本文对此进行了解释）。有趣的是，这个工具本身是用很少见到的Idris语言编写的。


`Radek Slupik (Channable) `
## [在运行pg_upgrade之后，逻辑复制会发生什么情况？](https://postgresweekly.com/link/111038/web)
留意你的复制插槽。

`Michał Mackiewicz `

## [使用GDB跟踪到Postmaster在大型查询期间生成的并行工作进程](https://postgresweekly.com/link/111039/web)
顺便说一句，“Postmaster”指的是Postgres中处理传入的客户端连接并将它们路由到服务器进程的部分（尽管该术语本身现在已被弃用）。


`Cary Huang `
## [Crunchy Bridge：完全管理的多云Postgres](https://postgresweekly.com/link/111040/web)

`Crunchy Bridge `

## [Heroku数据库连接计算器](https://postgresweekly.com/link/111041/web)
优化您的数据库池配置依赖于相当多的变量（dynos、worker、进程、线程的数量），因此本指南在解释每个计算的同时也为您提供了数学依据。

`Rails Autoscale `

## [pgSCV 0.7.0发布](https://postgresweekly.com/link/111042/web)
pgSCV是Postgres度量收集器，它以Prometheus格式公开所述度量。


`Alexey Lesovsky `
## [rails-pg-extras 2.0:Postgres对Ruby和rails的性能分析](https://postgresweekly.com/link/111044/web)
Ruby on Rails开发者？这个插件可以让你快速获得有关锁，索引使用，缓存命中率，vacuum统计等信息。还有一个纯Ruby（非Rails）版本。


`Paweł Urbanek `
## [db-to-sqlite 1.4：用于将表或查询从任何SQL数据库导出到sqlite的CLI工具](https://postgresweekly.com/link/111046/web)


`Simon Willison `
# 💡本周提示


**🗓即将举办的Postgres活动**
