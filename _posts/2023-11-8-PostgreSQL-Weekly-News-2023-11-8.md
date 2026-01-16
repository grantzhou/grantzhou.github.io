---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2023-11-8
---
### PostgreSQL每周新闻#529 - 2023年11月8日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/529)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/cnztjdobei13tdsxzjxr.jpg)
## [Postgres加密：可用选项](https://postgresweekly.com/link/147410/web)
当谈到加密时，您只能使用开箱即用的普通 Postgres，但可以使用从硬件到 Postgres 扩展（例如 pgsodium ）或应用程序提供的各种数据安全层级防御。这篇文章提供了一个简短的概述，并引发了有关该主题的广泛的黑客新闻讨论。


`Matt Palmer `
## [在同一个表上使用多个触发器](https://postgresweekly.com/link/147413/web)
如果在同一个表上部署多个触发器会发生什么情况？多个触发器按什么顺序触发？Hans-Jürgen 沉迷于他平常的一些实验来找出答案！


`Hans-Jürgen Schönig `
## [使用 Epsio 流式传输 PostgreSQL 查询](https://postgresweekly.com/link/147409/web)
通过将 Epsio 插入数据库来提高最复杂查询的性能。每当基础数据发生变化时，Epsio 就会不断为您定义的查询准备和更新结果，而无需重新计算整个数据集。


`Epsio `
## [为 Postgres 编写存储引擎：一种内存中表访问方法](https://postgresweekly.com/link/147414/web)
Phil 对这篇杰作进行了最好的总结： “本周我一直在努力了解替代存储引擎的 Postgres 表访问方法。特别具有挑战性，因为文档非常稀疏，并且存在很少的最小实现。我把我的方法写下来了！”


`Phil Eaton `
## [Timescale 推出动态 PostgreSQL](https://postgresweekly.com/link/147417/web)
大胆声称是“数据库的下一代发展”，这最终是对 Timescale 的 Postgres平台的一项创新，但仍然是一项有趣的创新。动态 PostgreSQL提供了一致的性能基准，但可以在预定义的范围内即时扩展计算——他们将这种模型称为“购买基础，租用峰值”。


`Freedman and Godeke (Timescale) `
**本周摘要：**
*   📅pgDay Paris 2024已开始征集演讲者 - 该活动将于 2024 年 3 月在法国巴黎举行，提交截止日期为 12 月 22 日。


*   🇫🇷我们也借此机会记住Postgres是法国政府官方推荐的。Postgres 万岁！


*   🇳🇴就在巴黎 pgDay的前几天，北欧 pgDay 2024将于明年 3 月在挪威奥斯陆举行，他们的 CFP 也开放。


*   🎧《Citus Con 之路》播客邀请 Dimitri Fontaine 和 Vik Fearing讨论是否每个数据问题都可以或应该用 SQL 解决。如果您是那种考虑使用 PL/pgSQL 进行Advent of Code的人，那么这就是为您准备的。


*   ✍️Andrew Atkinson 从曼哈顿回来，并与我们分享PGConf NYC 2023 的回顾。


## [SQL 范围界定出奇的微妙和语义化](https://postgresweekly.com/link/147424/web)
🤯Justin 向我们展示了一组非常简单的 SQL 查询，并要求我们预测它们将返回什么。如果你答对了，我会感到惊讶。有趣地观察一些可能不直观（但标准化）的 SQL 行为。


`Justin Jaffray `
## [Timescale 如何将 Postgres 扩展至 350 TB 以上（每天新增 10B 条记录）](https://postgresweekly.com/link/147425/web)
特别是针对他们的新Insights数据库可观察性工具。


`ROB KIEFER (TIMESCALE)`
## [SUPABASE 和 POSTGRES MAX LYNCH中的 Easy 行级安全 (RLS) 策略](https://postgresweekly.com/link/147426/web)


`MAX LYNCH `
## [如何在 WSL2 安装 Postgres 和 pgAdmin](https://postgresweekly.com/link/147427/web)


`ANDRAZ `
## [基于 Kubernetes 的 pgAdmin 教程](https://postgresweekly.com/link/147428/web)


`TRISTEN RAAB `
## [pgext：一个裸露的、最小的 Postgres 扩展](https://postgresweekly.com/link/147429/web)
而且看不到 Rust！这是一个基于 C 的小型扩展模板，它提供了被视为可用的 Postgres 扩展的最低限度。


`Phil Eaton `
## [DoltgreSQL：具有版本控制概念的 Postgres 兼容数据库](https://postgresweekly.com/link/147430/web)
Dolt是一个历史悠久的 Go 支持的数据库，提供“git数据”类型的分支、克隆、合并等体验，但使用 MySQL 有线协议。DoltgreSQL 提供相同的功能，但通过 Postgres 有线协议 - 万岁！


`Daylon Wilkins `
## [PGLoader：用于迁移到 Postgres 的数据加载工具](https://postgresweekly.com/link/147433/web)
一种历史悠久的数据加载工具，支持并行性，可以加载可能部分错误但不会停止（可能\copy）的数据。最近在MySQL 到 Postgres 的迁移故事中提到了这一点。


`Dimitri Fontaine `
## [Credcheck 2.3](https://postgresweekly.com/link/147435/web)
 - 在用户创建期间自动检查凭据。


## [FerretDB 1.14.0](https://postgresweekly.com/link/147436/web)
 - 它看起来像 MongoDB，但后面有 Postgres。


## [asyncpg 0.29.0](https://postgresweekly.com/link/147437/web)
 - Python 中 asyncio 的 Postgres 客户端库。


## [Sequelize 6.34.0](https://postgresweekly.com/link/147438/web)
 - 功能丰富的 Node.js ORM。 



# 💡本周提示


**🗓即将举办的Postgres活动**
