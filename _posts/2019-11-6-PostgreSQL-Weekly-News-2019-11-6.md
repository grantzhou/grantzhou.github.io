---
layout: post
title: PostgreSQL 每周新闻 2019-11-6
categories: [PostgreSQL]
tags: [PGWeekly]
---
### PostgreSQL每周新闻#330 - 2019年11月6日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/330)

## [Postgres 12 初始查询性能印象](https://www.cybertec-postgresql.com/en/postgresql-v12-initial-query-performance-impressions/)
我们一直对 Postgres 12 感到兴奋，但它的实际性能如何？Kaarel 进行了各种规模级别的压力测试，结果好坏参半，没有明显的结论。

`Kaarel Moppel`

## [在面向行的数据库中构建列式压缩](https://blog.timescale.com/blog/building-columnar-compression-in-a-row-oriented-database/)
Timescale 如何在最新版本的 TimescaleDB 时间序列数据扩展中实现 91%-96% 的压缩率。

`Timescale`

## [PostgreSQL 专家实践培训](http://www.2qpgconf.com)
以特别优惠价格参加芝加哥 2Q PGConf 2019 的 PostgreSQL 实践培训，由当地 2ndQuadrant 专家授课。课程包括：PostgreSQL 数据库安全、PostgreSQL 多主复制、Postgres 优化、PostgreSQL 业务连续性。

`2ndQuadrant PostgreSQL Training` **赞助商**

## [postgres-checkup：Postgres 健康检查工具](https://gitlab.com/postgres-ai/postgres-checkup/)
一个诊断工具，对 Postgres 数据库的健康状况进行"深度分析"，检测问题并为解决发现的任何问题提供建议。[v1.3.0](https://gitlab.com/postgres-ai/postgres-checkup/-/tags/1.3.0) 刚刚发布。

`Postgres.ai`

## [使用 HAProxy 与 Xinetd 实现应用程序连接故障转移](https://www.percona.com/blog/2019/10/31/postgresql-application-connection-failover-using-haproxy-with-xinetd/)
我是 [haproxy](http://www.haproxy.org/) 的忠实粉丝，这是一个功能强大但易于管理的 TCP 和 HTTP 代理/负载均衡器，所以我很期待这个系列的其余部分。

`Jobin Augustine`

## [实现 K-最近邻空间分区广义搜索树索引](https://www.2ndquadrant.com/en/blog/postgresql-12-implementing-k-nearest-neighbor-space-partitioned-generalized-search-tree-indexes/)
K-最近邻回答了"最接近的匹配是什么？"这个问题。PostgreSQL 12 可以回答这个问题，并在回答时使用索引。

`Kirk Roybal`

## [在 FreeBSD 上安装 PostgreSQL 12 软件包](https://fluca1978.github.io/2019/11/04/PostgreSQL12FreeBSD.html)
由于 Postgres 12 的最终版本尚未纳入季度软件包更新，因此您需要做一些工作。

`Luca Ferrari`

## [通过 Ansible 在 FreeBSD 上安装 Postgres](https://fluca1978.github.io/2019/10/30/PostgreSQL_FreeBSD_Ansible.html)

`Luca Ferrari`

## 🛠 代码和工具

## [PostgREST 6.0：从 Postgres 数据库提供 RESTful API](https://postgrest.org/en/v6.0/)
这不是新项目，但它是一个成熟的项目，本周又在社交媒体上流行起来，所以让我们再次关注它 :-)

`Joe Nelson et al.`

## [消除改进查询性能的猜测](https://www.pgmustard.com?referrer=postgresweekly)
基于查询计划，pgMustard 为您提供加快查询速度的技巧。免费试用。

`pgMustard` **赞助商**

## [使用 Ruby 管理 PostgreSQL 的分区表](https://www.honeybadger.io/blog/pg-partition-manager/)
`pg_partition_manager` 是一个新的 gem，用于维护需要随着应用程序中基于时间的数据的添加和过期而创建和删除的分区表。

`Benjamin Curtis`

## [Pgpool-II 4.1.0 发布](https://www.postgresql.org/about/news/1989/)
为 Postgres 添加连接池和负载均衡。4.1 引入了语句级负载均衡和自动故障恢复。

`Pgpool Global Development Group`

## 💡 本周技巧

**将多个 `LIKE` 模式放入数组**

对列内容执行任意搜索的一种简单方法是在查询中使用 `LIKE` 子句。例如，在博客文章表中，此查询可以找到标题包含字符串 `'Java'` 的所有文章：

```sql
SELECT * FROM posts WHERE title LIKE '%Java%';
```

如果您想创建更复杂的查询，事情很快就会变得笨拙：

```sql
SELECT * FROM posts WHERE title LIKE '%Java%' OR title LIKE '%Perl%' OR title LIKE '%Python%';
```

Postgres 支持两个名为 `ANY`（`SOME` 是含义相同的别名）和 `ALL` 的 SQL 操作符，可用于对一组值执行单个检查，我们可以将其与 `LIKE` 查询一起使用。

`ANY` 和 `ALL` 更常与子查询一起使用，但我们可以将多个 `LIKE` 匹配模式放入数组，然后将其提供给 `ANY` 或 `ALL`，如下所示：

```sql
SELECT * FROM posts WHERE title LIKE ANY(ARRAY['%Java%', '%Perl%', '%Python%']);
```

还有一种以更短样式编写数组字面量的方法，如果您喜欢：

```sql
SELECT * FROM posts WHERE title LIKE ANY('{%Java%,%Perl%,%Python%}');
```

自然，虽然这些查询会找到 `title` 与任何提供的模式匹配的任何行，但您也可以使用 `ALL` 来确保仅获取包含所有模式的标题。

本周技巧由 [DigitalOcean](https://blog.digitalocean.com/how-we-launched-our-marketplace-using-digitalocean-kubernetes-part-1/?medium=display&utm_source=cooperpress&utm_campaign=MDB_Dev_Signup_Cold_Newsletter11-6-2019) 赞助。了解 [DigitalOcean 的工程师如何在其托管的 Kubernetes 服务之上为开发人员构建可扩展的市场](https://blog.digitalocean.com/how-we-launched-our-marketplace-using-digitalocean-kubernetes-part-1/?medium=display&utm_source=cooperpress&utm_campaign=MDB_Dev_Signup_Cold_Newsletter11-6-2019)。

## 🗓 即将举行的活动

- [PG Down Under](https://pgdu.org/)（11月15日，澳大利亚悉尼）— 这个年度澳大利亚 Postgres 会议的第二次举办。
- [2Q PGCONF 2019](https://www.2qpgconf.com/)（2019年12月4-5日，芝加哥）— 致力于交流关于世界上最先进的开源数据库 PostgreSQL 知识的会议。
- [PgDaySF](https://2020.pgdaysf.org/)（2020年1月21日，旧金山）— 将 PostgreSQL 国际社区带到旧金山和硅谷的中心。
- [PgConf.Russia](https://pgconf.ru/2020)（2020年2月3-5日，俄罗斯莫斯科）— 一天的教程和两天的三个并行会议的演讲。
- [PGConf India](https://pgconf.in/conferences/pgconfin2020)（2020年2月26-28日，印度马哈拉施特拉邦班加罗尔）— 专门的培训日和为期两天的多轨道会议。
- [pgDay Paris 2020](https://2020.pgday.paris/#%2319)（2020年3月26日，法国巴黎）— 与同行一起了解更多关于世界上最先进的开源数据库的信息。