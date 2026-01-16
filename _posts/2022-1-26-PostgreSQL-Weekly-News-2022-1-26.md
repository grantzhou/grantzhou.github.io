---
layout: post
title: PostgreSQL 每周新闻 2022-1-26
---
### PostgreSQL每周新闻#439 - 2022年1月26日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/439)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/gb9ywcridxgik91rsomr.jpg)
## [PostGIS 的高程剖面和飞行路线](https://postgresweekly.com/link/118947/web)
我总是对使用 PostGIS 和 Postgres 进行的地理工作印象深刻。 这篇文章演示了将飞行的各种点变成实际的飞行路径。


`Paul Ramsey `
## [如何使用 generate_series() 和 SQL 塑造样本数据](https://postgresweekly.com/link/118948/web)
关于使用 Postgres 本身生成大量测试数据集以进行基准测试、测试工作负载或使用数据库功能的系列文章中的最后一篇。 此阶段继续操作此类生成的数据以适应所需的配置文件。


`Ryan Booz (Timescale) `
## [免费电子书：Postgres 中的有效索引](https://postgresweekly.com/link/118945/web)
了解如何为您的查询创建最佳 Postgres 索引。 我们深入探讨了索引类型、运算符、数据类型等。 创建正确的索引通常可以提高您的查询性能。


`Pganalyze `
## [数据库实验室引擎：一种快速克隆 Postgres 数据库的方法](https://postgresweekly.com/link/118949/web)
承诺“超快”数据库克隆（声称能够在 10 秒内克隆 1TB 数据库，这要归功于其写时复制方法），特别是用于构建开发或 QA/暂存环境 基于全尺寸的生产型数据库。


`Postgres.ai `
## [Postgres 新手索引](https://postgresweekly.com/link/118950/web)
如果您了解 B-Tree、GIN 和 GIST 索引之间的区别，请跳过这篇文，这将为您提供非常高级的概述。 如果你想更进一步，你可以阅读更详细的指南，比如 B-trees 或 BRIN 索引。


`Elizabeth Christensen `
## [使用 Postgres 应对 Advent of Code 挑战的一些经验教训](https://postgresweekly.com/link/118957/web)
Advent of Code 是每年 12 月举行的一组年度编程挑战。 通常使用 Python 或 C# 等语言，但有些人开始使用 SQL 等语言。 虽然作者没有用 SQL 完成全部 25 天，但他们通过尝试学到了一些有趣的东西。


`Matt Dupree and Amanda Murphy `
## [AWS 的 Postgres 平台安全最佳实践概述](https://postgresweekly.com/link/118959/web)
以 AWS 为导向，了解使用 RDS for PostgreSQL 或 Aurora 的 Postgres 风格时应遵循的良好实践。 安全组、强制 SSL、IAM 身份验证和加密都会出现。


`Baji Shaik and Divya Sharma (AWS) `
## [加速 Postgres 中的 VACUUM](https://postgresweekly.com/link/118960/web)
我们已经有一段时间没有发表大量关于清理的文章了，但这里有一些快速提示可以调整 Postgres 的设置以加速自动清理过程。


`Alexei Kozlov `
## [使用 Postgres 进入“只读”模式](https://postgresweekly.com/link/118961/web)
如果您需要暂时将 Postgres 实例置于“只读”状态，可以使用 default_transaction_read_only 来阻止写入事务。


`Jonathan Katz `
## [使用 Flux 和 PostgreSQL 丰富实时应用程序的数据](https://postgresweekly.com/link/118946/web)


`InfluxData `
## [安装 Citus 和 Postgres 包的提示](https://postgresweekly.com/link/118962/web)
Citus 是众所周知的水平扩展 Postgres 的扩展，这篇文章回答了一些关于它如何打包以及如何安装和管理的问题。


`Gürkan İndibay (Citus Data) `
## [使用 Postgres 咨询锁进行分布式锁定](https://postgresweekly.com/link/118964/web)
Postgres 的咨询锁功能可以为您的应用程序提供有用且值得信赖的锁定机制，甚至不必涉及存储在 Postgres 本身中的数据。 这篇文章（从 2020 年开始——我们当时错过了它）展示了一家公司如何使用它们。


`Richard Clayton `
## [如何创建 Amazon CloudWatch 仪表板以监控 AWS 上的 Postgres](https://postgresweekly.com/link/118966/web)
深入探讨了创建用于监控 RDS 或 Aurora 的动态仪表板，包括慢查询、错误日志、清理过程等。


`Shunan Xiang and Li Liu (AWS) `

## 🔧 代码和工具：

## [重塑：Postgres 的零停机模式迁移工具](https://postgresweekly.com/link/118967/web)
一个用 Rust 编写的实验性工具，用于在 Postgres 12 及更高版本上以渐进的方式执行复杂的迁移，因此不需要停机。


`Fabian Lindfors `
## [Que 1.0：使用 Postgres 的咨询锁的 Ruby 作业队列](https://postgresweekly.com/link/118968/web)
我们在上面提到了咨询锁，这里是它们的完美用途，通过使用锁来保护作业的状态，为 Ruby 带来更可靠的作业队列功能。


`Chris Hanks `
## [Pgweb：基于 Web 的 Postgres 数据库浏览器/客户端](https://postgresweekly.com/link/118969/web)
一个用 Go 编写的长期建立的客户端，因此零依赖二进制文件很容易在需要的地方构建。 GitHub 存储库。


`Dan Sosedoff `

