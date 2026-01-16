---
layout: post
title: PostgreSQL 每周新闻 2023-6-7
---
### PostgreSQL每周新闻#509 - 2023年6月7日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/509)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,w_430,h_100/e_make_transparent/co_white,e_outline:7/xyflkz7n00elwtgja9ne.png)
## [使用 Hyperloglog 的高压缩度量存储](https://postgresweekly.com/link/140616/web)
postgresql-hll是将HyperLogLog 算法引入 Postgres 的扩展。HyperLogLog 是一种概率算法，可以有效地估计大型数据集中不同值的数量，以一点点精度换取显着的时间和内存节省。


`Christopher Winslett `
## [什么是 Postgres“模式”](https://postgresweekly.com/link/140619/web)
术语模式在数据库世界中有多种含义，但在 Postgres 模式中是命名容器，可以包含其他命名对象，如表、数据类型和函数，有点类似于命名空间。


`Hans-Jürgen Schönig `
## [❤️ Postgres](https://postgresweekly.com/link/140615/web)
您需要一个像您一样热爱 Postgres 的数据库提供商。我们会处理所有麻烦 - 监控、备份、HA、灾难恢复，因此您不必这样做。想要惊人的支持？当您有问题时，我们会在场。


`Crunchy Bridge `
## [PgBouncer/Postgres兼容性指南](https://postgresweekly.com/link/140620/web)
PgBouncer是一种流行的连接池，但并非所有 Postgres 功能都适用于它。如果您正在尝试调试 PgBouncer 问题，那么这篇文章适合您，并且这篇文章试图让您更轻松地浏览更广泛的文章。


`JP Camara `
## [SQL配方：与邻居进行比较](https://postgresweekly.com/link/140628/web)
如果您需要计算记录与前一个或下一个记录之间的差异，LAG()窗口函数适合您。Anton 为我们提供了一些使用示例。（如果你错过了我们上周对他关于窗口函数的采访，它在第 508 期的底部。）


`Anton Zhiyanov `
## [Azure 上 Postgres 的 OpenAI 的未来](https://postgresweekly.com/link/140630/web)
ChatGPT 支持插件作为一种为流行的聊天机器人/LLM 提供数据以制定回复的方式。这篇文章解释了广泛的概念，并展示了插件和存储嵌入与 pgvector 的组合如何开辟新的查询机会。


`Krishnakumar Ravi (Microsoft) `
## [SchemaSpy：轻松构建数据库文档](https://postgresweekly.com/link/140633/web)
一种长期存在的工具，可分析数据库的元数据、模式和其他信息，以帮助您通过 HTML 报告可视化、检查和理解您的数据模型。


`SchemaSpy `
## [[开源]专栏，矢量化的Postgres](https://postgresweekly.com/link/140634/web)


`HYDRA `
## [pgsql-ast解析器11.1:一个简单的Postgres SQL解析器](https://postgresweekly.com/link/140635/web)
一个基于 TypeScript 的 SQL 语法解析器，可以为大多数查询生成类型化的 AST（不支持 PL/pgSQL）。它被用作作者的pg-mem 项目的一部分，这是一个用于 Node 和浏览器的迷你内存中 Postgres 克隆。


`Olivier Guimbal `
## [Goxygen 0.4：用于JavaScript项目的Go后端生成器](https://postgresweekly.com/link/140637/web)
一种工具，用于设置一个新的基于 Go 的项目，前端使用 Angular、React 或 Vue，并使用 Docker 和 Docker Compose 文件使其全部运行。支持 Postgres、MySQL 或 MongoDB 作为数据库


`Sasha Shpota `
# 💡本周提示


**🗓即将举办的Postgres活动**
