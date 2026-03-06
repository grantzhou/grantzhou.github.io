---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2019-10-23
---
### PostgreSQL每周新闻#328 - 2019年10月23日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/328)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/jiagvjutiltfsgdchttw.jpg)
## [如何使用pg_receivewal用以避免发生事务缺失](https://postgresweekly.com/link/78798/web)
pg_receivewal（以前的pg_receivexlog）实时传输postgres服务器或集群的预写日志，可最大限度的避免数据丢失。


`Laurenz Albe `
## [Postgis 3.0.0:Postgres的地理空间对象](https://postgresweekly.com/link/78799/web)
在未来很长一段时间内，postgis 3.0将流行的postgres空间扩展引入postgres 12，将栅格支持移到单独的扩展中，并通过并行化显著提高性能（这里有更多介绍）。

`PostGIS Developers `



## [PostgreSQL 12的自动故障转移](https://postgresweekly.com/link/78801/web)
pg_auto_failover是postgres集群自动故障转移的扩展，其背后的团队正在思考如何将其升级到支持postgres 12。


`Microsoft `
## [基于postgis的陆地约束点网格生成](https://postgresweekly.com/link/78803/web)
如果你还没有使用过postgis，这是一个很赞的教程。


`Alex S Korban `
## [使用sql进行日期的格式化](https://postgresweekly.com/link/78804/web)
日期和时间类型常常会给sql带来挑战，因此最好有一些教程来总结使用它们的各种方法。


`Lori Brok `
## [从Amazon Aurora PostgreSQL发送通知](https://postgresweekly.com/link/78805/web)
作为托管服务，Amazon Aurora限制您访问扩展，迫使您直接从与Postgres兼容的数据库实现发送通知。那么，数据库作业完成后，如何获取通知？这是怎么做的。


`Rajeshkumar Sabankar and Santhosh Kumar Adapa `
## [e-maj 3.2.0：一种记录和回滚表更新的方法](https://postgresweekly.com/link/78806/web)
e-maj记录对（您选择的）表执行的更新，并允许您随意取消/回滚此类更新。v3.2引入了postgres 12支持。


`Dalibo `
## [PGBouncer 1.12.0:Postgres的连接池](https://postgresweekly.com/link/78807/web)
1.12包括对SCRAM支持的修复，以改进与较新Postgres版本的互操作性。

`PgBouncer `



## [aquameta：一个完全在postgres中构建的实验性web开发平台](https://postgresweekly.com/link/78809/web)
我非常喜欢为正确的工作使用正确的工具，但是这是一个有趣的项目。aquameta中的应用程序“完全表示为关系数据”。


`Aquameta `




**🗓即将举办的Postgres活动**
- [pgDay Santiago](https://postgresweekly.com/link/78810/web)（10月29日，智利圣地亚哥）-面向所有级别的PostgreSQL用户，为每个人提供会谈和与同行见面的机会。
- [PG Down Under](https://postgresweekly.com/link/78811/web)（11月15日，澳大利亚悉尼）-本年度澳大利亚邮政会议的第二次出游。
- [PgConf.Russia](https://postgresweekly.com/link/78812/web)（2020年2月3日至5日，俄罗斯莫斯科）-一天的辅导和两天的三次平行会谈。
- [PGConf India ](https://postgresweekly.com/link/78813/web)（2020年2月26日至28日，印度马哈拉施特拉邦班加罗鲁）-一个专门的培训日和一个多轨道两天会议。
- [pgDay Paris 2020](https://postgresweekly.com/link/78814/web)（2020年3月26日，法国巴黎）-在同行中了解更多关于世界上最先进的开源数据库的信息。
