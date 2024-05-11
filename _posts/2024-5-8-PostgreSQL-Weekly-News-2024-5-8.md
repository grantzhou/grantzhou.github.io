---
layout: post
title: PostgreSQL 每周新闻 2024-5-8
---
### PostgreSQL每周新闻#554 - 2024年5月8日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/554)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/x8gpgirt7ztu4v89idmy.jpg)
## [在 PostgreSQL 上进行黑客攻击确实很难](https://postgresweekly.com/link/154778/web)
Robert 多年来一直是 Postgres 的前十大提交者之一，但他反思了对 Postgres 做出贡献的过程有多么令人生畏，即使对于经验丰富的开发人员来说也是如此。这篇文章有很多有趣的见解。


`Robert Haas `
## [pgvector v0.7 中的新功能](https://postgresweekly.com/link/154779/web)
我们上周提到了 pgvector 令人兴奋的 v0.7 版本，但这里对其新功能进行了适当的总结，包括额外的向量类型和新的距离函数。


`Pavel Borisov `
## [POSETTE 日程表已出炉：Postgres 2024 活动！](https://postgresweekly.com/link/154777/web)
POSETTE 日程表已出炉，内容丰富，包括 4 场主题演讲和 38 场演讲，由来自社区和 Postgres 团队的 44 位优秀演讲者发表。POSETTE 是微软 Postgres 团队组织的免费虚拟活动。记住日期：6 月 11 日至 13 日！


`Microsoft `
## [了解 Postgres 模式和search_path](https://postgresweekly.com/link/154781/web)
Dolt 数据库的开发人员在 MySQL 方面拥有丰富的经验，但他们已开始将Doltgres构建为提供 Postgres 兼容性的版本控制数据库。这意味着要了解 Postgres 的模式。这是一个很好的入门知识，也展示了search_path，有点类似于操作系统在解析查询中的非限定名称时的PATH 变量。


`Zach Musgrave `
**本周摘要：**
*   本周PostgreSQL 人物的采访对象是 Nazir Bilal Yavuz，他在微软从事 Postgres 工作。


*   Michael Christofides 与 Claire Giordano 在Path To Citus Con播客中讨论了▶️他的背景、EXPLAIN以及对 Postgres 文档的看法。


*   🇨🇭 2024 年瑞士 PGDay 的时间表已经公布——它将于今年 6 月 27 日至 28 日在苏黎世附近举行。


*   Azure 团队上个月对Azure PostgreSQL 灵活服务器进行了快速更新，涉及一些新功能和更新。


*   Reddit 上有一场关于UUID 与整数序列的优缺点的有趣讨论。


## [如何不更改 Postgres 列类型](https://postgresweekly.com/link/154789/web)
ALTER TABLE .. ALTER COLUMN在某些情况下是可以的，但需要注意一些限制，特别是在生产中。幸运的是，有一些替代方法。


`Radim Marek `
## [使用 Postgres 的应用程序的通知程序模式](https://postgresweekly.com/link/154790/web)
Brandur 是 Postgres 内置发布/订阅功能的忠实粉丝。


`Brandur Leach `
## [cursor_tuple_fraction和 PostgreSQL JDBC](https://postgresweekly.com/link/154791/web)
Laurenz 的第一句话就吸引了我： “这篇文章就像是一个失败的故事。”


`Laurenz Albe `
## [13个提高插入性能的技巧](https://postgresweekly.com/link/154792/web)
📄 前五条适用于 Postgres，其余的则特定于 TimescaleDB 时间序列数据扩展/系统。


`MICHAEL FREEDMAN (TIMESCALE)`

## [将 IvorySQL 引入 Neon Autoscaling 平台](https://postgresweekly.com/link/154793/web)
📄  IvorySQL是一个由 Postgres 提供支持的数据库，可提供 Oracle 兼容性。


`David Zhang`

## [转换陷阱：Oracle 到 Postgres 迁移中的隐式转换](https://postgresweekly.com/link/154795/web)


`DEEPAK MAHTO`


## [📄使用 pgEdge 分布式 PostgreSQL CADY MOTYKA (PGEDGE)进行自动 DDL 复制](https://postgresweekly.com/link/154796/web)


## [（双）时态表、PostgreSQL 和 SQL 标准](https://postgresweekly.com/link/154797/web)


`HENRIETTA DOMBROVSKAYA`


## [使用 Postgres 扩展实现饱和算法](https://postgresweekly.com/link/154800/web)
饱和算法是将算术函数的结果限制在一定范围内的概念，从而防止溢出。Adjust 的人们构建了pg-saturation_int，这是一个提供遵循此概念的整数类型的扩展。


`Artur Zakirov `
## [pg_back 2.3.0：一个简单、全面的 Postgres 备份工具](https://postgresweekly.com/link/154802/web)
一个由 Go 提供支持的工具，用于以您选择的格式将您的数据库转储到文件（包括角色、服务器参数等）。


`Nicolas Thauvin `
## [pgdsat：Postgres 数据库安全评估工具](https://postgresweekly.com/link/154803/web)
检查集群上的大约 70 个安全控制，包括来自 CIS 合规基准的所有建议。


`HexaCluster `
## [PG Slot Notify Bot](https://postgresweekly.com/link/154804/web)
⚙️ - 将槽位增长情况通知给 Slack 频道。PeerDB


## [pgAdmin 4 v8.6](https://postgresweekly.com/link/154805/web)


# 💡本周提示


**🗓即将举办的Postgres活动**
