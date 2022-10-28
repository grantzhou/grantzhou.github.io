---
layout: post
title: PostgreSQL 每周新闻 2022-10-13
---
### PostgreSQL每周新闻#476 - 2022年10月13日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/476)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,w_430,h_100/e_make_transparent/co_white,e_outline:7/xyflkz7n00elwtgja9ne.png)
## [Postgres 15 发布](https://www.postgresql.org/about/news/postgresql-15-released-2526/)
自 2016 年 Postgres 9.6 以来，每个新的 Postgres 主要版本都在 9 月底或 10 月初发布，现在 Postgres 15（Postgres 的第 32个主要版本）在通常的 beta 和 RC 版本之后与我们同在。

在接下来的几周里，Postgres Weekly将继续发布有关变化、性能基准和类似发展的博客文章，但现在，有什么新内容？

- SQLMERGE - 很长一段时间 - 用于在单个语句中有条件地修改、插入或删除行。
- 支持 WAL 文件的 LZ4 和 Zstandard (zstd) 压缩。
- 使用 gzip、LZ4 或 zstd 和pg_basebackup.
- 用于检查字符串的新正则表达式函数regexp_count，包括和regexp_like。
- “安全调用者”视图可以使用视图调用者而不是视图创建者的权限来查询数据——这是一项关键的数据安全功能。
- 一种新的jsonlog日志记录格式，不出所料，它使用定义的 JSON 结构进行日志记录。
- 一个新的pg_walinspect扩展打开了通过 SQL 而不是单独的工具查询预写日志的可能性。
- 整体上更快的排序性能。
- 现在可以授予用户更改某些服务器级配置参数的权限。
- 改进的逻辑复制功能。

当然，还有更多内容，您需要查看官方发行说明，因为它们提供了最详尽的更改和新功能指南。

注意：这只是 Postgres Weekly 的 Postgres 15 发行版“newsflash”问题。最新的完整问题，请参阅昨天的问题 - 问题 #475。

# 💡本周提示


**🗓即将举办的Postgres活动**
