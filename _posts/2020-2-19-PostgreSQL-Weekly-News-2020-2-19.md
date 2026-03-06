---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2020-2-19
---
### PostgreSQL每周新闻#343 - 2020年2月19日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/343)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/stjqbsburp6eg7cn5ehl.jpg)

## [pg_flame：一个解释EXPLAIN ANALYSE插件](https://postgresweekly.com/link/84085/web)
从stdin读取JSON查询计划，并将flamegraph HTML的HTML写入stdout。如果你想保持简单，可以通过Docker使用。

`Marcus Gartner `

## [发布的Postgres 12.2、11.7、10.12、9.6.17、9.5.21和9.4.26](https://postgresweekly.com/link/84086/web)
每一个主要的Postgres产品都会得到一个更新来修复一个关键的安全问题，以及各种小错误的修复。这也是Postgres9.4的最后一个版本，现在9.4已经“寿终正寝”。

`PostgreSQL Global Development Group `

## [Postgres与MySQL中的可重复读取隔离级别](https://postgresweekly.com/link/84088/web)
默认情况下，Postgres和MySQL在事务中使用不同级别的隔离。在一个正在运行的事务中，Postgres在提交后将看到其他事务所做的更改，而MySQL使用“repeatable read”，其中查询结果在整个事务中保持一致。不过，还有比这更重要的一点，这篇文章巧妙地向我们展示了它是如何工作的。


`Daniel Vérité `
## [从Postgres迁移到CockroachDB的体会](https://postgresweekly.com/link/84089/web)
我们喜欢Postgres，但我们更喜欢一个故事，所以听一下这位工程师从Postgres转向CockroachDB时的经历。

`Karl Seguin `

## [认知vacuum](https://postgresweekly.com/link/84090/web)
autovacuum乎运行良好，但当autovacuum遇到问题时时，你y应该怎么样去解决问题？罗伯特解释了这种情况以及如何解决它。

`Robert Haas `

## [利用pg_setting查看你的Postgres配置](https://postgresweekly.com/link/84091/web)
如果你想知道Postgres的默认配置有什么问题。pg_settings视图为您提供了一个有关当前情况的权威视图。


`Luca Ferrari `
## [压缩wal归档的原因与方法](https://postgresweekly.com/link/84092/web)
为什么压缩wal归档变得越来越重要，以及如何做到这一点。


`Jobin Augustine `
## [Postgres Vision 2020-提前购买鸟票](https://postgresweekly.com/link/84093/web)
Postgres大会将于今年6月22日至24日在波士顿举行。


`EnterpriseDB `
## [cloudfs_fdw：用于访问云文件系统上文件的外部数据包装器](https://postgresweekly.com/link/84094/web)
具体来说，它在S3或HTTP上处理CSV、JSON、Excel和ODF文件。


`Ernst-Georg Schmid `
## [Schemalint：Postgres模式的Linter](https://postgresweekly.com/link/84095/web)
一个linter，允许您在诸如大小写或列类型之类的问题上引发错误（因此，更像是ESLint而不是基本的格式化程序）。


`Kristian Dupont `
## [wal2json：用于提取变更集的JSON输出插件](https://postgresweekly.com/link/84096/web)
每个事务（或元组）都会生成一个JSON对象，其中包含用于更新的新元组和旧元组。


`Euler Taveira de Oliveira `
# 💡本周提示


想快速查看数据库有多大吗？您可以在单个查询中执行此操作：


```
select pg_size_pretty(pg_database_size('n2'));

 pg_size_pretty 
----------------
 446 MB
(1 row)
```


n2是数据库名称。或者，如果您愿意，可以获取您可以在服务器上访问的所有数据库的结果，如下所示：


```
select name, pg_size_pretty(pg_database_size(datname)) as size
postgres-#   from pg_database;
      name  |  size   
-----------+---------
  postgres  | 7079 kB
 template1 | 7079 kB
 template0 | 6969 kB
        n2        | 446 MB
```


如果您想通过查看特定的表或索引大小来深入了解，请回到我们在第294期中更深入的提示。

**🗓即将举办的Postgres活动**

- [PgConf India](https://postgresweekly.com/link/84100/web)（2月26日至28日，印度班加罗鲁）
- [Postgres Conference 2020](https://postgresweekly.com/link/84097/web)（3月23日至27日，美国纽约）
- [Nordic PgDay 2020](https://postgresweekly.com/link/84101/web)（3月24日芬兰赫尔辛基）
- [pgDay Paris 2020](https://postgresweekly.com/link/84102/web)（3月26日，法国巴黎）
- [Swiss PGDay 2020](https://postgresweekly.com/link/84104/web)（6月18日至19日，瑞士）
- [Postgres Ibiza 2020](https://postgresweekly.com/link/84301/web)（6月25日至26日，西班牙伊比沙岛）
