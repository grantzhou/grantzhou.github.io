---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2019-12-11
---
### PostgreSQL每周新闻#335 - 2019年12月11日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/335)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/v1576005477/j9xwnk9klmkl9li75ba1.png)

## [Odyssey1.0：一个可扩展的Postgres连接池](https://postgresweekly.com/link/81079/web)
Yandex刚刚发布了其多线程连接池和请求路由器的1.0版。“我们在生产中使用Odyssey。目前，它在数百台主机上每秒处理超过1000000个请求。”

`Yandex `

## [Postgres新手：保持好奇心](https://postgresweekly.com/link/81080/web)
一个多元化的帖子，里面包含了许多有趣的零散知识。主题涵盖了缓冲、BPF和IO调度等。

`Dmitry Dolgov `

## [PostgreSQL状态调查结果](https://postgresweekly.com/link/81082/web)
我们几个月前发了这篇Postgres的调查报告，。。大约有500人填写了问卷。一半的受访者在AWS上使用Postgres，80%的受访者也在工作之余使用Postgres，而且我们大多数人从未参加过真实的Postgres活动。罗伯特·特里特对结果有一些独立的看法。

`Timescale `

## [PGCon 2020现在寻找演讲主题](https://postgresweekly.com/link/81084/web)
PGCON2020将于明年5月在加拿大渥太华举行。他们正在寻找演讲者。

`PGCon `

## [Amazon为RDS开发了一个代理系统](https://postgresweekly.com/link/81085/web)
如果有很多进程（比如Lambda函数）正在访问基于RDS的数据库，那么这最终会非常方便。目前它只支持MySQL（PostgreSQL支持即将推出），并且只在预览版中提供。


`Amazon Web Services `
## [EnterpriseDB发布Postgres平台12](https://postgresweekly.com/link/81086/web)
EnterpriseDB提供商业Postgres发行版，增加了管理工具、Kubernetes操作员等。


`EnterpriseDB `
## [DB Fiddle:SQL数据库演练场](https://postgresweekly.com/link/81088/web)
我经常发现这个工具对于测试SQL的一些小部分很有用。它允许您从浏览器中对几个版本的Postgres（包括现在的版本12）、MySQL和SQLite运行基本查询。


`Status200 `
## [Postgres 12的解释设置](https://postgresweekly.com/link/81089/web)
一种使EXPLAIN输出更能代表更改影响查询的设置时实际发生的情况的方法。

`Luca Ferrari `

## [如何使用pg_Upgrade执行主版本升级](https://postgresweekly.com/link/81091/web)


`James Chanco Jr. `
## [如何为Postgres和Aurora创建无服务器GraphQL API](https://postgresweekly.com/link/81092/web)
了解如何在Amazon的Aurora上构建一个由Postgres（和MySQL）支持的无服务器GraphQL API。

`Gareth McCumskey `

## [逻辑复制的有趣方面一览](https://postgresweekly.com/link/81093/web)


`Rafia Sabih `
## [phpPgAdmin 7.12.1发布](https://postgresweekly.com/link/81100/web)
一个基于Web的Postgres管理工具。


`Robert Treat `
# 💡本周提示


当您使用psql时，您几乎肯定是在使用诸如\dt之类的命令来获取表列表，或\l来列出表，但是它们是如何工作的呢？


我倾向于认为这样的命令是“魔术”，因为很容易假设psql可以查看Postgres而我没有，但实际上它只是发出类似于任何我可能选择运行的SQL查询。我们能看看这些SQL查询是什么吗？对！


psql有一个ECHO_隐藏变量，您可以将其设置为显示（或“ECHO”）通过反斜杠命令在后台执行的任何SQL查询。设置成这样：


```
\set ECHO_HIDDEN on
```


然后，查看在运行类似以下命令时会发生什么情况：


```
=> \l
    
********* QUERY **********
SELECT d.datname as "Name",
       pg_catalog.pg_get_userbyid(d.datdba)
         as "Owner",
       pg_catalog.pg_encoding_to_char(d.encoding)
         as "Encoding",
       d.datcollate as "Collate",
       d.datctype as "Ctype",
       pg_catalog.array_to_string(d.datacl, E'')
         AS "Access privileges"
FROM pg_catalog.pg_database d
ORDER BY 1;
**************************
  
... list of databases follows here as usual ...
```


如果您自己复制并粘贴此查询，您将得到与通常相同的结果。


这篇技巧的实用性一开始可能看起来很有限，但它可以帮助您理解事物是如何在幕后表示的，并可能调整此类查询以更好地满足您自己的数据库查询需求。


**🗓即将举办的Postgres活动**
- [PgDay SF](https://postgresweekly.com/link/81094/web)（1月21日在旧金山）
- [PgDay FOSDEM](https://postgresweekly.com/link/81101/web)（1月31日，比利时布鲁塞尔）
- [PgConf.Russia](https://postgresweekly.com/link/81095/web)（2月3日至5日，俄罗斯莫斯科）
- [PgConf India](https://postgresweekly.com/link/81096/web)（2月26日至28日，印度马哈拉施特拉邦班加罗鲁）-一个专门的培训日和一个多轨道两天会议。
- [Nordic PgDay 2020](https://postgresweekly.com/link/81102/web)（3月24日在芬兰赫尔辛基）
- [pgDay Paris 2020](https://postgresweekly.com/link/81097/web)（3月26日，法国巴黎）
- [Swiss PGDay 2020](https://postgresweekly.com/link/81098/web)（6月18日至19日，瑞士）
