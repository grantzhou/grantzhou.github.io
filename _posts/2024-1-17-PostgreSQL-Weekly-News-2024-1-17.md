---
layout: post
title: PostgreSQL 每周新闻 2024-1-17
---
### PostgreSQL每周新闻#538 - 2024年1月17日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/538)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/efoegvdhvcam6sdo1f6h.jpg)
## [在 500 行 SQL 中实现 GPT](https://postgresweekly.com/link/150059/web)
当一篇文章自称演示“在 PostgreSQL 中作为单个 SQL 查询的完整 GPT2 实现” '，您知道您将踏上一段艰难的旅程。大型语言模型中涉及的算法可以用SQL重新实现吗？ （它不会很快取代 ChatGPT，但本文中的最终查询非常引人注目..）


`Quassnoi `
## [Postgres 17 的 ALTER TABLE 更改生成表达式的命令](https://postgresweekly.com/link/150060/web)
当您 CREATE 一个表时，您可以定义通过表达式自动生成的生成列。如果您稍后想要更改此类表达式，Postgres 17 将以ALTER COLUMN ... SET EXPRESSION的形式给出答案。


`Hubert depesz Lubaczewski `
## [❤️Postgres](https://postgresweekly.com/link/150058/web)
您需要一个像您一样热爱 Postgres 的数据库提供商。我们将处理所有麻烦 - 监控、备份、HA、灾难恢复，因此您无需担心。想要惊人的支持吗？当您有疑问时，我们会随时为您服务。


`Crunchy Bridge `
## [Postgres 16 的 pg_query 简介](https://postgresweekly.com/link/150062/web)
pg_query 很长站立的独立库（带有 Ruby、Rust 和 Go 绑定），用于将 SQL 查询转换为解析树。这个新版本基于 Postgres 16，支持 SQL/JSON，现在也可以在 Windows 上运行。


`Fittl & Mijalkovic (pganalyze) `
## [使用预加载的库优化 Postgres 函数](https://postgresweekly.com/link/150064/web)
借助扩展，可以用多种不同的语言编写 Postgres 函数，但需要在需要时加载这些扩展 — session_preload_library 可用于在连接启动时预加载库，从而节省宝贵的毫秒时间。


`Hans-Jürgen Schönig `
**本周摘要：**
*   📘 Henrietta Dombrovskaya 宣布出版第二版PostgreSQL 查询优化 由 Apress 提供。


*   这有点像“信息转储”。目前，Takayuki Tsunakawa 已一直致力于新的 Postgres wiki 页面：'操作备忘单.'它汇集了来自各种 Postgres 博客的智慧和链接，主题涉及安全性、可扩展性和数据库结构等广泛主题。


*   📅 PgConf․dev 2024 的 CFP 已结束，但您现在可以报名参加今年 5 月 28 日至 31 日在加拿大温哥华举行的活动.


*   📅 在其他活动新闻中，FOSSASIA PGDay 2024 将于今年 4 月在越南河内举行。 其 CFP 开放时间还有两周。


*   React + Postgres =🤯


*   Pavel Luzanov 浏览一下最新的 PG Commitfest 如果您想了解未来 Postgres 版本的众多调整中的一些。


*   Tembo 宣布全面推出 Tembo Cloud， 他们的托管 Postgres 平台。


## [等待 Postgres 17：增量基础备份](https://postgresweekly.com/link/150074/web)
 ▶ 逐步了解 Robert Haas 致力于 Postgres 17 开发分支的增量备份功能。 （带有文字记录的 6 分钟视频。）


`Lukas Fittl `
## [密码加密而不泄露凭据](https://postgresweekly.com/link/150075/web)
日志和代理有时会给您的系统安全带来意想不到的漏洞，但您可以使用预先哈希的版本通过网络处理用户密码。


`Sehrope Sarkuni `
## [postmaster.pid 文件解释](https://postgresweekly.com/link/150076/web)
一个有着悠久历史的短文件。


`Greg Sabino Mullane `
## [Procrastinate 1.1：适用于 Python 的基于 Postgres 的任务队列 ](https://postgresweekly.com/link/150077/web)
适用于 Python 3.8+ 的分布式任务处理库，使用 Postgres 来存储任务定义、管理锁和分派任务。它可以在同步和异步代码以及 Django 应用程序中使用。Github仓库。


`Jablon and Lemoine `
## [Steampipe：使用 SQL 查询您的云服务](https://postgresweekly.com/link/150079/web)
使用 SQL 查询甚至联接超过 100 个 API 来自 Airtable、AWS、Heroku、Slack 和 Stripe 等提供商，以及 Reddit 和 Hacker News 等社交媒体网站。它是开源 (AGPL)，现在有扩展可以使用它来自 Postgres。


`Steampipe `
## [pg_back 2.2.0：一个简单、彻底的 Postgres 备份工具](https://postgresweekly.com/link/150083/web)
用于将数据库转储到文件的工具，包括角色、服务器参数等，格式为你的选择。此新版本增加了对使用 AGE 进行加密的公钥和私钥的支持、一些错误修复和示例Dockerfile以及其他配置以简化在 Kubernetes 上的部署。


`Nicolas Thauvin `
## [pgcopydb 0.15 ](https://postgresweekly.com/link/150084/web)
 - 服务器之间的涡轮增压pg_dump|pg_restore。


## [GoBackup 2.8](https://postgresweekly.com/link/150085/web)
 - 用于云数据库备份的 Go 支持的 CLI 工具。


## [pg-mem 2.8.1](https://postgresweekly.com/link/150086/web)
 - JS 中的实验性内存中 Postgres 模拟


## [Hasql 1.6.4](https://postgresweekly.com/link/150087/web)
 - 适用于 Haskell 的快速 Postgres 客户端库。


## [plpgsql_check 2.7.2](https://postgresweekly.com/link/150088/web)
 - PL/pgSQL linter。


## [pg_partman / PostgreSQL](https://postgresweekly.com/link/150089/web)
 - 分区管理器 5.0.1



# 💡本周提示


**🗓即将举办的Postgres活动**
