---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2020-2-26
---
### PostgreSQL每周新闻#344 - 2020年2月26日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/344)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/v1582661449/n83rk36tjevqygoeh1kp.png)

## [共享缓冲区：探索Postgres的I/O缓存](https://postgresweekly.com/link/84442/web)
简单地说，shared_buffers config设置允许您指定用于缓存数据的内存量，但128兆字节的默认值相对较低（因此通常增加此值）。以下是缓存的作用和内容。

`Hans-Jürgen Schönig `

## [PostgreSQL的锁](https://postgresweekly.com/link/84444/web)
在数据库系统中，锁防止同时访问（或操作）已经在使用或正在更改的数据。Postgres支持多种类型的锁，如表锁、行锁、事务锁等等。这篇文章对他们进行了更深入的研究。

`Movead Li `

## [实时跟踪PostgreSQL关键性能指标](https://postgresweekly.com/link/84445/web)
使用可拖放的自定义仪表板以秒为单位确定运行缓慢的查询、瓶颈、错误率等，以确保数据库能够充分扩展。提升PostgreSQL性能，免费使用Datadog。


`Datadog `
## [Postgres备份的自动化测试](https://postgresweekly.com/link/84446/web)
有备份是一回事，但你也需要确保它们是可行的，并准备好实际使用。


`RapidLoop `
## [Postgres Parallelism，接下来呢？](https://postgresweekly.com/link/84447/web)
简单回顾一下PostgreSQL从9.6到现在的并行性之旅。


`Amit Kapila `
## [准备Postgres数据以进行扩展](https://postgresweekly.com/link/84448/web)
随着你的应用程序越来越受欢迎，你应该如何为Postgres实例的使用增长做好准备？


`Matthew Revell `
## [深入挖掘Postgres的底层：保持好奇心](https://postgresweekly.com/link/84449/web)
▶这是去年40分钟的讨论，它深入探讨了如何使用strace和gdb等工具来解决复杂的性能问题。可能你们大多数人永远不需要做这些事情，但知道这是可能的是很有用的。

`Dmitrii Dolgov `

## [为什么我不喜欢uuid数据类型](https://postgresweekly.com/link/84450/web)
uuid与标准的顺序键相比既有优点也有缺点。这篇文章只关注性能，但评论有助于平衡。


`Hubert depesz Lubaczewski `
## [在Kerberos环境中使用libpq 12连接到Azure PostgreSQL](https://postgresweekly.com/link/84451/web)


`Magnus Hagander `
## [使用Buildkite为所有软件项目提供更快的CI/CD](https://postgresweekly.com/link/84452/web)
看看Shopify如何将300名工程师扩展到1500名，同时将他们的构建时间控制在5分钟以内。


`Buildkite `
## [PostGIS 3.0.1:Postgres的地理空间对象](https://postgresweekly.com/link/84453/web)
它可能只是一个x.0.1版本，但它是PostGIS迁移到git之后的第一个版本，如果需要，它还支持当前的edge Postgres 13版本。


`PostGIS Developers `
## [rails pg extras:Postgres Ruby和rails数据库洞察](https://postgresweekly.com/link/84454/web)
RubyonRails开发人员？这个插件可以让您快速获得锁、索引使用、缓冲区缓存命中率、真空状态等信息。还有一个纯Ruby（非Rails）版本。


`Paweł Urbanek `
# 💡本周提示


**🗓即将举办的Postgres活动**
- [Postgres Conference 2020](https://postgresweekly.com/link/84456/web)（3月23日至27日，美国纽约）
- [Nordic PgDay 2020](https://postgresweekly.com/link/84457/web)（3月24日芬兰赫尔辛基）
- [pgDay Paris 2020](https://postgresweekly.com/link/84458/web)（3月26日法国巴黎）
- [Swiss PGDay 2020](https://postgresweekly.com/link/84459/web)（6月18日至19日，瑞士）
- [Postgres Ibiza 2020](https://postgresweekly.com/link/84460/web)（6月25日至26日，西班牙伊比沙岛）
