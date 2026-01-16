---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2021-11-17
---
### PostgreSQL每周新闻#431 - 2021年11月17日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/431)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/qvzaxw6i8o8xzbkypuym.jpg)
## [使用 generate_series() 生成更真实的样本时间序列数据](https://postgresweekly.com/link/116300/web)
如果你从标题中得到似曾相识的感觉，Timescale 之前已经使用 generate_series() 进行了介绍，但这在真实性方面需要进一步提升。 这比你想象的更深入。


`Ryan Booz `
## [PostgreSQL 14.1, 13.5, 12.9, 11.14, 10.19, and 9.6.24 Released](https://postgresweekly.com/link/116302/web)
呼，试着连续说出所有这些版本号而不不会舌头打结。 中间安全漏洞。 请注意，这也是 Postgres 9.6 的最后一个版本。


`PostgreSQL Global Development Group `
## [支持 PostGIS 的 PostgreSQL 数据库中的 OpenStreetMap 数据 - 免费下载](https://postgresweekly.com/link/116303/web)
CYBERTEC 实施了下载 OpenStreetMap 服务，该服务定期生成各种风格的 OpenStreetMap 数据提取，并作为 SQL 转储输出以简化其使用。 免费下载您的地图。


`CYBERTEC PostGIS OSM Downloader `
## [Odyssey 1.2：可扩展的 Postgres 连接池](https://postgresweekly.com/link/116304/web)
三年前，我们首次宣布发布 Yandex 的多线程连接池和路由器，它用于在内部每秒处理超过 100 万个请求。 它不断更新，现在支持 PAM 和 LDAP。


`Yandex `
## [dynamodb_fdw 1.0：DynamoDB 的外部数据包装器](https://postgresweekly.com/link/116305/web)
我自己还没有测试过，但我很惊讶到目前为止它只获得了一颗星。 这里的想法是提供从 Postgres 到 Amazon 的 DynamoDB 键/值文档数据库的访问。


`PGSpider `
## [pg_auto_failover 简介](https://postgresweekly.com/link/116309/web)
pg_auto_failover 是在 Postgres 集群中提供自动故障转移的扩展。 这篇文章讲述了扩展的整个故事，它是如何工作的，以及它的价值所在。


`Dimitri Fontaine `
## [在 Windows 上使用 WSL2 安装 Postgres](https://postgresweekly.com/link/116311/web)
Windows 子系统 Linux (WSL) 为在 Windows 上运行 Linux 二进制文件提供了一个兼容层，这意味着你可以以面向 Linux 的方式构建 Postgres 并在 Windows 上运行它，如果你愿意，而不是使用 本机 Windows 构建。


`Pavlo Golub `
## [在 Kubernetes 上轻松运行用于 Postgres 的 Babelfish](https://postgresweekly.com/link/116312/web)
Babelfish 是来自 AWS 的一个开源项目，它在 Postgres 之上添加了一个 SQL Server 兼容层，而 StackGres 是一个在 Kubernetes 上运行 Postgres 的平台。 您现在可以将这两者结合在一起。


`Alvaro Hernandez `
## [分析 Postgres 中的扫描](https://postgresweekly.com/link/116314/web)
了解不同类型的扫描以及查询规划器在不同情况下选择它们的原因。 如果您在查询计划中看到过诸如“顺序扫描”或“位图堆扫描”之类的术语并且不太明白它们的含义，这里提供了一些（非常基本的）解释。


`Zach Naimon `
## [ORDER BY 在 SQL 中是强制性的，以获取排序的结果](https://postgresweekly.com/link/116315/web)
你可能不假思索地隐含知道的事情之一。


`Franck Pachot `
## [像查询 Postgres 一样查询 MongoDB - 使用 SQL 使用 Studio 3T](https://postgresweekly.com/link/116321/web)


`Studio 3T `
## [PGroonga：将全文搜索功能扩展到所有语言](https://postgresweekly.com/link/116317/web)
将 Groonga 全文搜索引擎引入 Postgres，它可以比 Postgres 的默认设置更适合某些用例，例如日语或中文。


`PGroona Project `
## [Cloudflare Workers 推出关系数据库连接器](https://postgresweekly.com/link/116319/web)
Workers 是 Cloudflare 的全球分布式无服务器功能平台，他们添加了一项功能，用于通过隧道将功能连接到内部托管的关系数据库（包括 Postgres）。


`Sikand, McKeon and Yule (Cloudflare) `
