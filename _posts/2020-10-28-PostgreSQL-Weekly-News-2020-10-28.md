---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2020-10-28
---
### PostgreSQL每周新闻#379 - 2020年10月28日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/379)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/op8ufo6wzgsrbo2yfw0z.jpg)
## [DBA如何使用Postgres来发现被错误清除的40K选民信息](https://postgresweekly.com/link/97512/web)
一位长期的数据库管理员对选民数据运行查询，以学习如何使用Postgres，并偶然发现了一个严重的选民清除错误。 （提到Postgres的部分大约在4分钟处。）


`VICE (on YouTube) `
## [改善Postgres连接可伸缩性：快照](https://postgresweekly.com/link/97514/web)
从他对连接可伸缩性的角度出发，Andres继续解释了他在Postgres 14中对快照所做的改进，并着眼于性能的改进。


`Andres Freund `
## [如何加快Postgres查询的最佳做法。 免费电子书](https://postgresweekly.com/link/97516/web)
我们分享了帮助Atlassian，Robinhood等公司加快查询速度的经验。


`pganalyze `
## [Slonik：先进的Node.js Postgres客户端库](https://postgresweekly.com/link/97517/web)
经过实践检验的框架，可以抽象出重复的代码模式，防止不安全的行为，并提供丰富的调试体验。 如果您完全使用Node中的Postgres，这篇文值得一看。


`Gajus Kuizinas `
## [使用Postgres来塑造和准备科学数据](https://postgresweekly.com/link/97518/web)
而不是依靠Google Sheets或快速的Python脚本（两者都很好！），Steve只想将Postgres用于数据建模任务，而这篇文描述发生的情况。


`Steve Pousty `
## [使用SQL随机采样数据](https://postgresweekly.com/link/97519/web)
数据采样的数据建模的后续文章。


`Steve Pousty `
## [在Postgres中检测时间序列数据中的间隙](https://postgresweekly.com/link/97520/web)
即使您没有这个问题，也可以通过创造性的方法解决该问题。


`David Christensen `
## [在GitHub和PGXN上自动化Postgres扩展版本](https://postgresweekly.com/link/97521/web)
我很想知道实际上有多少人编写自己的扩展，但是如果您这样做，这里有一些有用的知识，可以通过GitHub在GitHub和PGXN上自动化发布扩展。 


`David E. Wheeler `
## [使用Scalefield-您的私有Postgres云数据库](https://postgresweekly.com/link/97522/web)
Scalefield可让您轻松地在自己的云中托管PostgreSQL集群-完全灵活，可扩展且可靠。


`CYBERTEC `
## [SQL中的外键和插入顺序](https://www.cybertec-postgresql.com/en/postgresql-foreign-keys-and-insertion-order-in-sql/)


`HANS-JÜRGEN SCHÖNIG`
## [使用“LIKE”做join，或者为什么PostgreSQL FTS是一个强大的替代方案](https://postgrespro.co.il/blog/joins-using-like-or-why-postgresql-fts-is-a-powerful-alternative/)

`VADIM YATSENKO`
## [关于Postgres分区的广泛网络研讨会](https://www.2ndquadrant.com/en/blog/postgresql-partitioning-by-simon-riggs-full-webinar-video/)

`2NDQUADRANT`
# 💡本周提示


使用部分索引来提高性能


顾名思义，部分索引仅对表中的一部分行进行索引。 与完全索引相比，部分索引可以提高性能，因为使用部分索引的查询不需要扫描那么多的行。


通过运行同时具有完整索引和部分索引的EXPLAIN语句并比较扫描的行数，可以看到性能差异。

假设我们有一个orders表，其中包含1,000,000行数据：


```
CREATE TABLE orders (
  id INT PRIMARY KEY,
  customer_id INT,
  status TEXT
);

INSERT INTO orders (id, customer_id, status)

SELECT
  i,
  (random()*10000)::INT,
  CASE (random() * 2)::int
    WHEN 0 THEN 'pending'
    WHEN 1 THEN 'shipped'
    WHEN 2 THEN 'completed'
  END
    FROM generate_series(1, 1000000) i;
```


首先，我们在customer_id列上添加二级索引：


```
CREATE INDEX full_idx ON orders (customer_id);
```


假设经常查询特定客户的不完整订单。 使用示例SELECT查询进行的简单EXPLAIN ANALYZE分析显示，在full_idx中扫描了108行，之后过滤器删除了36行：


```
EXPLAIN SELECT * FROM orders where customer_id = 1001 AND status != 'completed';

            QUERY PLAN
------------------------------------
 Bitmap Heap Scan on orders
  (actual time=0.041..0.116 rows=72 loops=1)
   Recheck Cond: (customer_id = 1001)
   Filter: (status <> 'completed'::text)
   Rows Removed by Filter: 36
   Heap Blocks: exact=108
   ->  Bitmap Index Scan on full_idx
       (actual time=0.026..0.026 rows=108 loops=1)
  Index Cond: (customer_id = 1001)
```


通过创建仅索引不完整订单的部分索引，我们可以减少扫描的行数。 运行与上面相同的EXPLAIN ANALYZE，将显示在partial_idx中仅扫描满足查询的72行：


```
CREATE INDEX partial ON orders (customer_id)
  WHERE status != 'completed';
  
EXPLAIN SELECT * FROM orders WHERE
  customer_id = 1001 AND status != 'completed';

            QUERY PLAN
------------------------------------
 Bitmap Heap Scan on orders
  (actual time=0.043..0.100 rows=72 loops=1)
   Recheck Cond: ((customer_id = 1001) AND
                  (status <> 'completed'::text))
   Heap Blocks: exact=72
   ->  Bitmap Index Scan on partial_idx
       (actual time=0.034..0.034 rows=72 loops=1)
  Index Cond: (customer_id = 1001)
```

本周的提示由CockroachDB的创建者Cockroach Labs赞助。 部分索引即将在版本20.2中提供。 在此演示中了解有关CockroachDB的信息：“分布式SQL：现代的云原生PostgreSQL。”
