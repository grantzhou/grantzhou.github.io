---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2020-8-12
---
### PostgreSQL每周新闻#368 - 2020年8月12日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/368)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/bduujyk1y2kizpzkyo73.jpg)

## [Postgres分页方法](https://postgresweekly.com/link/93239/web)
大多数webapp用户不希望一次看到一个包含数千个项目的列表，因此页码通常被作为一种在易于管理的一组大的查询结果的方法。使用Postgres有几种方法可以实现这一点，但需要进行各种权衡。

`Bruce Momjian `

## [使用pg_stat_statements排查故障](https://postgresweekly.com/link/93240/web)
这里介绍了Kaarel使用pg_stat_statements的排除PostgreSQL故障的故事。

`Kaarel Moppel `

## [[白皮书]AlwaysOn Postgres](https://postgresweekly.com/link/93241/web)
了解如何在PostgreSQL中使用第二象限的BDR技术实现AlwaysOn可用性。AlwaysOn为运行关键业务应用程序的全球PostgreSQL数据库集群提供高达6个9的可用性。

`2ndQuadrant PostgreSQL Products `

## [使用自然完全联接比较SQL中的两个表](https://postgresweekly.com/link/93242/web)
“自然联接是使用两个表的所有共享列名进行联接的语法糖，完全联接可确保我们也能检索到与联接谓词不匹配的列。”

`Lukas Eder `

## [Postgres13引入打印错误堆栈的功能](https://postgresweekly.com/link/93243/web)
postgres13引入了一个简单但有用的功能，在报告错误时将堆栈跟踪记录到服务器日志中。

`Amit Khandekar `

## [Postgres高可用性：考虑因素和候选因素](https://postgresweekly.com/link/93244/web)
这是系列文章中的第一篇，该文章探讨了将高可用性引入Postgres的各种方法。在这里提到了RepMgr、prosoni、PAF和PgPool II。

`Hamid Akhtar `

## [关于postgres13中的分区改进](https://postgresweekly.com/link/93246/web)

`Ahsan Hadi `

## [避免brin索引的陷阱](https://postgresweekly.com/link/93247/web)

`John Porvaznik `

## [面向R用户的Postgres速成课程](https://postgresweekly.com/link/93248/web)
R是一种流行的统计计算环境和语言，因此您可能会发现从中使用Postgres是很有用的。

`Pachá `

## [在Postgres中使用JSONB对象数组](https://postgresweekly.com/link/93250/web)


`Rob Tomlin `
## [超越jsonb？Postgres的通用非结构化数据类型](https://postgresweekly.com/link/93251/web)
Álvaro想知道常规的JSON支持是否足够，Postgres中是否应该有超出它的东西-一种通用的非结构化数据类型，如果你愿意的话。

`Álvaro Hernández `

## [plpgsql_check现在支持跟踪](https://postgresweekly.com/link/93252/web)
plpgsql_check是Pl/pgSQL代码的linter。

`Pavel Stěhule `

## [pgagroal 0.8.0：高性能Postgres连接池](https://postgresweekly.com/link/93254/web)
0.8带来了故障转移和systemd支持。


`Red Hat Inc. `
# 💡本周提示


当您使用NOW（）函数获取当前时间时，您将获得服务器时区中的当前日期和时间。


许多服务器都运行在UTC/GMT上，如果您也将UTC/GMT前后的时间使用规范化，那么一切都很好，但是一旦出现不匹配（无论是应用程序和数据库服务器之间，还是其他方面），事情就可能出问题，因此需要更具体一些。


NOW（）返回带时区的时间戳（在Postgres或YugabyteDB中称为timestamp），但如果您有一个普通的timestamp[without time zone]列并将NOW（）放入其中，则时区信息会自动删除：


```
=# create table test
      (a int primary key, b timestamp without time zone);
    
=# select now(), pg_typeof(now());
    
                now            |    	pg_typeof    	 
-------------------------------+--------------------------
 2020-05-06 16:44:03.917735-07 | timestamp with time zone
(1 row)


=# insert into test values
    (1, '2020-05-06 16:44:03.917735-07');
    
=# select * from test;
    
 a |         	b         	 
---+----------------------------
 1 | 2020-05-06 16:44:03.917735
(1 row)

=# show timezone;
  TimeZone
------------
US/Pacific
```


我们可以看到“b”列丢弃了时区。这意味着存储的结果是错误的，因为它不尊重用户将存储的纯时间戳值理解为UTC值的约定。


我们可以通过在时区“utc”使用now（）来解决此问题，如下所示：


```
=# insert into test values
  (2, (now() at time zone 'utc'));
  
=# select * from test;
  
 a |         	b         	 
---+----------------------------
 1 | 2020-06-10 19:38:22.859175
(1 row)
```


**🗓即将举办的Postgres活动**
