---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2022-6-22
---
### PostgreSQL每周新闻#460 - 2022年6月22日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/460)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/ctmux0lxk5sgijmm3kkf.jpg)
## [用于 Postgres 的 Citus 11 完全开源](https://postgresweekly.com/link/125080/web)
Citus 是 Postgres 的横向扩展插件，六年前首次开源，但其通用商业模式是提供扩展的“企业”版本以赚钱。 不再。 现在只有一个 Citus 版本，而且都是开源的，因此租户隔离、非阻塞分片重新平衡等功能现在对所有人开放。 这是一个巨大的版本，并在这篇文章中得到了很好的解释。


`Marco Slot (Citus Data) `
## [Postgres 14.4 已发布](https://postgresweekly.com/link/125081/web)
上周我们警告说即将发布 Postgres 14 更新，以解决在使用 CREATE INDEX CONCURRENTLY 或 REINDEX CONCURRENTLY 时索引无声损坏的令人讨厌的错误，现在它就在这里。 您可以使用 pg_amcheck 查看您是否受到影响。 非 Postgres 14 用户不受影响。


`PostgreSQL Global Development Group `
## [时间戳和时区：你需要知道的和你不知道的](https://postgresweekly.com/link/125082/web)
一些 PostgreSQL 程序员被日期和时间数据类型以及会话的时区设置对操作的影响所吓倒。 YugabyteDB 的 YSQL 可以带来相同的体验。 阅读最近对该主题进行的一项仔细而详尽的研究。


`YugabyteDB `
## [如何在 Postgres 上查找和停止运行查询](https://postgresweekly.com/link/125088/web)
Postgres 在一些麻烦的查询或资源限制的压力下陷入困境，您需要快速控制......如何在不破坏整个系统情况下停止这些查询？ 这篇文章在探讨和负责 Postgres 的后端流程方面比您预期的要详细得多。


`Adam Johnson `
## [TimescaleDB 2.7 如何使其数据聚合更好更快](https://postgresweekly.com/link/125089/web)
Timescale 的人们肯定正在努力使其成为时间序列工作负载的一个引人注目的选择。 这篇文章深入探讨了一些基准测试，展示了新的 2.7 版本与 2.6 相比有多快，一些查询速度提高了 44,000 倍（通常需要减少 60% 的存储空间）。


`Ryan Booz (Timescale) `
## [使用灵活的服务器 PostgreSQL HA 实现高正常运行时间](https://postgresweekly.com/link/125090/web)
“HA”不是笑料，而是高可用性，Azure 为其略微冗长的 Database for PostgreSQL 灵活服务器服务引入了一些新的 HA 功能。

`Sridhar Ranganathan (Microsoft) `
## [The Dalibo Postgres 执行计划可视化器](https://postgresweekly.com/link/125091/web)
给出 EXPLAIN ANALYZE 的输出并更好地了解 Postgres 计划如何处理您的查询。 与广为人知的 explain.depesz.com 类似，但以完全不同的方式呈现结果，因此两者都值得尝试。 这已经有一段时间了，但最近有一些更新。


`Dalibo `
## [使用 Datadog 数据库监控快速识别和解决 Postgres 查询](https://postgresweekly.com/link/125093/web)


`Datadog Database Monitoring `
## [pg_squeeze：修复表格膨胀的扩展](https://postgresweekly.com/link/125140/web)
虽然它不能替代vacuum，但它拥有一个方便的扩展，可以更进一步并在表格上获得更多空间改进。


`CYBERTEC `
## [pgCluu：Postgres 性能监控和审计工具](https://postgresweekly.com/link/125141/web)
一个由两部分组成的工具，它从正在运行的 Postgres 集群收集统计信息，然后提供性能信息供您检查。 

`Gilles Darold `

## [Cloudflare Workers Postgres 客户端](https://postgresweekly.com/link/125095/web)

`BUBBLYDOO`

