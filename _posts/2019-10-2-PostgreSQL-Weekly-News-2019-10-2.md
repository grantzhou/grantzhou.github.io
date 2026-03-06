---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2019-10-2
---
### PostgreSQL每周新闻#325 - 2019年10月2日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/325)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/v1570014828/zx5lirn5agvejwtdfbwc.png)
## [Postgres 12 RC 1发布，是最终版本么？](https://postgresweekly.com/link/77797/web)
postgresql 12的第一个版本现在可以下载了。最终版本预计将于明天发布。


`PostgreSQL Global Development Group `
## [postgres中透明数据加密的实现](https://postgresweekly.com/link/77799/web)
关于Postgres是否（以及如何）实施TDE的长期讨论的简要更新。简言之，目前工作正在进行中，这个在todo list的任务作有望在Postgres13发布。


`Bruce Momjian `
## [免费电子书：如何在Postgres数据库上获得3倍的性能提升](https://postgresweekly.com/link/77801/web)
了解我们的最佳做法，以优化PASGRESs查询性能，如亚特兰西等客户，以及如何减少从磁盘加载的数据为500倍。


`pganalyze `
## [Hacker Newer讨论…Postgres还是MySQL？](https://postgresweekly.com/link/77802/web)
Hacker Newer要求读者在两种技术之间做出选择，不出所料，Postgres似乎是最受欢迎的。


`Hacker News `
## [介绍phppgadmin 7.12.0](https://postgresweekly.com/link/77803/web)
phppgadmin是一个基于web的postgres管理工具（类似于mysql流行的phpmyadmin）。V7.12.0移动到PHP 7并支持PyGRESs（包括12）的所有当前版本。


`xzilla `
## [Postgis 3.0 Beta 1发布](https://postgresweekly.com/link/77805/web)
Postgist最适合与postgres 12一起使用，它是一个流行的postgres扩展，它可以方便而优雅的处理地理位置信息。


`PostGIS Developers `
## [如何在不长时间锁定并发查询的情况下运行快速alter表](https://postgresweekly.com/link/77806/web)
解决这个难题的有趣办法。


`Hubert depesz Lubaczewski `
## [如何在go中使用postgres](https://postgresweekly.com/link/77807/web)
这里有在Postgres中使用go的丰富经验，包括工具，驱动，日志，监控等。


`Artemiy Ryabinkov `
## [在postgres.conf中调整track_activity_query_size-大小](https://postgresweekly.com/link/77809/web)
默认情况下，postgres最多保留1024字节来跟踪每个查询运行，这可能不足以满足您的监视或日志记录首选项。以下是如何调整所涉及的设置。


`Hans-Jürgen Schönig `
## [同步复制是陷阱吗？](https://postgresweekly.com/link/77810/web)
“我认为，很多人在使用这项技术，并从中获得很少或根本没有好处，甚至有些人因此受损。”


`Robert Haas `
## [使用工具提高查询性能](https://postgresweekly.com/link/77811/web)
基于查询计划，pgMustard为您提供了使查询更快的提示。免费试用。


`pgMustard `
## [与postgres相比，redis存储json块的速度要快多少？](https://postgresweekly.com/link/77812/web)
如果您熟悉RIDS，即内存数据结构存储，让您吃惊的不是它很快，而是redis和postgres之间的用例和优缺点的不同。


`Peter Bengtsson `
## [理解heroku postgres日志语句和常见错误](https://postgresweekly.com/link/77814/web)


`Heroku `
# 💡本周提示

**SELECT的INTERSECT选项**

关系代数和集合论构成了sql的许多基础，并激发了sql的许多特性。这样的一个特性是能够将两个查询的结果相互交叉，从而可以在数学上交叉两个集合：


![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/v1569842492/dcsws9myvjc2yxmm2ltc.png)


例如，假设有一个customers表，其中有一个address_id列指向addresses表中的行。我们要获取两个表中存在的所有地址ID（即，客户记录指向一个地址，并且该地址存在）：


```
SELECT address_id FROM customers
  INTERSECT SELECT id FROM addresses;
```


如果要返回在customers表中引用但在addresses表本身中不存在的地址id，我们也可以进行相反的操作。我们使用except而不是intersect执行此操作：


```
SELECT address_id FROM customers
  EXCEPT SELECT id FROM addresses;
```


注意这里的顺序很重要。我们从客户中选择地址ID，然后存在于地址中的地址将被except删除。如果我们想找到没有被客户引用的任何地址的ID，我们可以旋转查询：


```
SELECT id FROM addresses
  EXCEPT SELECT address_id FROM customers;
```


如果这激起了您的兴趣，Lukas Eder的这篇教程将更详细地介绍更多的例子，并涵盖UNION。


**🗓即将举办的Postgres活动**
- [PostgreSQL Conference Europe 2019](https://postgresweekly.com/link/77817/web)（10月15日至18日，意大利米兰）
- [pgDay Santiago](https://postgresweekly.com/link/77818/web)（10月29日，智利圣地亚哥）
- [PG Down Under 2019](https://postgresweekly.com/link/77819/web)（11月15日，澳大利亚悉尼）-本年度澳大利亚第二次Postgres会议。
