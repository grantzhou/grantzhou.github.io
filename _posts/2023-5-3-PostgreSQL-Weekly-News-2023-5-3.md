---
layout: post
title: PostgreSQL 每周新闻 2023-5-3
---
### PostgreSQL每周新闻#504 - 2023年5月3日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/504)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,w_524,h_127/e_make_transparent/co_white,e_outline:7/bmhxbsirg1zkckgnwcor.png)
## [“我们最讨厌的 Postgres 部分”](https://postgresweekly.com/link/139047/web)
我们通常会对这样的标题的评论文章愤世嫉俗，但这篇文章是由安迪·帕夫洛 (Andy Pavlo) 合着的。 他和 Bohan Zhang 声称 Postgres 的多版本并发控制方法“很糟糕”，他们详细说明了原因。


`Bohan Zhang and Andy Pavlo (Ottertune) `
## [Postgres 16 中的 LZ4 和 ZSTD pg_dump 压缩](https://postgresweekly.com/link/139049/web)
LZ4 和 Zstandard 是在 Postgres 16 中添加到 pg_dump 的另外两种压缩方法。LZ4 提供速度，但 zstd 可以显着减少压缩转储的大小，如此处所示。


`Pavlo Golub `
## [Hydra：AWS Redshift 的开源替代品？](https://postgresweekly.com/link/139046/web)
这是神话般命名的公司（由 Heroku 的 Joseph Sciarrino 和 Jonathan Dance 创立）背后的代码库，它构建了一个柱状、矢量化的 Postgres，显示出一些令人印象深刻的加速。 数据仓库太贵了，所以让我们高度关注这个项目。


`Hydra `
## [了解并行查询的运行方式](https://postgresweekly.com/link/139053/web)
如果查询的执行策略可以分为多个部分，可以由多个 worker 同时执行，那么性能就会得到提升。 这篇文章解释了影响并行查询运行的基础知识和一些配置设置。


`Muhammad Ali (Stormatics) `
## [Docker 和 Postgres 的“突然死亡”的故事](https://postgresweekly.com/link/139061/web)
听起来比实际情况更病态，但 Laurenz 有一个有用的故事，讲述了客户在 Docker 容器中运行时遇到的 Postgres 崩溃问题。

`Laurenz Albe `
## [psql 提示和技巧](https://postgresweekly.com/link/139062/web)
介绍 psql 及其使用方法，尽管这对我来说总是很有帮助的。


`Ryan Booz `
## [加密 ZFS 和 Ubuntu 22.04 LTS 上的 Postgres 15](https://postgresweekly.com/link/139063/web)


`MANISH R JAIN`
## [在 Amazon Athena 和 Amazon RDS for PostgreSQL 之间加入历史数据](https://postgresweekly.com/link/139064/web)


`DEEPAK SHARMA (AWS)`
## [如何在 Ubuntu 23.04 上将 Postgres 14 升级到 15](https://postgresweekly.com/link/139065/web)


`PAOLO MELCHIORRE`
## [perst 1.3：用于 Postgres 数据的即时 RESTFul API](https://postgresweekly.com/link/139066/web)
它有点像更成熟的 PostgREST，但它是用 Go 而不是 Haskell 编写的（这里有更多的比较）。


`pREST Team `
