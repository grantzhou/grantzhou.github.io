---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2019-03-27
---

### PostgreSQL每周新闻#298 - 2019年3月27日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/298)

![pg_img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/fslxzjzgirumeh4bnk9v.jpg)

## [Postgres云解决方案基准测试：Amazon RDS](https://severalnines.com/blog/benchmarking-managed-postgresql-cloud-solutions-part-two-amazon-rds)
两周前，他们对[Amazon Aurora进行了基准测试](https://severalnines.com/blog/benchmarking-managed-postgresql-cloud-solutions-part-one-amazon-aurora)，现在轮到RDS了。剧透：在Postgres方面，Aurora的性能明显优于RDS，虽然Aurora是一个[完全不同的产品](https://aws.amazon.com/cn/blogs/database/introducing-the-aurora-storage-engine/)。

`VIOREL TABARA`

## [PostgreSQL 11在Heroku（和AWS）上可用](https://blog.heroku.com/postgresql-11-general-availability)
Heroku是云应用程序平台，多年来一直是Postgres的领先者，现在他们已经在整个服务中普遍提供Postgres 11的支持。欢呼。据相关新闻报道，[AWS RDS上也支持Postgres 11](https://aws.amazon.com/cn/about-aws/whats-new/2019/03/postgresql11-now-supported-in-amazon-rds/)！

`BECKY JAIMES (HEROKU)`

## [免费电子书：如何在Postgres数据库上获得3倍的性能提升](https://pganalyze.com/ebooks/optimizing-postgres-query-performance?utm_source=PostgresWeeklyPrimary)
![img](https://copm.s3.amazonaws.com/dfb2e687.png)  
了解我们为Atlassian等客户优化Postgres查询性能的最佳实践，以及如何将磁盘加载的数据减少500倍。

`PGANALYZE` **赞助商**

## [加速GROUP BY](https://www.cybertec-postgresql.com/en/speeding-up-group-by-in-postgresql/)
SQL的GROUP BY通常用于将结果集中的记录组合在一起以进行汇总/聚合，作者声称有一种方法可以加速这些操作并获得一些“免费”的额外性能。

`HANS-JÜRGEN SCHÖNIG`

## [Postgres中的索引：了解B-Tree](https://habr.com/en/company/postgrespro/blog/443284/)
[最新的一系列广泛的帖子](https://habr.com/en/company/postgrespro/blog/441962/)深入探讨了Postgres中索引的工作原理。这比你需要知道的更多，它会帮助你理解为什么索引有时会有那样表现。

`EGOR ROGOV`

## [Pivotal推出自己的Postgres版本](https://content.pivotal.io/blog/pivotal-postgres)
Pivotal是一家知名的云开发公司，他们已经创建了[自己的商用的Postgres 11软件包](https://pivotal.io/pivotal-postgres)（用于RHEL 7）以及复制管理器等企业级插件。

`PIVOTAL`

## [计算不同索引事物的最佳方式](https://www.peterbe.com/plog/best-way-to-count-distinct-indexed-things-in-postgresql)
计算子查询结果的效率比尝试在单个查询中使用DISTINCT进行计数要高效得多。

`PETER BENGTSSON`

## [监控PostgreSQL WAL文件](https://pgdash.io/blog/postgres-monitor-wal-files.html)
监视Postgres WAL文件可以实现更高性能的PostgreSQL部署。文章找出了原因和方法。

`PGDASH` **赞助商**

## [比较Postgres客户端：SQLPro vs Table Plus vs Postico](https://spin.atomicobject.com/2019/03/26/postgresql-database-client/)
一位开发人员非常简短地概述了她关于Postgres的三个不同的GUI应用程序的喜欢和不喜欢的点，以及使用每一个的原因。

'MEREDITH LIND'

## [Barman V2.7发布：备份和恢复管理工具](https://www.postgresql.org/about/news/1930/)
使用此工具可为所有关键生产数据库实施灾难恢复解决方案。[项目主页](https://www.pgbarman.org/)。

`2NDQUADRANT`

## [wal2json：用于变更集提取的JSON输出插件](https://github.com/eulerto/wal2json)
每个事务生成一个JSON对象，其中包含用于更新的新旧元组。

`EULER TAVEIRA DE OLIVEIRA`

# ![_config.yml]({{ site.baseurl }}/assets/img/Tips-icon.png)   本周提示
由strongdm提供支持

使用.psqlrc改善您的psql体验

除非你找到了你真正喜欢的GUI工具，否则在使用Postgres数据库时你很可能会使用到Postgres的默认psql客户端。

.psqlrc是一个用户级配置文件（虽然还有一个系统范围的psqlrc文件），您可以在主目录中创建为psql设置各种默认选项，并使其行为更适合您。

开始，可以在主目录中创建一个.psqlrc文件并粘贴这些命令：

`\timing`

`\pset null 'ø'`

简单的原因是因为我们只是为了展示其基本概念！

`\timing` 打开查询时间，显示查询运行了多长时间（这是我们在292期中的提示）。
`\pset null 'ø'` 使psql显示空值作为ø字符（类似于'空集'符号），从而不容易错过空格。

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/utt8rsg6s07hrv31ax0p.jpg)

想多学习一点？ 查看[An Explained psqlrc](https://thoughtbot.com/blog/an-explained-psqlrc)和[Customizing My Postgres Shell](https://www.citusdata.com/blog/2017/07/16/customizing-my-postgres-shell-using-psqlrc/)以获取更多想法。

*本周的提示由strongDM赞助。 Hearst，SoFi和Peloton的团队信任strongDM来管理工程师对所有对象的访问。*

🗓  即将举办的Postgres活动  

   * [pgconf.de 2019 (5月10日,莱比锡)](https://2019.pgconf.de/) —— 最成功的德语PostgreSQL会议。  
   * [PGDay.IT 2019 (5月16日,博洛尼亚)](https://2019.pgday.it/en/)  
   * [PGCon 2019(5月28日,渥太华)](https://www.pgcon.org/2019/) —— 供用户和开发人员见面和讨论Postgres的年度会议
   * [Postgres Vision 2019(6月24日,波士顿)](https://postgresvision.com/)  



