---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2022-3-23
---
### PostgreSQL每周新闻#447 - 2022年3月23日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/447)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/uu4e57imwmrvly2v6zsi.jpg)
## [使用 plprofiler 在 Amazon RDS 或 Aurora 上分析 PL/pgSQL 代码](https://postgresweekly.com/link/121287/web)
plprofiler 是一个 Postgres 扩展，可创建函数和存储过程的性能配置文件。 虽然它可以在任何 Postgres 系统上使用，但它现在可以在 Amazon 的 Postgres 平台上使用，这里是使用它的一个例子（无论是否使用 AWS）。


`Madiwale, Akula and Shaik (AWS) `
## [5 分钟的 Postgres - 关于 Postgres 的新的每周视频系列](https://postgresweekly.com/link/121289/web)
每个星期四，pganalyze 首席执行官 Lukas Fittl 都会发布一段短视频来评论过去 7 天中最值得注意的 Postgres 内容。 订阅我们的 YouTube 频道，享受明天的 5 分钟 Postgres 剧集。


`pganalyze `
## [调整 Postgres 的 max_wal_size 设置](https://postgresweekly.com/link/121290/web)
作者说，max_wal_size 配置参数设置了在日志中触发新检查点的预写日志 (WAL) 大小，该设置会对性能产生深远影响。


`Dave Page (EDB) `
## [对数据库进行分片如何使其更快](https://postgresweekly.com/link/121291/web)
作者是 AWS 数据英雄，也是数据库分片领域的无可争议的专家，他着眼于分片如何仍然是通过分配负载来提高性能的常用方法。 不是 Postgres 特有的，尽管 Notion 最近有一篇关于他们如何对 Postgres 进行分片的帖子。


`Trista Juan Pan `
## [使用 pgTAP 自动化数据库测试](https://postgresweekly.com/link/121295/web)
让您的 pianoPostgres 与 pgTAP 保持一致，这是一套数据库函数，可帮助在 psql 脚本或 xUnit 样式的测试函数中编写 TAP 发出单元测试。


`Josh Tolley `
## [查询参数数据类型和性能](https://postgresweekly.com/link/121297/web)
Laurenz 最近帮助客户解决了一个性能问题，该问题是由于查询参数类型选择不当（使用 JDBC 时）导致查询性能不佳。


`Laurenz Albe `
## [Wix 在构建超级 CI 管道时面临的 6 大挑战](https://postgresweekly.com/link/121298/web)



`Buildkite `
## [数据库设计：使用文档](https://postgresweekly.com/link/121299/web)
这不再是“NoSQL”的时代，但在数据库系统中使用文档模型的想法继续提供一些吸引力。 幸运的是，Postgres 和 JSON 可以让我们访问基于文档的方法，同时仍然保持高效。


`Emre Hasegeli `

## [在 Debian 或 Ubuntu 上安装 Pgpool-II](https://b-peng.blogspot.com/2022/03/pgpool-debian.html)

`Bo Peng `

## [PLV8 3.1：JavaScript V8 引擎，但适用于 Postgres](https://postgresweekly.com/link/121301/web)
Postgres 的可扩展性意味着您不必单独使用 PL/pgSQL 来向数据库添加更多功能 — 您可以使用 Perl 或 JavaScript 来代替。 PLV8 使后者发挥作用。 文档。


`plv8 team `
## [DBeaver 22：通用数据库工具](https://postgresweekly.com/link/121303/web)
用 Java 编写，这是一个长期存在的、开源的、跨平台的数据库工具，用于构建和运行查询、查看表、执行计划等。


`DBeaver Team `
## [Directus：使用实时 GraphQL + REST API 包装 SQL 数据库](https://postgresweekly.com/link/121304/web)
一个基于 Node.js 的开源系统，可以充当 Postgres、SQLite、MySQL、Oracle 和其他 SQL 数据库的前端，并提供现代仪表板 、客户端以及 REST 和 GraphQL API。


`Directus `
