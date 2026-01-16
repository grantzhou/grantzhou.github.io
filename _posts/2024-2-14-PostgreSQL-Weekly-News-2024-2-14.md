---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-2-14
---
### PostgreSQL每周新闻#542 - 2024年2月14日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/542)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/tg37ghcxv1nev4za1jd3.jpg)
## [Postgres 16 查询规划器/优化器的新增功能](https://postgresweekly.com/link/151246/web)
当 Postgres 新版本发布时，查询规划器的改进很少成为头条新闻，但 Postgres 16 获得了一些重大改进，这些改进增强了我们今天的所有查询。 David 介绍了最近的 10 项优化，包括 Postgres 15 与 16 查询计划，并向我们展示了改进的方式和时间。


`David Rowley `
## [使用 AI 自动优化您的 RDS 或 Aurora Postgres 数据库](https://postgresweekly.com/link/151245/web)
需要帮助优化 Postgres 旋钮、查询、索引和 autovacuum？ OtterTune 是您的人工智能数据库副驾驶，可以提高性能、降低成本并保持数据库健康。获得三个数据库的 30 天免费试用。


`OtterTune `
## [PostgreSQL 16.2、15.6、14.11、13.14 和 12.18 已发布](https://postgresweekly.com/link/151248/web)
所有受支持的版本均获得更新以修复各种错误以及一个安全漏洞，其中物化视图的所有者可以让更高权限的用户运行与该漏洞相关的代码查看更高级别的视图（现在所有用户确定的代码都以视图所有者的身份运行，正如其本来的意思）。


`PostgreSQL Global Development Group `
## [pg_analytics：将 Postgres 转变为快速 OLAP 数据库](https://postgresweekly.com/link/151283/web)
ParadeDB 人员的一些有趣的工作。 pg_analytics是一个扩展，可以显着加速 Postgres 中的分析查询处理，而无需采用 OLAP 数据库。


`ParadeDB `
**本周摘要：**
*   📗Andrew Dunstan 撰写了PostgreSQL 16 Administration Cookbook的简短评论，这是 Packt 出版的一本书，有五位 合著者。


*   📊Robert Haas最近对 Postgres 贡献者的分析，其中公司和机构对 Postgres 贡献最多：EDB、AWS 和 Crunchy Data 占据首位。


*   Cybertec 的 Christoph Berg 分享了他（主要是面向 Postgres）的 FOSDEM 2024 经验。


## [psql使用和连接到 Postgres.pg_service.conf](https://postgresweekly.com/link/151251/web)
忘记如何连接到您的 Postgres 服务？告别psql -h并欢迎.pg_service.confPostgres 的连接服务文件。


`James Blackwood-Sewell (Timescale) `
## [pgEdge](https://postgresweekly.com/link/151255/web)
📢免费的pgEdge分布式 Postgres DB，具有 3 节点主动-主动集群和跨 3 个区域的一键配置。前 500 名免费 T 恤。


`'Perfect resolution, excellent audio, no lag'. Try Tuple for free today, no credit card required.`
## [（貌似合理）使用 PostGIS 生成随机地理：Fluviation](https://postgresweekly.com/link/151253/web)
地理空间的东西往往超出了我的理解范围，但我喜欢看到它。很棒的帖子，有视觉效果。


`Dian M Fay `
## [pg_graphql 1.5：为 Postgres 带来 GraphQL 支持](https://postgresweekly.com/link/151258/web)
从现有 SQL 模式反映 GraphQL 模式，让任何 GraphQL 客户端通过 GraphQL 查询数据库，无需额外的服务器、进程或库。通过和添加了对偏移分页的支持。firstoffset


`Supabase `
## [pgmeminfo：调查内存使用情况的新扩展](https://postgresweekly.com/link/151260/web)
Pavel 展示了他的新扩展，该扩展提供了对 Postgres 内部内存使用统计信息的扩展访问，包括有关 Postgres 内部管理内存的信息。


`Pavel Stěhule `
## [pgagroal-cli 获得 JSON 输出支持](https://postgresweekly.com/link/151261/web)
pgagroal是 Postgres 的高性能连接池，现在支持 JSON 输出，这对于自动化场景和其他集成来说非常方便。


`Luca Ferrari `
## [TimescaleDB 2.14.0](https://postgresweekly.com/link/151264/web)
 - 扩展中 Postgres 的时间序列功能。此版本允许您随时更改现有压缩超表的压缩设置。


`PostGIS patch releases: v3.4.2, 3.3.6, 3.2.7, 3.1.11, 3.0.11, and 2.5.10.`


# 💡本周提示


**🗓即将举办的Postgres活动**
- [pgDay 巴黎 2024 年（3 月 14 日）](https://postgresweekly.com/link/151266/web)🇫🇷 - 您可以在 Twitter或Mastodon 上关注他们以获取更新。
- [PostgreSQL@SCaLE21x（3 月 14 日至 15 日）](https://postgresweekly.com/link/151269/web)🇺🇸 - 作为SCaLE 21x的一部分，在加利福尼亚州帕萨迪纳举行的为期两天、两场赛道的活动。
- [FOSSASIA 峰会 PGDay（4 月 9 日）](https://postgresweekly.com/link/151271/web)🇻🇳 -  2024 年 FOSSASIA PGDay在越南河内举行，作为更广泛的FOSSASIA 峰会的一部分。
- [2024 年德国 PostgreSQL 会议（4 月 12 日）](https://postgresweekly.com/link/151272/web)🇩🇪 - 一次迭代在慕尼黑举行。
- [2024 年 Postgres 会议（4 月 17 日至 19 日）](https://postgresweekly.com/link/151273/web)🇺🇸 - 在加利福尼亚州圣何塞举行。CFP还有几天就开放了！
- [2024 年芝加哥 PGDay（4 月 26 日）](https://postgresweekly.com/link/151275/web)🇺🇸 - 非营利性社区运营会议系列的一部分。时间表刚刚公布。
- [PGConf.BE 2024（5 月 7 日）](https://postgresweekly.com/link/151276/web)🇧🇪 - 比利时哈斯罗德。他们正在征集发言人。
- [2024 年 PostgreSQL 开发大会“pgconf.dev”（5 月 28 日至 31 日）](https://postgresweekly.com/link/151278/web)🇨🇦 - 今年在加拿大温哥华举行。
- [POSETTE（6 月 11 日至 13 日）](https://postgresweekly.com/link/151279/web)POSETTE 以前称为 Citus Con，是由 Microsoft Postgres 团队组织的免费虚拟开发者活动。
- [2024 年瑞士 PGDay（6 月 27 日至 28 日）](https://postgresweekly.com/link/151280/web)🇨🇭 - 为期两天的会议，主要以英语进行演讲，但也有一些以德语进行演讲。
- [PGConf NYC 2024（9 月 30 日至 10 月 2 日）](https://postgresweekly.com/link/151281/web)🇺🇸 - 在纽约市举行的为期 3 天的会议，承诺将充满用户故事和最佳实践。CFP 开放至六月。
