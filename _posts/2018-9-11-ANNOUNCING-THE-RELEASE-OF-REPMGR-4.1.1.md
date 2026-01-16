---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: REPMGR 4.1.1 的发布公告
---
英文原文地址：[点击这里](https://www.postgresql.org/about/news/1884/)

由2ndQuadrant Ltd发布于2018-09-05
英国牛津 - 2018年9月5日

2ndQuadrant今天宣布发布[repmgr 4.1.1](https://www.2ndquadrant.com/en/resources/repmgr/)

repmgr是PostgreSQL复制和故障转移管理最流行的工具。它增强并补充了PostgreSQL中的内置复制功能;便于设置和管理备用服务器，检查复制状态以及执行切换操作等管理任务。 repmgrd守护程序提供自动故障转移功能，可最大限度地延长数据库正常运行时间，并可轻松与其他工具（如PgBouncer）集成，以实现高应用程序可用性。

软件包可通过2ndQuadrant的公共RPM和APT存储库获得。安装包文档可在[此处](https://repmgr.org/docs/4.1.1/installation-packages.html)获得。

repmgr 4.1.1提供了以下可用性增强功能：

* repmgr standby switchover --dry-run不再复制外部配置文件以测试它们是否可以复制;这可以避免对目标系统进行任何更改。
* repmgr集群清理现在包括cluster_cleanup事件。
* repmgr待机切换改进了免费walsenders的检测。
* 改进了repmgr待机期间发出的消息。

此版本为repmgrd提供了重要的增强功能，例如：
* 始终在收到SIGHUP后重新打开日志文件，之前只有在检测到配置文件更改时才会发生这种情况。
* 记录器初始化后报告版本号。
* 改进的级联备用故障转移处理。
* 在短暂的网络中断后改进了重新连接处理 - 如果正在收集监控数据，这可能会导致主要的孤立会话。
* 检查promote_command和follow_command是在重新加载配置时定义的。这些在启动时检查但未由repmgrd重新加载，从而可以使用无效值构建repmgrd。

有关所有更改，增强功能和错误修复的详细列表，请阅读[此处的完整发行说明](https://repmgr.org/docs/4.1/release-4.1.1.html)。

我们建议您尽快升级到此版本。此版本可以作为repmgr 4.x的简单包升级安装。

可以在此处下载[源文件](https://repmgr.org/download/repmgr-4.1.1.tar.gz)，此处提供[安装说明](https://repmgr.org/docs/4.1/installation.html)。

repmgr根据GPL v3分发。

欲了解更多信息，请发送电子邮件至[info@2ndQuadrant.com](mailto://info@2ndQuadrant.com)
