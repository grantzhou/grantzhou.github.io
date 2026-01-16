---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2022-9-14
---
### PostgreSQL每周新闻#471 - 2022年9月14日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/471)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/y865x5tl8zwchiahdy4i.jpg)
## [选择主键标识符格式：选项](https://postgresweekly.com/link/128701/web)
确定用于主键的数据，甚至数据组合可能比您预期的要复杂，如果您使用常见的唯一 ID 方法，您应该利用？Victor 浏览了 Postgres 的许多选项以及它们的优缺点，然后展示了他为帮助您生成 ID 而构建的扩展。


`Victor Vados `
## [pg_netstat：监控您的数据库的网络流量量](https://postgresweekly.com/link/128703/web)
运行一个后台工作程序，该工作程序使用 libpcap 以您选择的时间间隔捕获数据包和聚合。然后，您可以通过pg_netstat视图查询数据库的实时网络统计信息，以查看进出数据包、进出字节等。


`Supabase `
## [PDF 下载：了解 Kubernetes](https://postgresweekly.com/link/128704/web)
2022 年更新！该资源涵盖了从基本概念到集群组件和网络模型实现的所有内容。新版本包括 Kubernetes 仪表板、高可用性控制平面和自动缩放。立即获得。


`Linode `
## [使用事务快照](https://postgresweekly.com/link/128705/web)
这是另一个很方便的功能。快照允许多个事务共享相同数据库状态的相同视图。pg_dump当允许多个实例使用该选项更快地构建单个转储时-j，或者在更复杂的数据同步场景中（帖子中提供了一个简洁的示例）时，这可以派上用场


`Robert Bernier `
## [PostgreSQL 15 Beta 4 已发布](https://postgresweekly.com/link/128706/web)
每周发布的一个缺点是发布后的第二天就发布了，因此它与上周四的发布一起发布；-) 幸运的是，这是通往 Postgres 15 道路上相对较小的一步，主要是修复错误和崩溃


`PostgreSQL Global Development Group `
## [“我希望在开始时就知道的 6 个有用的 Postgres 功能”](https://postgresweekly.com/link/128710/web)
身份语法（与 SERIAL 相比）、COALESCE + NULLIF、分组集、CTE 和域都出现了。


`Marat Badykov `
## [SQL 中的INNER JOINor是什么？OUTER JOIN](https://postgresweekly.com/link/128711/web)
如果您已经是连接专家，请明确指出，否则这是一个很好的介绍/复习，也可以轻松完成完全连接和“半连接”。


`Hans-Jürgen Schönig `
## [ppgcrypto 做了什么](https://postgresweekly.com/link/128712/web)
它让我们觉得好笑，但遗憾的是，我们不得不更改 Paul 的实际“加密”相关标题以避免命中垃圾邮件过滤器；-) 尽管如此，他还是对pgcrypto提供的加密和解密选项进行了实用、高级的研究数据库中的数据。


`Paul Ramsey `
## [Citus 如何以及为何将分布式 Postgres 完全开源](https://postgresweekly.com/link/128714/web)
关于为什么 Citus / Microsoft 开源 Citus 11 中剩余的少数企业功能的内幕故事，开源的确切内容以及实现它所采取的措施。


`Jelte Fennema (Citus Data) `
## [pg_idkit：用于生成 ID 的扩展](https://postgresweekly.com/link/128702/web)
在上面介绍的选择 Postgres 主键文章中，这个 Rust 构建的扩展提供了从 UUID 到 NanoID 和 ksuid 的无数不同的唯一 ID 方案。


`VADOSWARE LLC `
## [将关键任务应用程序迁移到云端……更快(https://postgresweekly.com/link/128715/web)
l,null,"en


`EDB BigAnimal `
## [Apache AGE 1.1.0：Postgres的图形扩展](https://postgresweekly.com/link/128716/web)
AGE（图形扩展）的灵感来自 AgnsGraph，这是一个基于 PostgreSQL 10 构建的多模型数据库 Bitnine，并通过 OpenCypher 和 SQL 为 Postgres 带来图形处理和分析功能。


`Apache Foundation `
# 💡本周提示


**🗓即将举办的Postgres活动**
