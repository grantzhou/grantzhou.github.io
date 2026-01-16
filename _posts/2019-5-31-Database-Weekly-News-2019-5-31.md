---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: 数据库每周新闻 2019-5-31
---

## 数据库每周新闻 #256 - 2019年5月31日
![config.yml]({{ site.baseurl }}/assets/img/DBWeekly.png)
备注：[英文原文地址](https://dbweekly.com/issues/256)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/v1559243458/h9ezqffxvml6khgza6gw.jpg)

## [MetricsDB：一个用于在Twitter上存储软件度量的时间序列数据库](https://blog.twitter.com/engineering/en_us/topics/infrastructure/2019/metricsdb.html)
Twitter的时间序列服务每秒可处理8300万个度量。而为了未来的扩展，他们必须寻求一种新的方法。MetricsDB于2017年上线，与传统的键值存储相比，它将总体成本降低了10倍，延迟降低了5倍。

`SATISH KOTHA AND ILHO YE (TWITTER)`

## [一个可扩展的内存非关系型时序数据库](https://www.youtube.com/watch?v=boAZXOSMY58)
GridDB（[主页](https://griddb.net/en/)，以防你不想看视频）曾在2016年短暂地吸引了我们的注意力，但似乎已经成为一个有趣的物联网优化时间序列数据库。GridDB是开源的（经AGPL许可），这里是它的Github网址。

`FIXSTARS CORPORATION`

## [Studio 3T使SQL迁移到MongoDB变得非常简单](https://studio3t.com/knowledge-base/articles/import-sql-database-to-mongodb/?utm_source=cooper&utm_medium=newsletter&utm_campaign=may31)

现在你可以使用Studio 3T的新的SQL迁移功能将整个SQL数据库导入MongoDB中。

`STUDIO 3T` **赞助商**

## [756个（仍持续增长）有趣数据集的链接](https://docs.google.com/spreadsheets/d/1wZhPLMCHKJvwOkP4juclhjFgqIY8fQFMemwKL2c64vk/edit#gid=0)
从昆汀电影中每一个的角色死亡，到游轮巡查，到板球比赛得分，再到国家公园的游客的各种各样的数据集，这是一个非常多样化的乐趣袋。

`DATA IS PLURAL`

## [评估实时消息总线的选择](https://www.datanami.com/2019/05/28/assessing-your-options-for-real-time-message-buses/)
现代实时数据处理系统通常依赖于拥有流处理系统的消息总线。这篇文章总结了包括Apache Kafka, RabbitMQ, 和ActiveMQ在内的部分前者工具。

`DATANAMI`


### 📖 简报
- [PostgreSQL 12 和 PostGIS 3 最终解决了并行空间查询的执行问题](http://blog.cleverelephant.ca/2019/05/parallel-postgis-4.html)。
- [据报道, 曾在Hadoop领域扮演重要角色的MapR, 在一笔融资交易失败后正在寻找一位买主以维持运营](https://www.datanami.com/2019/05/30/after-funding-falls-through-mapr-seeks-a-buyer-to-avoid-shut-down/)
- [黑客新闻用户聚集在一起讨论如何在关系型数据库管理系统RDBMS中表示层次结构](https://news.ycombinator.com/item?id=20027586)。
- [用于关系数据库管理系统SQL Server的亚马逊关系型数据库服务，现在每个实例最多支持100个数据库，高于之前的30个数据库的数量](https://aws.amazon.com/cn/about-aws/whats-new/2019/05/amazon_rds_for_sql_server_increases/)。

### 💻招聘
[高级网站运维工程师—Invoca（加州圣巴巴拉或远程）](https://www.invoca.com/company/job-listings/?gh_jid=4203792002&gh_src=a93ae5e82)--加入我们的运营工程师团队，每天向我们的SaaS开发平台和公共云基础设施多次部署代码。

[在Vettery上寻找数据库有关的工作](https://www.vettery.com/tech?utm_source=newsletter&utm_medium=cooper-dbweekly&utm_term=tech&utm_content=grouped&utm_campaign=ad-88878) – Vettery专门为科技领域的求职者提供相关工作并完全免费。


### 📒 教程和故事

[使用Docker Hub的PostgreSQL图像](https://www.2ndquadrant.com/en/blog/using-docker-hub-postgresql-images/) -- 如果你想使用Docker支持的图像来运行Postgres，例如CI的工作或开发，这将是非常有用的建议。

[将数据从SQL迁移到图形数据库Dgraph](https://blog.dgraph.io/post/migrating-from-sql-to-dgraph/) -- Dgraph是一个高级图形数据库，因此如何将面向SQL的关系模式转换为合适的模式的任务将会非常有趣。

[这些专门的数据库都是用来做什么的？](https://hubs.ly/H0h-XkJ0)-- 本文探讨了开发人员和数据库管理员可以用来为其业务相关者提供他们所需的见解的工具。

[如何使用Chef自动化每日DevOps（开发技术，运营和质量保障）数据库的任务](https://severalnines.com/blog/how-automate-daily-devops-database-tasks-chef) -- 用Chef将手动的数据管理任务转换为一组自动规则。

[如何大大降低PostgreSQL对SaaS的响应时间](https://blog.checklyhq.com/how-i-decimated-postgres-response-times-for-my-saas/) -- 一个将Postgres查询响应时间从平均约100毫秒（峰值为1秒）减少到稳定的1-10毫秒的故事。

[一个关于SQL查询优化的故事](https://parallelthoughts.xyz/2019/05/a-tale-of-query-optimization/) --“我们将查询时间从大约24分钟的缩短到了2秒，性能得到了极大的提高。”

[混合持久化的问题：解决“正确”的数据库的悖论](https://www.datanami.com/2019/05/29/the-polyglot-problem-solving-the-paradox-of-the-right-database/) -- 一个单片数据库很少能满足一个组织的所有数据需求，因此“混合持久化”这一概念变得流行起来。但是运行多个数据库也存在成本问题和其它缺点。


### 代码与工具
[PugSQL：一个用于从文件使用参数化SQL的Python接口](https://pugsql.org/)-- 在单独的文件中定义SQL查询，然后从普通的python代码中即时使用它们。一个受Clojure的HugSQL启发的有趣想法。

[test_db测试数据库：一个带有集成测试套件的MySQL示例数据库](https://github.com/datacharmer/test_db) -- 一个包含约30万“员工” 和280万个薪金条目记录的示例数据库。在167MB时，它便复杂到可用于一般测试（或练习SQL！）而不会崩溃。

[modssl: Redis和KeyDB的一个SSL模块](https://github.com/JohnSully/modssl) -- 任何老派的Apache httpd用户都可能对这个名字感到恼火，但这是一次旨在推广将SSL引入Redis并扩展其API功能的有趣尝试。
