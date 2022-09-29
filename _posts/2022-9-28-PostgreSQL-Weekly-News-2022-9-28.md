---
layout: post
title: PostgreSQL 每周新闻 2022-9-28
---
### PostgreSQL每周新闻#473 - 2022年9月28日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/473)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/v1664368643/rkwxkdhjtmn08a20bjne.jpg)
## [pgsqlite：将 SQLite 数据库导入 Postgres 的 Python 模块](https://postgresweekly.com/link/129295/web)
Postgres 很流行，但 SQLite 几乎是通用的。 bit.io 是一个新的 Postgres 平台，意识到了这一点，并创建了 pgsqlite 作为一种将 SQLite 数据库快速导入 Postgres 的方法。 这篇文章重点介绍了这一过程中涉及的一些困难。


`Adam Fletcher (bit) `
## [Postgres 15 中的 ICU 功能](https://postgresweekly.com/link/129298/web)
ICU（Unicode 的国际组件）是一套库，用于可靠地处理各种与 Unicode 相关的文本操作。 Postgres 从版本 10 开始支持 ICU 对列进行选择性排序/排序，但 Postgres 15 将允许您为整个数据库指定 ICU 排序规则。


`Peter Eisentraut `
## [使用完全托管的 Postgres DBaaS 加速开发](https://postgresweekly.com/link/129299/web)
世界领先的 Postgres 提供商现在在云中完全托管。 在我们管理和支持关键 Postgres 任务的同时，解放您的团队进行创新。 没有人比 EDB 做得更好。 点击了解更多。


`EDB BigAnimal `
## [监听和通知：Postgres 的客户端通知系统](https://postgresweekly.com/link/129300/web)
与其让许多客户端一遍又一遍地查询数据库以获取相同的信息，不如让他们等待，然后在信息准备好时发送信息呢？ LISTEN、NOTIFY 和触发器可以让您在某些用例中走得更远。


`Hans-Jürgen Schönig `
## [TimescaleDB 如何“增强” Postgres](https://postgresweekly.com/link/129301/web)
重要的是要注意这篇文章来自 TimescaleDB 的开发人员，他们给出了一些非常大胆的数字，但要点是展示仅将 TimescaleDB 引入标准 Postgres 设置如何能够提高性能，即使 你不是在做时间序列的工作。


`Ryan Booz (Timescale) `
## [▶ 使用 Psycopg 3.1 优化 Python 中的查询吞吐量](https://postgresweekly.com/link/129305/web)
Psycopg 3 是一个现代、功能丰富的 Python Postgres 适配器，在 v3.1（在此处发布）它支持管道模式，因此可以同时向 Postgres 发送大量查询，无需等待。


`Lukas Fittl `
## [使用 pg_stat_statements 进行查询优化](https://postgresweekly.com/link/129308/web)
每周我们都会阅读最新的 PostgreSQL Person of the Week 采访，感觉大多数时候被采访的人都将 pg_stat_statements 作为他们最喜欢的扩展，所以如果你不经常使用它，那么值得熟悉一下 ..（这篇文章可以追溯到 2021 年，但我们当时错过了它。）


`Kat Batuigas `
## ['Preferred Types'](https://postgresweekly.com/link/129310/web)
一个有趣的探索，一个奇怪的查询结果导致 Laetitia 在确定数据类型及其对某些类型的偏好时发现 Postgres 的行为中的一个怪癖。


`Laetitia Avrot `
## [为 Postgres 扩展处理 Heroku 的新 heroku_ext Schema](https://postgresweekly.com/link/129311/web)
Heroku 云平台进行了一项更新，要求在特殊的 heroku_ext 模式中创建所有扩展。 Heroku 刚刚发布了一个关于这个问题的常见问题解答（尽管需要登录才能看到它。）


`Justin Searls `
## [TOAST 的实际应用](https://postgresweekly.com/link/129313/web)
TOAST（超大属性存储技术）是 Postgres 出于效率原因将大列移动（甚至压缩）到与表的其余部分不同的位置的一种方法。


`Daniel Westermann `
## [PDF 下载：了解 Kubernetes 概念和实现](https://postgresweekly.com/link/129315/web)

`Linode `
## [使用 Ruby 和 Timescale 创建连续聚合](https://postgresweekly.com/link/129316/web)
连续聚合使用物化视图来连续和增量地刷新查询，以便只计算已更改的数据，而不是整个数据集。


`Jônatas Davi Paganini `

