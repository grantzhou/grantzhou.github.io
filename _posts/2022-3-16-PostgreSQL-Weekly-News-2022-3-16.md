---
layout: post
title: PostgreSQL 每周新闻 2022-3-16
---
### PostgreSQL每周新闻#446 - 2022年3月16日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/446)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/yjh9mvmvvednofiddgzd.jpg)
## [使用 150 行 SQL 进行 Postgres 审计](https://postgresweekly.com/link/120926/web)
审计，从跟踪随时间变化的意义上说，在许多情况下是一个基本过程，并且可以在 Postgres 内部创建一个完全在 Postgres 内部的审计系统，只需小心谨慎地使用 PL/ pgSQL。


`Oliver Rice (Supabase) `
## [Hooks：为 Postgres 生态系统提供动力的“秘密”功能](https://postgresweekly.com/link/120927/web)
Hooks 是 Postgres 的一个非官方文档的内部部分，它允许扩展来扩展或更改 Postgres 的行为。这篇文章着眼于一些常见的扩展如何使用它们来让 Postgres 做超出其原始设计的事情。


`Everett Berry `
## [Studio 3T 管理您的数据，同时让您的应用程序成形](https://postgresweekly.com/link/120929/web)
Studio 3T 的全套 MongoDB 工具可让您更快地查询，更快地使用数据进行开发，并自动将查询转换为代码。免费试用 30 天 - 无需信用卡。


`Studio 3T `
## [如何避免重复键违规的隐患](https://postgresweekly.com/link/120935/web)
如果多个客户端试图同时将相同的数据插入同一个表中，可以使用约束来防止重复，但可能会出现各种问题，包括浪费存储和不必要的自动吸尘工作。


`Divya Sharma and Shawn McCoy (AWS) `
## [在慢速网络上提高性能的管道模式](https://postgresweekly.com/link/120936/web)
Postgres 14 在 C API 中引入了一种“管道模式”，libpq它可以通过允许通过线路发送多个语句而无需每次等待响应来提高高延迟连接的性能。


`Laurenz Albe `
## [我的 Autovacuum 配置正确吗？](https://postgresweekly.com/link/120937/web)
Autovacuuming 是 19 年前在 Postgres 中引入的（！），但仍然会给数据库管理员带来偶尔的问题。密切关注正在发生的事情并调整一些参数可以有很长的路要走。


`Hubert depesz Lubaczewski `
## [PostGIS vs GPU for Performance and Spatial Joins](https://postgresweekly.com/link/120941/web)
GPU 辅助空间连接项目与 PostGIS 等效项目的实际比较。虽然 GPU 方法更快，但 Postgres 仍然有一些重要的优势需要考虑。


`Paul Ramsey `
## [如何在 Azure 上使用 HammerDB 对 Citus 和 Postgres 的性能进行基准测试](https://postgresweekly.com/link/120942/web)
HammerDB 是一个众所周知的数据库基准测试套件，因此提供了一种让系统承受压力的好方法。


`Jelte Fennema (Microsoft) `
## [PostgreSQL Anonymizer 0.10 已发布](https://postgresweekly.com/link/120944/web)
一种扩展，可在 Postgres 中使用各种不同的屏蔽方法屏蔽或替换个人身份信息 (PII) 或商业敏感数据。现在还有📒 50 页的 PDF文档，详细记录了如何使用该工具。


`Dalibo Labs `
## [🐘你一直想要的 Postgres 开发者体验](https://postgresweekly.com/link/120940/web)
l,null,"en


`Crunchy Bridge `
## [pg_dumpbinary：以二进制格式转储数据的数据库](https://postgresweekly.com/link/120946/web)
在特定情况下，使用二进制格式进行转储有一些好处。


`lzlabs `
## [PGSync 0.7：在数据库之间同步 Postgres 数据](https://postgresweekly.com/link/120948/web)
速度和安全性是当务之急，您可以同步部分表或表组。自述文件展示了一些示例。用红宝石写的。


`Andrew Kane `
## [supa_audit：Postgres 的通用表审计](https://postgresweekly.com/link/120949/web)
使用与上面链接的审计文章中概述的相同技术。


`Supabase `
# 💡本周提示


**🗓即将举办的Postgres活动**
