
这是**即将发布**的PG14发行说明的翻译文稿

===

PostgreSQL全球开发组今天宣布[PostgreSQL 14](https://www.postgresql.org/docs/14/release-14.html)正式发布,  这是世界上[最先进的开源数据库](https://www.postgresql.org/)
的最新版本。

PostgreSQL 14 带来了很多新特性，可以帮助开发人员和管理员部署以数据为支撑的应
用程序。PostgreSQL 持续在复杂数据类型上添加创新特性，包括更便利地访问JSON和对非
连续数据范围的支持。此次最新版本还增加了 PostgreSQL 在高性能和分布式数据工作负载
方面的改进趋势，在支持连接并发、高写入工作负载、并行查询和逻辑复制方面进行了改进
。

“PostgreSQL 的最新版本提高了我们用户大规模管理数据工作负载的能力，增强了可观察性
，并包含有助于应用程序开发人员的新功能，”，PostgreSQL 核心团队成员Magnus 
Hagander 说，"PostgreSQL 14 证明了全球 PostgreSQL 社区致力于解决反馈并继续
提供由大大小小的组织部署的创新数据库软件。”

[PostgreSQL](https://www.postgresql.org)是一种创新的数据管理系统，以其可靠性和健壮性著称，得益于[全球开发者社区](https://www.postgresql.org/community/) 
超过25年的开源开发，它已成为各种规模组织首选的开源关系型数据库。


### JSON 便利和多范围

PostgreSQL 从PostgreSQL 版本9.2开始就已经支持操作[JSON](https://www.postgresql.org/docs/14/datatype-json.html)数据，只是检索时所使用的语
法比较独特。PostgreSQL 14 可以[使用下标访问 JSON 数据](https://www.postgresql.org/docs/14/datatype-json.html#JSONB-SUBSCRIPTING)。
比如现在支持这样查询：
`SELECT ('{ "postgres": { "release": 14 }}'::jsonb)['postgres']['release'];`

这使PostgreSQL与从JSON数据中检索信息时的通用语法保持一致。PostgreSQL 14 中添加的
下标框架一般可以扩展到其他嵌套数据结构，同时也适用于本次发布的[`hstore`](https://www.postgresql.org/docs/14/hstore.html)数据类型。

[Range 类型](https://www.postgresql.org/docs/14/rangetypes.html)同样也是在PostgreSQL 版本9.2首次发布的，现在引入了"[multirange](https://www.postgresql.org/docs/14/rangetypes.html#RANGETYPES-BUILTIN)"数据类型
来支持非连续范围的数据。multirange是非重叠范围的有序列表，它让开发人员通过编写更
简单的查询来处理复杂的范围序列。PostgreSQL原生的范围类型（dates, times, numbers）
支持multirange，其他数据类型被扩展后也可以使用multirange。

### 高工作负载的性能改进

PostgreSQL 14 为使用多连接的工作负载提供了显著的吞吐量提升，在一些基准测试中，
速度提高了2倍。此版本继续通过在[频繁更新索引](https://www.postgresql.org/docs/14/btree-implementation.html#BTREE-DELETION)的表上减少索引膨胀来改进B树索引的整体
管理。

PostgreSQL 14 引入了[管道查询](https://www.postgresql.org/docs/14/libpq-pipeline-mode.html)的能力，这可以显著提升高延迟连接或具有许多小量写
(`INSERT`/`UPDATE`/`DELETE`)操作的工作负载性能。由于这是客户端功能，因此只要使用版本14
的客户端或使用[通过版本14的libpq构建的客户端驱动程序](https://wiki.postgresql.org/wiki/List_of_drivers)，就可以对任何现代 PostgreSQL 
数据库使用管道模式。

### 分布式工作负载的增强功能

分布式 PostgreSQL 数据库将从 PostgreSQL 14 中受益。使用[逻辑复制](https://www.postgresql.org/docs/current/logical-replication.html)时，PostgreSQL 现
在可以将正在进行的事务以流复制形式传输给订阅者，这对订阅大型事务的应用具有显著
的性能优势。PostgreSQL 14 还为支持逻辑复制的逻辑解码系统添加了一些其他性能改进。

过去用于处理跨 PostgreSQL 和其他数据库的联合工作负载的[外部数据包装器](https://www.postgresql.org/docs/14/sql-createforeigndatawrapper.html)，现在可以利
用 PostgreSQL 14 中的并行查询特性。
本版本在 [`postgres_fdw`](https://www.postgresql.org/docs/14/postgres-fdw.html)（与其他 PostgreSQL 数据库接口的外部数据包装器）中实现了此
功能。

除了支持并行查询之外，`postgres_fdw` 现在也可以使用[`IMPORT FOREIGN SCHEMA`](https://www.postgresql.org/docs/14/sql-importforeignschema.html) 指令在
外部表上批量插入数据并导入表分区。

### 管理和可观察性

PostgreSQL 14 将其性能提升扩展到了其 [vacuuming](https://www.postgresql.org/docs/14/routine-vacuuming.html)系统。
本版本包括用于减少 B 树索引开销的优化。此版本还添加了一个vacuum的"紧急模式"，旨
在防止事务ID环绕。
[`ANALYZE`](https://www.postgresql.org/docs/14/sql-analyze.html)用于收集数据库统计信息，基于其自身的性能改进，现在在 
PostgreSQL 14中运行速
度明显更快。

[现在可以配置](https://www.postgresql.org/docs/14/runtime-config-client.html#GUC-DEFAULT-TOAST-COMPRESSION)PostgreSQL的[TOAST](https://www.postgresql.org/docs/14/storage-toast.html) 系统的压缩选项，该系统用于存储较大的数据，如文本块
或几何图形。

PostgreSQL 14 为 TOAST 列添加了 LZ4 压缩，同时保留对 `pglz` 压缩的支持。

PostgreSQL 14 添加了几个新功能来帮助监控和可观察性，包括[跟踪“COPY”命令的进度](https://www.postgresql.org/docs/14/progress-reporting.html#COPY-PROGRESS-REPORTING)、
[预写日志 (WAL) 活动](https://www.postgresql.org/docs/14/monitoring-stats.html#MONITORING-PG-STAT-WAL-VIEW)和[复制槽统计信息](https://www.postgresql.org/docs/14/monitoring-stats.html#MONITORING-PG-STAT-REPLICATION-SLOTS-VIEW)。

启用[`compute_query_id`](https://www.postgresql.org/docs/14/runtime-config-statistics.html#GUC-COMPUTE-QUERY-ID)可以让您通过多个 PostgreSQL特性（包括 [`pg_stat_activity`](https://www.postgresql.org/docs/14/monitoring-stats.html#MONITORING-PG-STAT-ACTIVITY-VIEW)、
[`EXPLAIN VERBOSE`](https://www.postgresql.org/docs/14/sql-explain.html)和其他更多特性）来唯一跟踪某个查询。

### SQL 性能、一致性和便利性

查询计划和执行在PostgreSQL 14中也进行了改进。此版本包括对 PostgreSQL 并行查询支
持的多项改进，包括更好的并行顺序扫描性能、[`PL/pgSQL`](https://www.postgresql.org/docs/14/plpgsql.html)在使用 `RETURN QUERY` 命令时执行
并行查询的能力、以及启用 [`REFRESH MATERIALIZED VIEW`](https://www.postgresql.org/docs/14/sql-refreshmaterializedview.html) 执行并行查询。
此外，PostgreSQL 14中新增的附加缓存让嵌套查询性能得到提升。

[扩展统计]((https://www.postgresql.org/docs/14/planner-stats.html#PLANNER-STATS-EXTENDED))现在可以在 PostgreSQL 14 中用于表达式。此外，[PostgreSQL 13](https://www.postgresql.org/about/news/postgresql-13-released-2077/)中引入的一个
[窗口函数]功能(https://www.postgresql.org/docs/14/functions-window.html)现在也可以
从增量排序中得到提升。

[存储过程](https://www.postgresql.org/docs/14/sql-createprocedure.html)允许在代码块中进行事务控制，现在可以使用`OUT`参数返回数据。

PostgreSQL 14 引入了使用 [`date_bin`](https://www.postgresql.org/docs/14/functions-datetime.html#FUNCTIONS-DATETIME-BIN)函数，可以将时间戳按照任意间隔进行分组或对齐。

此版本还添加了符合SQL的[`SEARCH`](https://www.postgresql.org/docs/14/queries-with.html#QUERIES-WITH-SEARCH)和[`CYCLE`](https://www.postgresql.org/docs/14/queries-with.html#QUERIES-WITH-CYCLE) 子句，以帮助递归[公用表表达式](https://www.postgresql.org/docs/14/queries-with.html#QUERIES-WITH-RECURSIVE)的排序和循环
检测。

### 安全性改善

PostgreSQL 14 可以方便地使用 `pg_read_all_data` 和 `pg_write_all_data` [预定义角色](https://www.postgresql.org/docs/14/predefined-roles.html)为
用户分配表、视图和模式的只读和只写权限。

此外，此版本现在将符合标准的[`SCRAM-SHA-256`](https://www.postgresql.org/docs/14/auth-password.html)密码管理和身份验证系统做为PostgreSQL 
新实例的默认设置。

### 关于PostgreSQL

[PostgreSQL](https://www.postgresql.org)是世界上最先进的开源数据库，它的全球社区是一个由成千上万的用户、开发
人员、公司或其他组织组成的。PostgreSQL起源于加利福尼亚大学伯克利分校，已经有30
多年的历史，并且以无与伦比的开发速度继续发展。 PostgreSQL的成熟功能不仅与顶级商
业数据库系统匹配，而且在高级数据库功能、可扩展性、安全性和稳定性方面超过了它们。


### 链接

* [下载](https://www.postgresql.org/download/)
* [发行说明](https://www.postgresql.org/docs/14/release-14.html)
* [新闻资料](https://www.postgresql.org/about/press/)
* [安全](https://www.postgresql.org/support/security/)
* [版本政策](https://www.postgresql.org/support/versioning/)
* [在Twitter上关注@postgresql](https://twitter.com/postgresql)

