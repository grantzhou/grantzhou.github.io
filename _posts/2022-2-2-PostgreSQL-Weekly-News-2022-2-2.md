---
layout: post
title: PostgreSQL 每周新闻 2022-2-2
---
### PostgreSQL每周新闻#440 - 2022年2月2日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/440)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/gpmoyblovpfrdarbqcbw.jpg)
## [时间戳和时区：你需要做什么和不需要知道什么](https://postgresweekly.com/link/119196/web)
试图“揭开” Postgres 日期和时间数据类型的神秘面纱，其深度超出您的想象（这只是两部分系列中的第一部分 第二部分转到持续时间/间隔。）是时候了；-）


`Bryn Llewellyn (YugabyteDB) `
## [为 Postgres 创建一个外部数据包装器](https://postgresweekly.com/link/119198/web)
Postgres 的一大优势在于它通过扩展的可扩展性—。 一种强大的机制，甚至整个公司（例如 Citus Data 或 Timescale）都建立在它们之上。 扩展的一个常见用途是外部数据包装器，它允许 Postgres 与非本地数据格式交互——这篇文章涵盖了制作自己的数据格式所需的知识（注意：前面有很多 C 语言——如果你更喜欢 Rust，请考虑 pgx）。


`Aaron Son (DoltHub) `
## [pganalyze 电子书库：Postgres 优化指南等](https://postgresweekly.com/link/119201/web)
到目前为止，已有超过 10,000 人下载了我们的电子书。 查看我们关于 Postgres 查询优化、有效索引、使用 EXPLAIN 查找缓慢 Postgres 查询的根本原因、高效搜索和日志监控的指南。


`pganalyze `
## [PG 14 和最近的 SCRAM 身份验证更改：您应该迁移到 SCRAM 吗？](https://postgresweekly.com/link/119207/web)
如果您在切换到 Postgres 14 后遇到与密码验证相关的失败，您将在此处了解原因。 简而言之，在较新版本的 Postgres 中默认密码加密使用 SCRAM（自 Postgres 10 起可用）。 这篇文章解释了它是什么以及你为什么要继续使用它。


`Jobin Augustine (Percona) `
## [在 Postgres 14+ 中使用 JSON](https://postgresweekly.com/link/119208/web)
Postgres 的原生 JSON 支持可以追溯到 9.2 版本，但 PG14 中可用的功能与早期相比是一个巨大的飞跃。 Aaron 着眼于一些更现代的功能。


`Aaron Bos `
## [如何使用正则表达式组量词](https://postgresweekly.com/link/119209/web)
正则表达式提供了一种强大而灵活的方式来解析文本，即使它们并不总是最可靠的方式。 尽管如此，作者还是有一些 HL7 V2 数据（一种用于医疗保健的格式）来解析并设法在 Postgres 中使用正则表达式来完成这项工作。


`Selvakumar Arumugam `

## 🔧 代码和工具：

## [Procrastinate：一个基于 Postgres 的 Python 任务队列](https://postgresweekly.com/link/119213/web)
感觉这件事已经投入了很多精力和思考。 也不错的 API。


`Peopledoc `
## [🐘 你一直想要的 Postgres 开发者体验](https://postgresweekly.com/link/119212/web)


`Crunchy Bridge `
## [Pgpool-II 4.3 有什么新功能？](https://postgresweekly.com/link/119210/web)
流行的连接池（以及更多）中间件的 v4.3 实际上在 12 月下降，但这篇文章具体介绍了其中的一些变化。


`Tatsuo Ishii `
## [PostGIS 3.1.5 已发布](https://postgresweekly.com/link/119215/web)
v3.2 已发布，但这是旧分支的错误修复版本。


