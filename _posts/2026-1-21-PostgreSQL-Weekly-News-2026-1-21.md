---
layout: post
title: PostgreSQL 每周新闻 2026-1-21
---
### PostgreSQL每周新闻#632 - 2026年1月21日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/632)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/amnmicjwg1jkbgmuf3ya.jpg)

## [非常规的 Postgres 优化技术](https://postgresweekly.com/link/179508/rss)

又一篇来自 Haki Benita 的精彩文章。这次，他探讨了一些不寻常的优化技术，包括使用 `constraint_exclusion` 在查询与 `CHECK` 约束冲突时跳过扫描、通过索引低基数表达式（如将时间戳截断为日期）来构建更小的索引，以及通过排除约束使用哈希索引来强制唯一性。

**Haki Benita**


## [POSETTE 2026 — CFP 截止日期 2月1日](https://postgresweekly.com/link/179507/rss)

[POSETTE: An Event for Postgres](https://postgresweekly.com/link/179509/rss)，由 Microsoft 的 Postgres 团队组织的免费虚拟开发者活动，将于 6月16-18日举行。鼓励新老讲者提交演讲！不要拖延——CFP 将于 2月1日截止。[获取详细信息](https://postgresweekly.com/link/179507/rss)。

**Microsoft** 赞助商


## [软删除的挑战](https://postgresweekly.com/link/179510/rss)

删除还是不删除，这是个问题！如果你想在表中"删除"数据而不真正丢失它，使用布尔值或日期标志的"软"删除是常见解决方案，但这篇文章考虑了一些替代方案，如使用触发器将行移动到归档表，或从 WAL 捕获已删除的行以进行外部归档。

**atlas9**


**简讯：**

- Robert Haas 整理了他的[2025年度 Postgres 贡献者名单](https://postgresweekly.com/link/179511/rss)。自2024年名单以来，出现了几个新名字，包括 Dmitry Koval（实现了 [ALTER TABLE .. MERGE PARTITIONS](https://postgresweekly.com/link/179512/rss)）、Sami Imseih 和 Greg Burd。

- Microsoft 年度 [POSETTE](https://postgresweekly.com/link/179513/rss) 虚拟 Postgres 会议的 CFP 将于2月1日截止。Microsoft 的 Gauri Kasar [分享了一些制作强有力提案的建议](https://postgresweekly.com/link/179514/rss)。

- 🇫🇮 [Nordic PGDay 2026](https://postgresweekly.com/link/179515/rss) 将于今年3月24日在芬兰赫尔辛基举行。


## [🎤 '我如何开始使用 DBtune 以及为什么我们选择 Postgres'](https://postgresweekly.com/link/179516/rss)

DBtune 创始人兼斯坦福研究员 Luigi Nardi 加入 Claire Giordano，讨论他的开发者和研究之旅，为什么 DBtune 选择数据库调优和 Postgres 作为重点，以及数据库管理和调优"五级"自治的概念。如果你更喜欢阅读而不是听，还有[完整文字记录](https://postgresweekly.com/link/179517/rss)。

**Talking Postgres Podcast**


## [在 PostgreSQL 上将向量搜索扩展到10亿](https://postgresweekly.com/link/179518/rss)

具体来说是10亿个向量。这本质上是对 [VectorChord 1.0](https://postgresweekly.com/link/179519/rss) 的基准测试，这是一个用于高规模向量相似性搜索的扩展（[GitHub 仓库](https://postgresweekly.com/link/179520/rss)）。

**Junyu Chen (VectorChord)**


## [▶ PostgreSQL 18 的新特性](https://postgresweekly.com/link/179521/rss)

[PGX](https://postgresweekly.com/link/179522/rss) 的 CEO Christophe Pettus 最近为旧金山湾区 PostgreSQL 用户组做了一次演讲，在30分钟内总结了 Postgres 18 的一些增强功能。

**Christophe Pettus**


📄 [Postgres Serials 应该是 BIGINT（以及如何迁移）](https://postgresweekly.com/link/179523/rss) — Elizabeth Christensen

📄 [理解分区表上的 `ALTER TABLE` 行为](https://postgresweekly.com/link/179524/rss) — Chao Li


## 📰 分类广告：

[通过 PostgreSQL 18 将查询速度提升3倍](https://postgresweekly.com/link/179580/rss)。了解 AIO、Skip Scan 和复制增强。[立即注册！](https://postgresweekly.com/link/179580/rss)

🛠️ Auth0 for AI Agents 为开发者提供了一个基础，可以在不影响安全性或创新的情况下构建 AI 代理。[开始构建](https://postgresweekly.com/link/179526/rss)。


## 🛠 代码和工具

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/gr2dhjbpo0fskzro2z37.jpg)

- [SQL Shader](https://postgresweekly.com/link/179527/rss)（上图）是 Matias Gonzalez 的一个有趣实验，它将带有 `x`、`y` 和 `value` 列的 Postgres 查询输出渲染到类似着色器的画布上。[更多信息在这里](https://postgresweekly.com/link/179528/rss)。

- [credcheck 4.4](https://postgresweekly.com/link/179529/rss) – 在用户创建、重命名以及密码更改期间执行凭据检查和验证的扩展。

- [pgmoneta 0.20.0](https://postgresweekly.com/link/179530/rss) – Postgres 备份/恢复工具，现在支持 Grafana 12，改进了 S3 支持和更好的锁定。

- [pgBackRest 2.58.0](https://postgresweekly.com/link/179531/rss) – 另一个流行的备份工具，现在支持 S3、GCS 和 Azure 的 HTTP。

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/vwchrnzyx0prw7llibtd.jpg)

- 📊 [Postgres Explain Visualizer 2 1.20](https://postgresweekly.com/link/179532/rss) – 用于可视化 Postgres 执行计划的 Vue.js 组件（上图）。现在支持暗黑模式。

- [SQLPage 0.42](https://postgresweekly.com/link/179533/rss) – Rust 驱动的纯 SQL 数据应用构建器，可在 SQL 查询之上自动构建 UI。

- [pgschema 1.6.1](https://postgresweekly.com/link/179534/rss) – Terraform 风格的声明式 Postgres 模式迁移工具。

- [Rbatis v4.7.0](https://postgresweekly.com/link/179535/rss) – 高性能 Rust"编译时"ORM，具有动态 SQL 生成和异步支持。

- 📊 [pgmetrics v1.19.0](https://postgresweekly.com/link/179536/rss) – 收集和报告 Postgres 指标，用于脚本编写、自动化和故障排除。