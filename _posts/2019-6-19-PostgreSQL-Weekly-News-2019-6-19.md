---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2019-6-19
---

### PostgreSQL每周新闻#310 - 2019年6月19日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/310)

## [在“每个项目”上轻松运行Postgres](https://jamey.thesharps.us/2019/05/29/per-project-postgres/)
“我研究出如何设置一个几乎和SQLite一样方便的Postgres数据库。”目标是让它像在项目文件夹中输入postgres一样简单，以获得仅为该项目运行的Postgres实例。怎么实现？使用direnv来处理环境和Nix包管理器（仅限Linux和macOS）。

`JAMEY SHARP`

## [从另一个角度来看Postgres的Bloom索引](https://www.percona.com/blog/2019/06/14/bloom-indexes-in-postgresql/)
上周我们链接了[Egor Rogov对bloom索引的看法](https://habr.com/en/company/postgrespro/blog/452968/)，但如果你从未听说过bloom过滤器的数据结构，那么这是一个更容易理解的介绍。

`AVINASH VALLARAPU`

## [PostgresLondon——最后的注册机会🐘](https://postgreslondon.org/)
在伦敦加入我们的PGConf UK变革，了解更多关于PostgreSQL最新的成就和令人兴奋的未来发展。您还可以参加以下的专家实践培训：PostgreSQL安全和 Multi-master 复制。

`POSTGRESQL EVENTS` **赞助商**

## [Timescale推出Timescale Cloud：托管时间序列数据库服务](https://blog.timescale.com/timescale-cloud-first-fully-managed-time-series-database-service-runs-on-aws-gcp-azure/)
为什么这是一个Postgres新闻？除了作为托管云服务之外，[TimescaleDB](https://github.com/timescale/timescaledb)还是一个开源Postgres扩展，用于大规模处理时间序列数据。

`JEFF SPOSETTI AND AJAY KULKARNI`

## [使用SQL进行线性插值](https://bytefish.de/blog/postgresql_interpolation/)
如果你有按时间顺序排列的不完整的数据集，如何找到缺失的数据，以及如何修复。这篇文章是关于以上问题的实际操作。

`PHILIPP WAGNER`

## [实现MySQL和Postgres之间的交叉复制的概述](https://severalnines.com/blog/overview-postgresql-mysql-cross-replication)
使用两种不同的工具实现MySQL和Postgres数据库之间的交叉复制的详细说明：pg_chameleon（Postgres特定系统）和SymmetricDS（数据库未知工具）。

`NAWAZ AHMED`

## [检查单次传递中的序列状态](https://fluca1978.github.io/2019/06/11/SequenceCheck.html)
介绍一个可以从pg_sequence目录中收集有关序列的信息的函数。

`LUCA FERRARI`

## [要在PostgreSQL数据库中监视的度量标准](https://www.influxdata.com/blog/metrics-to-monitor-in-your-postgresql-database/?utm_campaign=postgres&utm_medium=newsletter&utm_source=cooperpress)
在数据库性能方面，您需要跟踪几个关键指标，并且它们并非都是特定于数据库的。

`INFLUXDATA` **赞助商**

## [PG Reloaded：定期恢复Postgres数据库的CLI工具](https://github.com/zikani03/pg_reloaded)

`ZIKANI NYIRENDA MWASE`

## [Postgres派生的数据库列表](https://wiki.postgresql.org/wiki/PostgreSQL_derived_databases)

`POSTGRESQL WIKI`

# ![_config.yml]({{ site.baseurl }}/images/Tips-icon.png)   本周提示
由pganalyze提供支持

### CREATE TABLE的LIKE选项  
你可能听说过[表继承](https://www.postgresql.org/docs/10/tutorial-inheritance.html),但是,如果你想要一些不那么紧密耦合的东西呢？假设你只想创建一个与另一个表具有相同列的表？  
在CREATE TABLE上输入LIKE选项。它的结果如下：  

```
# create table people (name text, age integer);
# create table people2 (LIKE people)
# \d people2
       
Table "public.people2"
 Column | Type 
--------+---------
   name | text 
    age | integer
```  
这是最基本的例子，但它远不止于此。 例如，假设你在第一个表上定义了索引，约束，注释或存储设置，你可以指定是要包含所有这些还是仅包含单个：  
```
# create table people3 (LIKE people INCLUDING ALL)
# create table people4 (LIKE people INCLUDING INDEXES)
```  
你还可以使用LIKE来包含列，同时添加其他你自己选择的列。 例如：  
```
# create table people5 (LIKE people, city text);
```  
有关此功能的更多信息，请查看[CREATE TABLE文档](https://www.postgresql.org/docs/9.1/sql-createtable.html)的like_option部分。

本周提示由pganalyze赞助。DBA和开发人员使用pganalyze来确定Postgres数据库中性能问题的根本原因，以优化查询并获取有关关键问题的警报。

🗓  **即将举办的Postgres活动**  

- [Postgres Vision 2019(6月24日,波士顿)](https://postgresvision.com/) —— Web发明者Tim Berners-Lee爵士将发表主题演讲。
- [PostgresLondon 2019 (7月2-3日，伦敦)](https://postgreslondon.org/)
- [PostgresConf Beijing 2019(7月3-6日，中国北京)](https://postgresconf.org/conferences/Beijing)
- [PGConf.Brasil 2019 (8月1-3日，巴西圣保罗)](https://www.pgconf.com.br/2019/en/) ——为期三天的PG会议，包括讲座，教程，课程，Couch Clinic和快闪讲座。
- [PGDay Austria 2019 (9月6日，奥地利维也纳新城)](https://pgday.at/en/)







