---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-3-27
---
### PostgreSQL每周新闻#548 - 2024年3月27日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/548)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/zlzorvhbggampjojw3kb.jpg)
## [从 Postgres 表中恢复已删除的数据](https://postgresweekly.com/link/153008/web)
事务和备份涵盖了大多数情况，但是您能否对被视为从表中删除的数据执行类似于“取消删除”的操作？ 使用 pg_dirtyread，你可以做很多事情，如果做不到这一点，你甚至可以深入挖掘 WAL..


`Christoph Berg `
## [Postgres 会改变它的许可证吗？](https://postgresweekly.com/link/153010/web)
最近宣布 Redis 将放弃 BSD 许可证，转而采用双重“可用源”和 SSPL 许可证，这让人们感到担忧。 Postgres 是否容易受到类似举措的影响？ [当然不会](https://postgresweekly.com/link/153012/web)。


`Jonathan Katz `
## [如何使用 CP-SAT 求解器自动选择 Postgres 索引](https://postgresweekly.com/link/153007/web)
了解支持 pganalyze Index Advisor 3.0 的约束编程模型。 Lukas Fittl 和 Philippe Olivier 的这段技术深入探讨（56 分钟视频）是使用 CP-SAT 求解器推荐 Postgres 索引的幕后花絮。


`pganalyze `
## [介绍 pgzx：使用 Zig 创建 Postgres 扩展](https://postgresweekly.com/link/153014/web)
是的，我们上周链接到了 pgzx，但似乎我们操之过急，因为现在有一个合适的发布帖子，其中包含用于创建准系统扩展和运行的 C 与 Zig 示例 使用 Zig 构建扩展的优势。


`Golubenco and Siering (Xata) `

**本周摘要：**

*   Redgate Software 的 [Grant Fritchey](https://postgresweekly.com/link/153016/web) 是本周 PostgreSQL 本周人物的受访者。


*   [POSETTE 的 CFP](https://postgresweekly.com/link/153017/web) 仍然开放到 4 月 7 日，如果您想发言，Claire Giordano 会很高兴。


*   🗓️ 在其他活动方面，[2024 年瑞士 PGDay](https://postgresweekly.com/link/153018/web) 将于今年 6 月举行，[其 CFP](https://postgresweekly.com/link/153019/web) 开放至 4 月 8 日。


*   Postgres 平台 Tembo 现在利用 [FerretDB](https://postgresweekly.com/link/153020/web) 提供类似 [MongoDB 的托管服务](https://postgresweekly.com/link/153021/web)，称为 [MongoAlternative](https://postgresweekly.com/link/153022/web)。


## [检查您的权限](https://postgresweekly.com/link/153023/web)
“如果您依靠 PostgreSQL 权限系统来阻止角色运行函数（并访问其他对象），请确保您知道默认权限是什么，并相应地进行调整。”


`Christophe Pettus `
## [如何使用 plpgsql_check 识别语义问题](https://postgresweekly.com/link/153024/web)
plpgsql_check 是一个用于静态分析 Postgres PL/pgSQL 过程代码的工具。


`Pattanayak, Rout, Kumar and Borse (AWS) `
## [解析 PostGIS：计算距离](https://postgresweekly.com/link/153026/web)
Paul 深入解说 PostGIS 的距离计算实现。


`Paul Ramsey `

## [从 Heroku Postgres 过渡到 AWS EC2：分步方法](https://postgresweekly.com/link/153027/web)


`MUHAMMAD ALI`
## [了解 Postgres 的 Planner：简单扫描路径与计划](https://postgresweekly.com/link/153028/web)


`CARY HUANG`
## [使用Neon的Postgres数据库分支和PostgreSQL匿名器](https://postgresweekly.com/link/153029/web)
🥸在带有蒙版PII的类似生产的环境中发展。


**本周机密：**

* 🥸 使用 [Neon 的 Postgres 数据库分支和 PostgreSQL Anonymizer](https://postgresweekly.com/link/153029/web) 在具有屏蔽 PII 的类似生产环境中进行开发。

* 📢 免费的 [pgEdge](https://postgresweekly.com/link/153030/web) 分布式 Postgres DB，具有 3 节点主动-主动集群和跨 3 个区域的一键配置。 [前 500 名免费 T 恤](https://postgresweekly.com/link/153030/web)。


## [Slonik v38：Node.js 的复杂 Postgres 客户端](https://postgresweekly.com/link/153031/web)
一个经过“实战测试”的框架，提供严格的类型、详细的日志记录、抽象重复代码模式、防止不安全行为以及丰富的调试体验。


`Gajus Kuizinas `
## [MobilityDB 1.1：地理空间轨迹数据管理和分析平台](https://postgresweekly.com/link/153032/web)
MobilityDB 基于 Postgres 和 PostGIS 构建，旨在处理移动中的事物，因此提供可以存储和查询的地理空间轨迹。 [GitHub 存储库](https://postgresweekly.com/link/153033/web)。


`Université libre de Bruxelles `
## [Nano ID for PostgreSQL 2.1](https://postgresweekly.com/link/153034/web)
小型、URL 友好、唯一的字符串 ID 生成器。

## [QuestDB 7.4](https://postgresweekly.com/link/153035/web)
Java 驱动的时间序列数据库，具有 Postgres 有线协议兼容性。

## [FerretDB 1.21](https://postgresweekly.com/link/153036/web)
类似于 MongoDB，但位于 Postgres（或 SQLite）之上。

## [postgres-meta 0.80](https://postgresweekly.com/link/153037/web)
用于管理 Postgres 的 RESTful API。

