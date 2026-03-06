---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-4-3
---
### PostgreSQL每周新闻#549 - 2024年4月3日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/549)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/bwlp6dezovelszoib7z4.jpg)
## [安息吧 Postgres 维护者 Simon Riggs](https://postgresweekly.com/link/153258/web)
我们非常悲伤地告诉大家，Postgres 贡献者（也是多本 Postgres 书籍的作者）Simon Riggs在英国杜克斯福德机场的一次坠机事故中丧生。核心团队也表达了自己的敬意，并提到了他的贡献，包括时间点恢复、热备用和同步复制。他在 12 月的 PGConf EU 上发表了最后一次演讲，主题是▶️ Postgres 的未来 20 年。


`Josh Berkus et al. `
## [为 Postgres 101 做贡献：初学者的经验](https://postgresweekly.com/link/153263/web)
我最近看到一些人抱怨弄清楚如何为某些开源项目做贡献有多么困难，所以如果您也是 Postgres 的用户，那么 Elizabeth 提交补丁并获得批准的经验将非常有用。


`Elizabeth Christensen `
## [使用 Crunchy Bridge 优化数据库性能](https://postgresweekly.com/link/153257/web)
 使用 Crunchy Bridge 提升 Postgres 性能！YNAB 的 IOPS 提高了 30%，成本降低了 10%。无缝扩展，继续使用原始 Postgres，并优化支出。在 YNAB 案例研究中了解更多信息。


`Crunchy Bridge `
## [控制 WAL 文件增长](https://postgresweekly.com/link/153264/web)
对 Postgres 中的预写日志子系统的简要介绍，包括查看检测 WAL 文件积累所需的关键监控事项。


`RapidLoop / pgDash `
**本周摘要：**
*   David Wheeler 继续致力于增强 Postgres 扩展分发生态系统——现在他想知道：PGXN v2 的服务和工具应该用 Go 还是 Rust 编写？


*   Infisical 的 Tony Dang 撰写了有关他的团队从 MongoDB 到 Postgres 的“大迁移”的文章。


*   📅 POSETTE是微软一年一度的在线 Postgres 活动，CFP 仅开放 4 天。


*   思考Postgres 如何占领数据库世界。


*   🤡 我没有看到很多以 Postgres 为主题的愚人节尝试，但Supabase 尝试了其新的、新颖的纸质备份系统..😅


## [journald以及 Postgres 中的 Syslog 日志记录](https://postgresweekly.com/link/153271/web)
使用 journald 和 syslog 日志记录与 Postgres 并不是一个新想法，但 Laurenz 认为应该有更多的人尝试一下，因此整理了这个基本教程： “我将我的 PostgreSQL 实例切换到 syslog 日志记录，我想我不会再切换回来了。”


`Laurenz Albe `
## [为什么 Figma 要用 Postgres 来重新设计轮子？](https://postgresweekly.com/link/153272/web)
仔细研究 Figma 的自定义分片解决方案，包括动机和未来预测。


`Denis Magda `

## [使用 Rust 构建托管 Postgres 服务：第 1 部分](https://postgresweekly.com/link/153277/web)
稍微了解一下 Tembo 的幕后情况。


`Adam Hendel `


## [DoltgreSQL 0.5](https://postgresweekly.com/link/153280/web)
 - 版本控制的 Postgres - Dolt的 Postgres 风格版本 ，一个受 Git 启发的数据库。


## [PGlite 0.1.1](https://postgresweekly.com/link/153282/web)
 - 轻量级 Postgres 以 WASM 形式打包到浏览器、Node.js、Bun 和 Deno 的 TypeScript 库中。现在支持 Postgres 数组类型。

## [Ora2Pg 24.3](https://postgresweekly.com/link/153283/web)
 - 帮助从 Oracle 迁移到 Postgres 的工具。

## [pg_partman 5.1 & 4.8 ](https://postgresweekly.com/link/153284/web)
 - 分区管理扩展。

## [sqlc 1.26](https://postgresweekly.com/link/153285/web)
 - 从 SQL 生成类型安全的 Go 代码。（包括针对使用输出插件的用户的重要安全修复。）

## [pgmoneta 0.10](https://postgresweekly.com/link/153286/web)
 - 适用于 Node.js 和 TypeScript 的流行 ORM。

## [Prisma 5.12](https://postgresweekly.com/link/153287/web)
 - Go 库将数据从 DB 提取到结构中。

## [scany 2.1.2](https://postgresweekly.com/link/153288/web)
 - Go 库将数据从 DB 提取到结构中。

## [plpgsql_check 2.7.5](https://postgresweekly.com/link/153289/web)
 - PL/pgSQL linter。   



# 💡本周提示


**🗓即将举办的Postgres活动**
- [PGDay at FOSSASIA Summit
 (April 8-9)](https://postgresweekly.com/link/153290/web)🇻🇳 - 作为更广泛的 FOSSASIA 峰会的一部分，在越南河内举行。
- [PostgreSQL Conference Germany 2024
 (April 12)](https://postgresweekly.com/link/153291/web)🇩🇪 - 下一届会议将在慕尼黑举行。
- [PG BootCamp Minsk 2024
 (April 16)](https://postgresweekly.com/link/153292/web)🇧🇾
- [Postgres Conference 2024 (April 17-19)](https://postgresweekly.com/link/153293/web)🇺🇸 - 在加利福尼亚州圣何塞举行。
- [PDXPUG April Meeting (April 18)](https://postgresweekly.com/link/153294/web)🇺🇸 - 在俄勒冈州波特兰举行的 2 小时社区聚会，重点讨论 Postgres 17 中的新功能
- [PGDay Chicago 2024
 (April 26)](https://postgresweekly.com/link/153295/web)🇺🇸 - 非营利性社区运营会议系列的一部分。以下是时间表，以下是Henrietta Dombrovskaya 期待看到的一些演讲。
- [PGConf.BE 2024
 (May 7)](https://postgresweekly.com/link/153298/web)🇧🇪 - 比利时哈斯罗德。
- [PostgreSQL Development Conference 'pgconf.dev' 2024 
 (May 28-31)](https://postgresweekly.com/link/153299/web)🇨🇦 - 今年在加拿大温哥华举行。
- [Prague PostgreSQL Developer Day 2024
 (June 4-5)](https://postgresweekly.com/link/153300/web)🇨🇿
- [POSETTE
 (June 11-13)](https://postgresweekly.com/link/153267/web)🌎 -  由微软 Postgres 团队组织的免费虚拟开发者活动。CFP仅开放四天！
- [Swiss PGDay 2024
 (June 27-28)](https://postgresweekly.com/link/153302/web)🇨🇭 - 为期两天的会议，以英语和德语进行演讲。
- [PGConf NYC 2024
 (September 30-October 2)](https://postgresweekly.com/link/153303/web)🇺🇸 - 纽约市为期 3 天的会议。CFP开放至 6 月。
