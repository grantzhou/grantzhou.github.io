---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2022-6-29
---
### PostgreSQL每周新闻#461 - 2022年6月29日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/461)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/ttj3vztwmqphfjdt0qkk.jpg)
## [Google Cloud Spanner 的 Postgres 接口正式发布](https://postgresweekly.com/link/125437/web)
看到很多聪明人歌颂非开源的云数据库是不寻常的，但 Google 的 Cloud Spanner 凭借其高可用性、可扩展性和 ACID 合规性的承诺而拥有许多这样的粉丝——进入 Postgres 生态系统被视为一个越来越重要的因素。 值得注意的是，作者说：“PostgreSQL 是用于操作数据库的新‘API’，”——也许我们可以期待 Google 对 Postgres 的更多热爱？


`Justin Makeig (Google Cloud) `
## [Amazon Aurora 增加了对 Postgres 14 的支持](https://postgresweekly.com/link/125438/web)
Amazon 高度可扩展的托管 类似Postgres 服务通过改进的并行查询、分区表、逻辑复制和清理以及新功能提升到 Postgres 14 标准 像多范围类型。 这是新功能的完整清单。


`Amazon Web Services `
## [Teleport 的工作原理：基本概念](https://postgresweekly.com/link/125465/web)
Teleport 是访问所有基础设施的最简单、最安全的方式。 Teleport 提供对 SSH 或 Windows 服务器、Windows 桌面、Kubernetes 集群、数据库（PostgreSQL、MongoDB、Redis 等）和 Web 应用程序的安全访问。 学习更多。


`Teleport `
## [在 Postgres 中调试死锁](https://postgresweekly.com/link/125443/web)
锁提供了一种保护数据完整性的绝妙方法，直到您遇到死锁。 Laurenz 设置了一个简单的死锁，以展示一些调试它们的技术。


`Laurenz Albe `
## [Postgres 索引、选择性和统计数据](https://postgresweekly.com/link/125444/web)
当 Postgres 的查询计划没有达到标准时，深入了解一些调整的方法。


`Paul Ramsey `
## [Postgres 升级很难](https://postgresweekly.com/link/125445/web)
如果你和 Hacker News 上的一些人一样，想说“升级很容易，只需使用 pg_upgrade”，请务必阅读这些说明，因为惊喜和边缘案例比比皆是。


`Andreas 'ads' Scherbaum `
## [通过 Postgres 使用 Cloudflare Tunnel 和 Access](https://postgresweekly.com/link/125448/web)
Cloudflare 的数据库团队解释了他们如何在内部使用 Cloudflare 的 Tunnels 服务来提高员工访问数据库的安全性。


`McNeil and Ravichandran (Cloudflare) `
## [pg_squeeze：修复表格膨胀的扩展](https://postgresweekly.com/link/125449/web)
虽然它不能替代vacuum，但它拥有一个方便的扩展，可以更进一步地在表格上获得更多空间改进。


`CYBERTEC `
## [Barman 3.0: Backup and Recovery Manager for Postgres](https://postgresweekly.com/link/125450/web)
一个管理工具，用于执行 Postgres 服务器的远程（热）备份和灾难恢复。


`EDB `
## [在 pganalyze 资源库中查看我们的免费 Postgres 电子书](https://postgresweekly.com/link/125452/web)


`pganalyze `
## [pgenv 1.3: Postgres 二进制文件管理](https://postgresweekly.com/link/125453/web)
旨在简化 Postgres 不同版本的构建和运行，特别是在它们之间切换以进行测试等。


`David E. Wheeler and Contributors `
## [pg_ivm 1.1：IVM（增量视图维护）扩展](https://postgresweekly.com/link/125454/web)
增量视图维护以计算和应用增量更改而不是重新计算所有内容的方式使物化视图保持最新。 pg_ivm 提供了一种“即时维护”，其中物化视图在基表被修改后立即更新。 v1.1 添加了 Postgres 13 和聚合支持。


`SRA OSS, Inc. Japan `
## [PGSpider 1.0：分布式大数据的数据虚拟化引擎](https://postgresweekly.com/link/125455/web)
想想集群在规模上满足 FDW功能？


`Toshiba Corporation `

