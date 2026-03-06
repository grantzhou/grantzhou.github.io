---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2023-3-22
---
### PostgreSQL每周新闻#498 - 2023年3月22日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/498)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,e_trim,w_330,h_112/e_make_transparent/co_white,e_outline:5/glyygzju08rfcfwf2sxw.png)
## [简易Postgres时间箱](https://postgresweekly.com/link/137132/web)
一些“分类”基于时间的数据以生成有用的图表和报告的技巧。使用generate_series()、width_bucket()、floor()和 等date_bin()，您可以以不同方式对数据集进行分组，并快速检索基于查询的报告。


`Paul Ramsey `
## [现场可靠性工程师和软件工程师C++](https://postgresweekly.com/link/137131/web)
加入我们的“牛逼”团队。我们的软件团队在 17 个国家开展业务，我们一直在寻找更多杰出的工程师。


`Stickermule `
## [在Heroku上宣布Postgres 15](https://postgresweekly.com/link/137133/web)
Heroku 曾经是提供托管 Postgres 服务的领跑者，现在已经为所有新应用程序提供了 Postgres 15，如果您使用的是 9.6 或 10，我们鼓励您尽快升级。


`Heroku `
## [批量修改后的表维护](https://postgresweekly.com/link/137141/web)
对表进行大量修改可能会扭曲Postgres 的查询计划器使用的统计信息，因此在进行此类更改后重新计算这些统计信息可能是明智之举。ANALYZE table_name救援


`Tobias Petry `
## [排序规则的工作原理](https://postgresweekly.com/link/137142/web)
排序规则是指系统应该如何比较和排序字符串的规则。在这里，Peter Eisentraut 解释了归类在 Postgres 中的工作原理以及 Unicode 在定义归类标准中的作用。


`Peter Eisentraut `
## [删除与删除](https://postgresweekly.com/link/137140/web)
了解您想要删除数据的DELETE和TRUNCATE主要区别在于行级和表级操作。


`Hans-Jürgen Schönig `
## [使用Rails和Postgres的基本时间序列数据](https://postgresweekly.com/link/137143/web)
如果您正在处理时间序列数据并且还没有准备好跳到更专用的东西，那么这是一个很好的起点。


`Saad Syed (Census Engineering) `
## [pgwarehouse:将Postgres数据库同步到Snowflake或Clickhouse仓库](https://postgresweekly.com/link/137144/web)
作者在 Hacker News 上说： “最近构建它是为了帮助一位朋友从他们的 Postgres 数据库中设置一个 Snowflake 仓库。还使用 ClickHouse 对其进行了测试，这对于在本地运行很酷。使用快速且不需要二进制日志访问的简单 COPY，但因此不支持实时复制。”


`Scott Persinger `
## [Tuple，一个为远程开发人员构建的闪电快速配对工具](https://postgresweekly.com/link/137145/web)


`Tuple `
## [PgLock 1.0：使用咨询锁隔离跨机器的代码执行](https://postgresweekly.com/link/137146/web)
针对 Rubyists，但有趣的是看到 Postgres 如此直接用于管理跨非数据库相关进程的锁。


`Heroku `
## [Frenzy:Postgres有线协议感知镜像代理](https://postgresweekly.com/link/137147/web)
—这个基于 Go 的 Postgres 代理还处于早期阶段，但很有趣的是在这个阶段看到一些确实有效的东西，如果你需要构建自己的类似东西可能会有用。 ”这真是 suuuuuper hacky，但在 2 小时的工作中，我能够代理一些查询！”


`Kelly Sommers `
# 💡本周提示


**🗓即将举办的Postgres活动**
