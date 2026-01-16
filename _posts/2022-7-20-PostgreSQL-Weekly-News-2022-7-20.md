---
layout: post
title: PostgreSQL 每周新闻 2022-7-20
---
### PostgreSQL每周新闻#464 - 2022年7月20日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/464)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/v1658323472/dzjcs83w9wc1pcds23iz.jpg)
## [PostgreSQL 14 Internals: The Book](https://postgresweekly.com/link/126389/web)
这本书是为那些“在使用数据库时不会满足于黑盒方法”的人而写的，作者是我们最喜欢的一位深入研究 Postgres 特性的技术作者。第一部分现在以160 多页的 PDF 格式提供。


`Egor Rogov `
## [\gexec在psql： Postgres 高级用户实践？](https://postgresweekly.com/link/126391/web)
如果您使用eval过 Python 或 JavaScript 等语言，\gexec提供类似的机制psql并打开一些有趣的方式来动态生成和运行集体查询。（如果你喜欢历史，这里是pgsql-hackers 列表中原始公告中该功能的一些背景。） 


`Julian Markwort `
## [2022 年 PostgreSQL 现状报告的初步见解](https://postgresweekly.com/link/126393/web)
PostgreSQL 现状调查最近结束。在我们不断深入研究结果的同时，请阅读我们新博客文章中的第一个见解，并分享您的电子邮件，以便在完整报告发布时获得通知


`Timescale `
## [在Postgres 15 中使用DISTINCT](https://postgresweekly.com/link/126400/web)
使用DISTINCTwithSELECT通过指定表达式从结果中消除“重复”行。我们仍处于Postgres 15的 beta 阶段，但这篇文章展示了如何SELECT DISTINCT通过并行化提高性能。


`Robert Bernier `
## [BRIN 索引何时获胜？](https://postgresweekly.com/link/126402/web)
BRIN 和 BTree 索引的易于理解的比较，并解释了尽管 BRIN 相对简单（例如，非常大的仅插入表），但何时以及为什么 BRIN 最有意义。


`Paul Ramsey `
## [Postgres 的视图和物化视图是如何工作的](https://postgresweekly.com/link/126403/web)
还有，重要的是要注意， “它们如何影响 TimescaleDB 连续聚合。” 无论您是否使用 Timescale，这都是对视图的有用介绍，这些视图优雅地解释了为什么 Timescale 必须创建适合时间序列用例的额外机制。


`David Kohn (Timescale) `
## [使用 PostgreSQL 将内部工具构建速度提高 10 倍](https://postgresweekly.com/link/126404/web)
l,null,"en


`Retool `
## [Postgres vs SQLite with Litestream](https://postgresweekly.com/link/126405/web)
▶尽管我很喜欢 Postgres，但 SQLite 对于许多用例来说绝对是完美的。Litestream是一种工具，可让您将 SQLite 更改流式传输到其他位置，从而开辟更多机会。它的创建者 Ben Johnson 在这个节目中谈到了它，并将整体方法与 Postgres 进行了比较。 


`Ship It Podcast podcast`
# 💡本周提示


**🗓即将举办的Postgres活动**
