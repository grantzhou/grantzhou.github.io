---
layout: post
title: PostgreSQL 每周新闻 2022-4-6
---
### PostgreSQL每周新闻#449 - 2022年4月6日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/449)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/ovuvbxdhf0pftb24xu5l.jpg)
## [Postgres 如何选择用于查询的索引](https://postgresweekly.com/link/121864/web)
每当一篇博客文章的日期为 4 月 1 日时，我都会立即处于紧张状态，但 Lukas 深入而直接地观察 Postgres 的查询计划器如何工作，这并不是胡闹。这直接进入 Postgres 的源代码（！），但也涵盖了一个实际示例，说明为什么这是一个有用的知识，可以放在你的口袋里。


`Lukas Fittl `
## [将时间戳映射到 'Bins'date_bin](https://postgresweekly.com/link/121866/web)
不知何故，到目前为止，我错过了 Postgres 14 中的这个简洁的添加。date_bin是将提供的时间戳放入从指定来源开始的一组间隔内定义的 bin/bracket/zone 的函数。它为长期存在的人提供了更精细的控制date_trunc。


`Hans-Jürgen Schönig `
## [应用程序性能被您的数据库阻止？](https://postgresweekly.com/link/121868/web)
扩展 Postgres 数据库可能意味着成本和复杂性。PolyScale 为 Postgres 提供即插即用的无服务器边缘缓存。无需编写代码或部署基础架构，即可在几分钟内实现全球扩展。


`PolyScale.ai `
## [Postgres 容器应用程序：在 Postgres中轻松部署应用程序](https://postgresweekly.com/link/121876/web)
一个有趣的开发。Postgres 容器应用程序提供了一种机制，用于从 Postgres 内部启动基于容器的应用程序，该应用程序本身直接与 Postgres 数据库一起运行。这是 Crunchy 特有的，但考虑其用例很有趣。


`Craig Kerstiens (CrunchyData) `
## [用pg_stat_statement识别postgres性能瓶颈](https://postgresweekly.com/link/121877/web)
pg_stat_statements一次又一次地作为最常用的 Postgres 扩展之一出现，这是有充分理由的：它非常适合调试性能问题。它现在默认在 Timescale Cloud 上可用，但您当然也可以在非 Timescale 系统上使用它。


`Ryan Booz (Timescale) `
## [快速技巧：在表中的每个字段中搜索](https://postgresweekly.com/link/121879/web)
您想在表中查找一个值，而不关心它在哪一列中！该怎么办？您可以选择一行作为单个值并将其转换为字符串..


`Hubert depesz Lubaczewski `
## [只需 5 分钟即可了解最新的初创公司、技术和编程](https://postgresweekly.com/link/121880/web)
l,null,"en


`TLDR Newsletter `
## [整理VACUUM](https://postgresweekly.com/link/121881/web)
看，我们不能一个月不以某种方式进行吸尘。它不像极端熨烫那样有趣，但是确保根据数据库的要求正确配置清理过程的演练更有用.. Shaun 在这里介绍了它。


`Shaun Thomas (EDB) `
## [Postico：macOS 的原生 Postgres 客户端](https://postgresweekly.com/link/121884/web)
它是一个商业产品（带有试用版），但具有优雅的原生 macOS 美学。七年前我们第一次联系到它，但喜欢查看项目仍然运行良好


`Egger Apps `
## [一个 Postgres Wire-Compatible SQLite 代理](https://postgresweekly.com/link/121885/web)
如果你可以使用 Postgres 客户端工具.. 但是在远程服务器上使用 SQLite 数据库呢？这就是这个有趣的实验提出的想法


`Ben Johnson `
# 💡本周提示


**🗓即将举办的Postgres活动**
