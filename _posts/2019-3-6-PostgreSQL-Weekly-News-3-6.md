---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2019-03-06
---

### PostgreSQL每周新闻#295 - 2019年3月6日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/295)

![pg img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/xljhbftdd3kyllwfmn1x.jpg)

## [PostgreSQL的工具们（回答那些喜欢图形界面的人）](https://rob.conery.io/2019/03/04/postgresql-tools-for-the-visually-inclined/)
为了回应一个[批评Postgres配套工具](https://www.softwareandbooz.com/postgresql-for-a-sql-server-dba-the-tooling-stinks/)的SQL Server DBA，Rob Conery阐述了Postgres（和Unix）与工具相关的文化是如何不同的，以及其优点。

`ROB CONERY`

## [pgCenter的Wait Events Profiler](https://blog.dataegret.com/2019/03/pgcenters-wait-event-profiler.html)
[pgCenter](https://github.com/lesovsky/pgcenter)是一个通过统计数据来监控和故障排除Postgres的流行工具。最近的0.6版本增加了对分析等待事件的支持（基本上是指当Postgres等待事件发生的时候，例如等待IO或获得锁）。

`ALEXEY LESOVSKY`

## [在PostgreSQL环境中诊断和解决性能问题](https://www.quest.com/products/foglight-for-postgresql/?utm_source=none&utm_medium=Direct-External+Online+Advertising&utm_campaign=FY2019_Q4_AMER_DBPerf_CooperPress_FoglightPostgres_Jan_eNewsletter_ADV&utm_term=&utm_content=cooper-press-enewsletter)

![quest_img](https://copm.s3.amazonaws.com/2100ff85.jpg)  
管理基础架构的运行状况。基于Web的仪表板直观地提醒您注意可能影响性能或可用性的问题，清晰的企业级范围视图可帮助您优化整个PostgreSQL环境。[下载免费试用版](https://www.quest.com/products/foglight-for-postgresql/?utm_source=none&utm_medium=Direct-External+Online+Advertising&utm_campaign=FY2019_Q4_AMER_DBPerf_CooperPress_FoglightPostgres_Jan_eNewsletter_ADV&utm_term=&utm_content=cooper-press-enewsletter)

`QUEST SOFTWARE` **赞助商**

## [PostgreSQL项目参与谷歌编程之夏2019（Google Summer of Code 2019）](https://www.postgresql.org/about/news/1925/)
GSoC是Google的一个项目，Google在夏季为参与某些开源项目的大学生提供津贴——Postgres就是其中之一。如果您想参加，请[了解更多信息](https://wiki.postgresql.org/wiki/GSoC)。

`POSTGRESQL全球开发组`

## [如何使用JOIN LATERAL以及为什么你希望这样的原因](https://blog.2ndquadrant.com/join-lateral/)

`ELEIN MUSTAIN`

## [在Postgres 10+中使用PL/pgSQL函数中的并行查询](https://rafiasabih.blogspot.com/2019/03/using-parallelism-for-queries-from-pl.html)
虽然在9.6中引入了并行查询，但直到Postgres 10才能在PL函数中使用它。

`RAFIA SABIH`

## [我和WAL搏斗，WAL赢了：为什么hot_standby_feedback可能会误导](http://richyen.com/replication/postgres/hot_standby_feedback/2019/03/05/i_fought_the_wal.html)

`RICHARD YEN`

## [电子书：如何在Postgres数据库上获得3倍的性能提升](https://pganalyze.com/ebooks/optimizing-postgres-query-performance?utm_source=PostgresWeeklySecondary)
pganalyze团队分享他们的最佳实践经验，通过帮助像Atlassian这样的公司优化他们的Postgres数据库，在过去几年中积累了这些经验。

`PGANALYZE` **赞助商**

## [如何使用Postgres GSSAPI Kerberos身份验证设置Windows Active Directory](https://info.crunchydata.com/blog/windows-active-directory-postgresql-gssapi-kerberos-authentication)
这是非常适合的，如果你需要这样做，这些指导将有所帮助。

`STEPHEN FROST`

## [ShiftLeft如何使用PostgreSQL的TimescaleDB扩展](http://highscalability.com/blog/2018/12/5/how-shiftleft-uses-postgresql-extension-timescaledb.html)
TimescaleDB是Postgres的扩展，可以帮助处理时间序列数据。在这篇文章，您可以了解ShiftLeft如何利用它来获取metrics和漏洞事件数据。

`HIGH SCALABILITY`

## [一个让PostgreSQL的EXPLAIN ANALYZE更易读的工具](https://explain.depesz.com/)
这是一个工具，您可以粘贴EXPLAIN ANALYZE查询的结果，然后得到更易于理解的版本。

`HUBERT DEPESZ LUBACZEWSKI`

# ![_config.yml]({{ site.baseurl }}/assets/img/Tips-icon.png)   本周提示
由Dotadog提供支持

## 如何获得比默认设置更好的Postgres配置

如果您没有使用托管数据库，或者您没有使用sysadmin，那么您可能会使用Postgres的默认内存和缓存设置。这些已经很好了，但只需稍加调整，Postgres就可以更好地利用其环境。

阅读[有关设置的官方文档](https://www.postgresql.org/docs/9.6/runtime-config-resource.html#RUNTIME-CONFIG-RESOURCE-MEMORY)会花费很长的时间！但值得庆幸的是，在线配置生成器可以提供比默认值更好的设置建议，并且只需要一分钟即可完成。

1、可以使用pgtune。填写服务器的操作系统，内存，磁盘类型，并回答其他一些问题，就可以获得建议的主要设置。

![pgtune_img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/ylbj5dq1jdwwrwxhhejz.jpg)  

2、还可以使用pgconfig.org。这个工具深受pgtune的启发，但有一些简洁的附加功能，例如能够并排查看不同类型工作负载的不同设置。

![pgconfig_img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/xaenaqbht3yo9pbudtyq.jpg)  

> 本周提示由Datadog赞助，Datadog是PostgreSQL基础架构、分布式跟踪和日志记录的云监控平台。 开始[免费试用](https://postgresweekly.com/link/59029/web)。

🗓  即将举办的Postgres活动  

 [pgDay Israel 2019 (3月14日，以色列)](https://pgday.org.il/)  
 [Nordic PGDay 2019 (3月19日，哥本哈根)](https://2019.nordicpgday.org/)  
 [PGConf APAC 2019 (3月19日，新加坡)](https://2019.pgconfapac.org/)  
 [pgconf.de 2019 (3月10日,莱比锡)](https://2019.pgconf.de/)  
