---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2022-11-9
---
### PostgreSQL每周新闻#480 - 2022年11月9日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/480)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,e_trim,w_500,h_100/e_make_transparent/co_white,e_outline:7/xh5y6qe2tcrjx1vxyfer.png)
## [Postgres 15，十亿次交易](https://postgresweekly.com/link/131321/web)
上周 B-tree 和 BRIN 索引展开较量，现在是 2017 年的 Postgres 10 vs Postgres 15！Kaarel 对它们进行了十亿次交易压力测试，并进行了一些观察，包括 v15 提高了存储效率。


`Kaarel Moppel `
## [Postgres内部人员术语](https://postgresweekly.com/link/131323/web)
想让自己看起来像 Postgres 中的一员吗？不？嗯，辛苦了，Paul 来这里是为了让我们快速了解元组、TOAST、关系、页面等等。如果您想更进一步，您知道 Postgres 也有官方词汇表吗？


`Paul Ramsey `
## [Dynaboard：专为开发人员打造的Pro Code Web App Builder](https://postgresweekly.com/link/131325/web)
在协作式代码转发 WYSIWYG 环境中构建高性能公共和私有 Web 应用程序。


`Dynaboard `
## [在查询中重写OR到UNION](https://postgresweekly.com/link/131326/web)
几年前，Laurenz 写了一篇关于避免OR出于性能原因，而不是依靠UNION基于方法的文章。但它总是赢家吗，为什么 Postgres 不为此进行优化呢？劳伦兹有一些答案。


`Laurenz Albe `
## [LISTEN和NOTIFY如何促进应用层的高可用性](https://postgresweekly.com/link/131334/web)
Shaun 研究了一些替代方法来使用触发器在虚构的社交网络上发送通知，例如依靠 Postgres 的内置发布/订阅功能（通过NOTIFY和 LISTEN）将工作外包给外部守护进程。


`Shaun Thomas `
## [使用JSON函数浏览餐厅评论](https://postgresweekly.com/link/131336/web)
我总是欢迎使用 Postgres 的 JSON 查询功能的实际例子。这从基础开始，然后转向诸如在单个查询中创建餐厅评级直方图之类的事情。


`Francesco Tisiot `
## [什么是PostgreSQL Commitfest以及如何贡献](https://postgresweekly.com/link/131337/web)
一种经过时间考验的贡献核心 Postgres 代码的方法。


`Pavel Borisov (Supabase) `
## [Orafce 4.0:Postgres的Oracle兼容性函数](https://postgresweekly.com/link/131338/web)
Orafce 实现了一些来自 Oracle 的功能，这些功能可能对迁移到 Postgres 的用户有用。v4.0 放弃了对 Postgres 9.6 和 10 的支持，并合并到orafce_sql中，这是 Oracle 的 DBMS_SQL 接口的 Postgres子集。


`Orafce `
## [使用Datadog的OOTB仪表板监控自定义PostgreSQL度量](https://postgresweekly.com/link/131340/web)


`Datadog `
## [pg_builder 2.1.0：PHP中的Postgres查询生成器](https://postgresweekly.com/link/131341/web)
奇怪的是，它包含 Postgres 查询解析器的部分重新实现，并通过将查询与 AST 相互转换来工作。v2.1 拥有改进的 Postgres 15 支持。


`Alexey Borzov `
# 💡本周提示


**🗓即将举办的Postgres活动**
