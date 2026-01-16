---
layout: post
title: PostgreSQL 每周新闻 2019-02-06
---

### PostgreSQL每周新闻#291 - 2019年2月6日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/291)

![pg img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/d6li9nzua3jpxwctjydp.jpg)

##[PostgreSQL走向 11](https://www.youtube.com/watch?v=MJ_y5Ej-5vE)
来自FOSDEM的Joe Conway的演讲不仅突出了Postgres 11中包含的所有重要新功能，而且还深入了解了一些历史，并期待Postgres 12。 48分钟。

*译者：视频来自油管，访问需要梯子*

`JOE CONWAY`

##[PostgreSQL规模化-数据库Schema无需停机即更改](https://medium.com/braintree-product-technology/postgresql-at-scale-database-schema-changes-without-downtime-20d3749ed680)
Baypree Payments是PayPal公司大量使用Postgres的一个部门，由于提供支付处理服务，因此必须实现零停机。 这里深入探讨了在没有停机的情况下进行架构更新所涉及的所有事情。

*译者：文章来自Medium，访问需要梯子*

`JAMES COLEMAN`

##[保证你获得机器学习工作](https://www.springboard.com/workshops/ai-machine-learning-career-track/?utm_source=postgresweekly&utm_medium=email&utm_content=postgresweekly-1)
利用首个在线机器学习课程，由机器学习专家提供1：1的指导和工作保证。 保证获得机器学习工作，否则退款。

![t pic1](https://copm.s3.amazonaws.com/444751f9.jpg)

`SPRINGBOARD` *赞助商*

##[MailChimp的Mandrill服务经历因交易ID环绕而中断](https://news.ycombinator.com/item?id=19086626)
如果大规模使用Postgres并且与自动清洗设置不完全一致，这是您真正需要注意的事项。 Sentry在2015年经历了类似的中断，并进行了全面的报告。

`黑客新闻`

##[在systemd下使用带有密码短语保护的SSL密钥的Postgres](https://blog.2ndquadrant.com/postgresql-passphrase-protected-ssl-keys-systemd/)
很多人不使用密码短语，但是如果你愿意，当你使用systemd启动Postgres时，怎么能让它工作？

`PETER EISENTRAUT`

##[在Postgres中实现“AS OF”查询](https://www.cybertec-postgresql.com/en/implementing-as-of-queries-in-postgresql/)
许多数据库（例如Oracle）提供“AS OF”查询（a.k.a。'time travel'）。 这篇博客解释了如何在Postgres中模仿类似事情。

`HANS-JÜRGENSCHÖNIG`

##[现已推出：Gartner的“数据库平台即服务权威指南”](https://www.enterprisedb.com/blog/definitive-guide-database-platforms-service)
获取您的报告副本。

`ENTERPRISEDB` *赞助商*

##[Postgres中的64位交易ID会持续多长时间？](https://andreas.scherbaum.la/blog/archives/970-How-long-will-a-64-bit-Transaction-ID-last-in-PostgreSQL.html)
Postgres的MVCC实现意味着它可以一次保留多个版本的数据，从而允许并发事务发生。 这需要维护一组活动的事务ID。
但是意味着TXID环绕可能发生（参见上面的Mandrill故事），那么如果Postgres使用64位id而不是32位呢？ Spoiler：虽然[不太可能改变](https://news.ycombinator.com/item?id=19083745)。

`ANDREAS'ADS'SCHERBAUM`

##[SQL查询的一生](https://numeracy.co/blog/life-of-a-sql-query)
运行SQL语句时会发生什么？ 我们跟踪Postgres处理查询时的每个转换，直到返回结果。

`ERIC FENG`

##[使用pg_repack在线重建Postgres数据库对象](https://www.percona.com/blog/2019/02/04/pg_repack-rebuild-postgresql-database-objects-online/)

`AVINASH VALLARAPU`

# ![_config.yml]({{ site.baseurl }}/images/Tips-icon.png)   本周提示
由Dotadog提供支持
![data dog](https://res.cloudinary.com/cpress/image/upload/v1549285104/cdttwslojuv9zso9nswk.png)

## 本地跨数据库SELECT和INSERT
来自[Alan Au](https://twitter.com/alan_au)的小贴士

您是否曾想从一个本地数据库中选择SELECT并将结果插入另一个？ 您可以使用Postgres自带的dblink扩展来完成此操作。

首先，您需要在两个数据库上设置dblink扩展：

`CREATE EXTENSION dblink;`

然后从本地（或“目标”）数据库运行此类查询：

`INSERT INTO my_table`

`SELECT * FROM dblink（`

`'dbname = my_other_db options = -csearch_path ='，`

`'SELECT some_data FROM my_other_table;'）`

`AS temp（some_data TEXT）;`

请注意，[postgres_fdw](http://www.craigkerstiens.com/2016/09/11/a-tour-of-fdws/)提供了一种更通用和现代的方法来执行类似的操作，特别是如果您想要连接到外部数据库，但dblink可能非常适合您对快速本地作业的需求。

> 本周提示由Datadog赞助，Datadog是PostgreSQL基础架构、分布式跟踪和日志记录的云监控平台。 开始[免费试用](https://postgresweekly.com/link/59029/web)。



