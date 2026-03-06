---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2020-12-9
---
### PostgreSQL每周新闻#385 - 2020年12月9日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/385)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/v1607518322/d1nj838ojgba9lfbq8hr.png)
## [MongoDB到PostgreSQL的无缝迁移](https://postgresweekly.com/link/99941/web)
Coinbase是大型数字货币交易所，因此必须具有扎实的数据基础。 他们在这里分享了从大型跨数据库数据迁移到AWS RDS PostgreSQL的经验教训。


`Alex Ghise (Coinbase) `
## [用Postgres中的2个小正则表达式替换代码行](https://postgresweekly.com/link/99942/web)
我喜欢正则表达式，但是“正则表达式”这个词确实让许多开发人员望而却步。Postgres对他们有用吗？ 是的，史蒂夫在这里展示了一个。

`Steve Pousty `

## [▶️ 未来的数据库体系结构是Postgres兼容的](https://postgresweekly.com/link/99943/web)
在Postgres中使用的语言和工具对提高效率非常重要。12月16日加入我们，参加一个现场技术讲座，了解数据库体系结构如何以及为什么发展是离不开Postgres的。预留你的位置。


`CockroachDB `
## [何时使用超大规模（Citus）扩展Postgres](https://postgresweekly.com/link/99944/web)
Citus Data的Citus现在是Microsoft的一部分（尽管仍然是开源的），并且是横向扩展Postgres的有效方法。 在本文中，克莱尔解释了何时以及为何需要这种功能。

`Claire Giordano (Microsoft) `

## [清理BLOB](https://postgresweekly.com/link/99946/web)
BLOB是SQL标准的二进制字符串类型，与Postgres的bytea方法稍有不同，但无论哪种方式，如果使用BLOB接口（例如通过lo_import）将二进制数据引入数据库，则需要小心，因为导入的数据可能会留在数据库中，即使您认为已将其删除。

`Hans-Jürgen Schönig `

## [利用YugabyteDB中的Postgres聚合函数分析COVID-19数据](https://postgresweekly.com/link/99947/web)
Yugabyte是一个与Postgres兼容的“NewSQL”数据库，下面我们将介绍如何使用SQL函数对冠状病毒统计数据进行线性回归分析。


`Bryn Llewellyn `
## [V4 UUID生成基准](https://postgresweekly.com/link/99948/web)
uuid_generate_v4 与 gen_random_uuid的对战！结果相差很大。


`Shane Husson `
## [想知道你应该如何优化一个特定的查询吗？](https://postgresweekly.com/link/99949/web)
pganalyze使用auto_explain自动收集解释计划。识别慢速顺序扫描、磁盘排序等。

`pganalyze `

## [恢复单个Postgres表](https://postgresweekly.com/link/99950/web)
如果要从转储还原单个表，该怎么办？


`Thomas Vilhena `
## [升级和更新Postgres](https://postgresweekly.com/link/99951/web)
更新（比如从12.0升级到12.1）与升级（比如从12.0升级到13.1）是完全不同的，需要考虑一些工具。


`Hans-Jürgen Schönig `
## [比较批量加载到Postgres的选项](https://postgresweekly.com/link/99952/web)
比较COPY、\copy、file_fdw和pg_bulkload在不同场景下加载624MB CSV数据。


`Muhammad Usama `
## [看一看pgtop，一个Postgres 的top clone](https://postgresweekly.com/link/99953/web)
另一种查看当前正在运行的查询的方法。


`Cosimo Streppone `
## [pgagroal 1.0：面向Postgres的高性能连接池](https://postgresweekly.com/link/99954/web)
有很多特性和承诺，比如速度极快。GitHub repo。

`Agroal `

## [pg shortkey：类似YouTube的短id作为Postgres的主键](https://postgresweekly.com/link/99957/web)
数据库的触发器，允许您使用类似YouTube的URL安全短id（例如oHg5SJYRHA0）作为主键（如果您愿意）。几个月前，我们第一次把这个联系起来，但黑客新闻发现了这个问题，于是一场有趣的讨论随之展开。

`turbo `

## [pg-listen:Postgres 为Node.js 设计的 LESTEN 和 NOTIFY ](https://postgresweekly.com/link/99959/web)
如果你使用Node.js并且希望使用Postgres作为带有通知通道的消息代理，这将有所帮助。（如果您不熟悉这个Postgres特性，本文将有所帮助。）


`Andy Wermke `
# 💡本周提示


**🗓即将举办的Postgres活动**
