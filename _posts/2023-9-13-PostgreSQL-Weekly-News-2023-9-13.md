---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2023-9-13
---
### PostgreSQL每周新闻#521 - 2023年9月13日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/521)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/b1rvqbklldm5oxjiexlx.jpg)
## [解释 Postgres 的“冰山模因”](https://postgresweekly.com/link/144777/web)
“冰山层”是一种常见的图像模因格式，用于展示对特定主题的“深入知识”水平的不断提高，Postgres 去年也有了自己的一种。这篇文章巧妙地介绍了冰山的概念，从水面上的基本想法到“深处”中更神秘的东西（比如臭名昭著的“allballs” ）。这里有很多值得学习和娱乐的东西。


`Aryan Ebrahimpour `
## [pgJQ：现在您可以在Postgres中使用JQ](https://postgresweekly.com/link/144781/web)
JQ是一种流行（且功能强大的）切片，过滤和转换JSON的方式，并且此扩展将其及其相关的语言带入Postgres，以与标准JSONB功能和操作员无缝运行的方式。


`Florents Tselai `
## [Postgres 扩展，只需几分钟](https://postgresweekly.com/link/144776/web)
PolyScale.ai 是一种可加速数据库的高性能数据交付网络。使用智能缓存，它可以提高查询性能，降低延迟，并使数据访问和扩展工程变得轻而易举，无论是在本地还是在边缘。


`PolyScale.ai `
## [为什么人们关心 PostGIS 和 Postgres](https://postgresweekly.com/link/144783/web)
Path to Citus Con 播客的最新一集讨论了 Postgres 最大、最受欢迎的扩展之一的大主题： PostGIS。Paul Ramsey 和 Regina Obe 与 Claire Giordano 一起，Pino de Candia 对空间和地理的所有事物进行了深入研究（至少在 Postgres 方面）。如果您愿意，可以提供书面文字记录。


`Carol Smith (Microsoft) `
## [谁是 Postgres 的“负责人”？](https://postgresweekly.com/link/144787/web)
Bruce 试图回答很多人在遇到 Postgres 时都会遇到的一个问题——谁是控制者？它最终不是一个特定的群体，提交者、核心团队成员、安全团队、各个委员会和其他人都发挥着作用。“那么，谁负责呢？你和社区中的其他人都是如此，”布鲁斯建议道。


`Bruce Momjian `
**本周摘要：**
*   Yugabyte的Denis Magda🐦表明，PostgreSQL和Postgres的名称之间的混淆导致Postgres在DB-Engines排名中的位置较低，否则它应该有。


*   Postgres 的社区行为准则委员会 已发出呼吁，寻求该委员会的新成员，因为该委员会的成员每年都会更新。


*   🐦 Phil Eaton 表示，虽然 Postgres 是一个出色的数据库，但之所以有如此多的新数据库系统不断出现，是因为 Postgres 不太能够快速利用更新的创新。然而，Thomas Munro 回复说，他认为引用的常见问题解答已经过时，并且从长远来看，在 Postgres 中使用线程和异步 I/O 之类的想法是可行的。


## [监控 Postgres 复制](https://postgresweekly.com/link/144793/web)
复制可以帮助您的数据库变得更具弹性，但可能会带来复杂性的成本，需要密切关注复制滞后等问题。


`Hans-Jürgen Schönig `
## [何时考虑在Postgres中进行分区](https://postgresweekly.com/link/144794/web)
表分区可以是扩展数据库的强大工具，但它并不是一种万能的解决方案。


`Soto and Blackwood-Sewell (Timescale) `
## [了解 Postgres 和 Citus 中的分区和分片](https://postgresweekly.com/link/144795/web)
分区与分片帖子，特别探讨了使用 Citus 进行分区和分片的好处。


`Claire Giordano `


`pganalyze`
## [我们曾经将文件存储为base64字符串在Postgres中。](https://postgresweekly.com/link/144797/web)
仅仅因为您可以，并不一定意味着您应该。


`Paul Oms (MailPace) `
## [temBoard 8.1：Postgres 远程控制/仪表板](https://postgresweekly.com/link/144800/web)
用于 Postgres 的 Python 构建的 Web 仪表板和监控系统。您可以在相关服务器上安装代理，然后 temBoard Web 应用程序可以在您喜欢的任何地方运行。


`Dalibo `
## [pgexporter 0.4：Postgres 的 Prometheus Exporter](https://postgresweekly.com/link/144801/web)
现在支持 Postgres 10 到 16 以及Grafana 集成的新文档。还有一个入门指南。


`Red Hat `
## [Ora2Pg 24.1](https://postgresweekly.com/link/144804/web)
↳Oracle 到 Postgres 数据库模式转换器。


## [pg_show_plans 1.1.5](https://postgresweekly.com/link/144805/web)
↳ 获取当前运行的所有 SQL 语句的查询计划。


## [PL/RUST v1.2.5](https://postgresweekly.com/link/144806/web)
↳用 Rust 语言编写 Postgres 函数。


## [PGRX 0.10.0](https://postgresweekly.com/link/144807/web)
↳使用 Rust 构建 Postgres扩展。


## [PLPGSQL_CHECK 2.5](https://postgresweekly.com/link/144808/web)
↳PL/PGSQL代码的linter。


## [PG分区管理器4.7.4](https://postgresweekly.com/link/144809/web)


# 💡本周提示


**🗓即将举办的Postgres活动**
