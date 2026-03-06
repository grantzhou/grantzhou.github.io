---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2020-5-13
---
### PostgreSQL每周新闻#355 - 2020年5月13日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/355)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/v1589300029/pryzuzd84hdzubadddkj.jpg)
## [为什么你不应该手动修改Postgres的数据目录](https://postgresweekly.com/link/88137/web)
当被告知永远不要自行修改Postgres数据目录的内容时你很想问 “为什么？”，那这篇文章你应该读读。 很复杂的。


`Robert Haas `
## [ now（）vs 'NOW'::timestamp vs clock_timestamp（）](https://postgresweekly.com/link/88138/web)
啊，日期和时间，任何应用程序开发人员生命的祸根..以及数据库用户:-)这篇文章探讨了使用 Postgres当前时间管控的用法。


`Hans-Jürgen Schönig `
## [实时编码：Grafana指南101-警报入门](https://postgresweekly.com/link/88139/web)
5月20日加入我们，以了解如何使用Grafana的警报功能来获取有关数据异常的通知，挖掘根本原因并响应关键问题。 分步演示+技巧=更便宜，更灵活的监控


`Timescale `
## [谁在2019年为Postgres开发做出了贡献？](https://postgresweekly.com/link/88141/web)
Robert的年度研究，看看谁对Postgres开发的贡献最大，如果您按添加的代码行，其他人的代码的提交者以及pgsql-hackers列表中的参与者进行排序。


`Robert Haas `
## [关于Postgres 13中改进的（自动）vacuum](https://postgresweekly.com/link/88142/web)
本文概述了在下一主要版本中的Postgres自动vacuum功能的六种改进方案。


`Amit Kapila `
## [Postgres的内部原理](https://postgresweekly.com/link/88143/web)
多年来，我们已将其博客链接了两次，但是如果Bruce Monjian没有看到，那我假设你们中的许多人也没有。 这里有很多令人生厌的内容，但是如果您能了解其中的一些内容，就会学到很多有关Postgres如何开展业务的知识


`Hironobu SUZUKI `
## [网络延迟确实有很大的不同](https://postgresweekly.com/link/88145/web)
尽可能快地查询是很棒的，但是网络延迟也很重要。 汉斯·于尔根（Hans-Jürgen）演示了如何在模拟延迟的情况下衡量其影响。


`Hans-Jürgen Schönig `
## [您的数据就是您的业务](https://postgresweekly.com/link/88146/web)
PGX是一家提供全面服务的数据库咨询公司，专注于在任何平台或托管环境上的PostgreSQL数据系统。


`PostgreSQL Experts, Inc. `
## [PostgreSQL模糊搜索](https://postgresweekly.com/link/88147/web)


`Kevin Alemán `
## [使用DISTINCT ON（来自Ruby）避免进行N + 1查询](https://postgresweekly.com/link/88148/web)
最近，我修复了一个棘手的N + 1查询，并认为我应该写出来与大家分享


`John Nunemaker `
## [Kubernetes中的本地永久磁盘卷和Postgres用法](https://postgresweekly.com/link/88149/web)
2ndQuadrant在Kubernetes 1.17上运行了一些Postgres基准测试，以使用OpenEBS Local PV测试本地永久磁盘卷的性能。


`Gabriele Bartolini `
# 💡本周提示

BETWEEN 和 BETWEEN SYMMETRIC

假设您有一个像这样的基本人员表：

| id 	| name   	| age 	|
|----	|--------	|-----	|
| 1  	| Sam    	| 34  	|
| 2  	| Chris  	| 18  	|
| 3  	| Quinn  	| 52  	|
| 4  	| Lennox 	| 44  	|

如果要返回年龄在25至50岁（含）之间的人员，则可以编写下列查询语句：


```
SELECT * FROM people WHERE age >= 25 AND age <= 50;
```

到目前为止，还算不错，但是您也可以使用BETWEEN运算符来进一步完善：


```
SELECT * FROM people WHERE age BETWEEN 25 and 50;
```

（额外提示：您可以使用NOT BETWEEN获得相反的效果！）


这很棒，并且使内容可读性强，但是如果切换了这些值（例如BETWEEN 50和25）怎么办？ 因为值必须是有序的，所以它不起作用。

使用 BETWEEN SYMMETRIC


```
SELECT * FROM people WHERE age BETWEEN SYMMETRIC 50 and 25;
```

此查询将以正确的顺序放置范围限制，并返回相关的两行。 请注意，尽管这是Postgres特定于BETWEEN的扩展（（主要是！-HSQLDB也支持）），所以这取决于您想达到怎么样的通用性:-)


**🗓即将举办的Postgres活动**
- [Bruce Momjian on 'The Future of Postgres Sharding'](https://postgresweekly.com/link/88151/web) - 五月15/16（根据时区）由中国PostgreSQL协会举办的系列会议中的第一场。
- [Postgres Pulse](https://postgresweekly.com/link/88152/web) - 每周的东部时间上午11点。 每周与Bruce Momjian，Vibhor Kumar等人在EnterpriseDB进行基于Zoom的会议
- [Postgres Vision 2020](https://postgresweekly.com/link/88153/web) - 在6月23日至24日。 多天多次尝试在线进行在线Postgres会议。
