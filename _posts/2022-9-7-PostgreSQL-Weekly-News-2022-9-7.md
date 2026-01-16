---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2022-9-7
---
### PostgreSQL每周新闻#470 - 2022年9月7日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/470)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/v8dz1knqoxxajjzdvnll.jpg)
## [📊 如何使用 SQL 绘制 ASCII 条形图](https://postgresweekly.com/link/128373/web)
想看到一个超酷炫的 SQL 查询（你可以花 20 分钟自己研究），它会产生一些可以说非常有用的东西？ 把它变成一个你可以从 psql 中使用的函数可能会很有趣。


`Lukas Eder `
## [从 Postgres 15 推迟了完整的 SQL/JSON 支持](https://postgresweekly.com/link/128374/web)
虽然 Postgres 已经有很多处理 JSON 数据的方法，但 SQL/JSON 更多的是从 SQL 处理 JSON 的标准。 Postgres 支持它的路径语言有一段时间了，但为 v15 带来更完整支持的补丁已经恢复，希望它可以成为明年 v16 的头条功能。 在此处阅读完整的讨论。


`Hubert depesz Lubaczewski `
## [时间序列数据库的内容、原因和方式](https://postgresweekly.com/link/128378/web)
时间序列数据库是增长最快的数据库类别——但它们是什么？ 了解什么是时间序列数据 - 完整的真实示例 - 何时以及为什么“正常”数据库还不够，以及入门方法。

`Timescale `
## [使用 Postgres Dump Manifests](https://postgresweekly.com/link/128379/web)
Postgres Dump Manifests不仅存储数据库中的内容，还存储有关这些数据库的meta数据（以清单的形式）。 为什么这很有趣？ 您可以编辑manifest去影响以后如何恢复此类dump！


`Robert Bernier `
## [Amazon RDS 和 Amazon Aurora 中的并行VACUUM](https://postgresweekly.com/link/128380/web)
不，这不是关于同时在 RDS 和 Aurora 中VACUUM（！），而是关于在这两种服务上使用 Postgres 13+ 的并行操作清理过程。 （但是，这篇文章的大部分内容通常适用于 Postgres。）


`Bhattacharyya and Asadulla Baig (AWS) `
## [Postgres 配置参数的多样性](https://postgresweekly.com/link/128381/web)
PostgreSQL 有很多参数需要配置。 猜猜有多少。 我们不会剧透（这一次），但 Stefanie 已经设法将它们分成 15 组就足够了。 她还提供了一些与他们合作的建议。


`Stefanie Janine Stölting `
## [“错误：nextval：达到序列的最大值”(https://postgresweekly.com/link/128382/web)
使用串行伪类型时的基本建议（用于创建基于整数的自动递增列的方便表示法）。 一个更好的选择是使用 serial8 或 bigserial 来获得 64 位，而不是应该持续你.. 很长一段时间 :-)


`Hans-Jürgen Schönig `
## [如何为 Aurora PostgreSQL 表创建审计跟踪](https://postgresweekly.com/link/128383/web)
Rana 说，您可以在一个表上使用触发器并跟踪另一个表中发生的所有内容，但这会带来太多的性能开销。 AWS Aurora 提供了一种不同的方法，使用 AWS Database Migration Service (DMS) 在单独的数据库实例上创建连续审计日志表。 


`Rana Dutt (AWS) `
## [您的数据库，在边缘](https://postgresweekly.com/link/128384/web)



`PolyScale.ai `
## [深入研究 Postgres 和 OS 内存分配](https://postgresweekly.com/link/128385/web)
很少有人需要深入到这个级别，但是如果你对监视 Postgres 和 Linux 内存分配系统之间的交互感兴趣..


`Frits Hoogland (YugabyteDB) `
## [▶ 与 Andrew Atkinson 讨论 Postgres 和 Ruby](https://postgresweekly.com/link/128386/web)
Ruby 风格的 Postgres 数据库讨论，涵盖约束、捕获不安全迁移和分析查询计划等领域。


`Code with Jason Podcast podcast`
## [Kanel：从 Postgres 生成 TypeScript 接口](https://postgresweekly.com/link/128429/web)
它通过检查实时数据库来工作，有点像反向对象/关系映射器。 GitHub 存储库。


`Kristian Dupont `

