---
title: SQLite数据库介绍
published: 2025-07-16
description: SQLite轻量级数据库
image: "https://cdn.jsdelivr.net/gh/YAO-JIAYE/my_imgs_repo@main/imgs/20250716143435466.png"
tags: [SQL]
category: 工具
draft: false
---


## 介绍:什么是 SQLite？

SQLite 是一个 C 语言库，它实现了一个 `小型`、 `快速`、 `独立`、 `高可靠性`且 功能齐全的SQL 数据库引擎。SQLite 是世界上使用最广泛的数据库引擎。SQLite 内置于所有手机和大多数计算机中，并且与人们日常使用的无数其他应用程序捆绑在一起。 更多信息...

SQLite文件格式稳定、跨平台且向后兼容，开发人员承诺在 2050 年之前保持这种状态。SQLite 数据库文件通常用作在系统之间传输丰富内容的容器 ，也用作数据的长期存档格式 。目前有超过 1 万亿 (1e12) 个 SQLite 数据库正在使用中 。

SQLite源代码 属于公共领域，任何人都可以免费将其用于任何目的。

## 如何下载使用

[SQLite下载地址](https://www.sqlite.org/download.html)

![](https://cdn.jsdelivr.net/gh/YAO-JIAYE/my_imgs_repo@main/imgs/20250716145159242.png)

把这两包下载解压到同一目录

![](https://cdn.jsdelivr.net/gh/YAO-JIAYE/my_imgs_repo@main/imgs/20250716145303438.png)

双击运行`sqlite3.exe`

```sqlite
sqlite> .open test.db
sqlite> create table Students(ID INT PRIMARY KEY NOT NULL,Name VARCHAR(20),Age INT,Address VARCHAR(50));
sqlite> INSERT INTO Students(ID,Name,Age,Address) VALUES (1,'Tom',20,'HANG ZHOU');
sqlite> select * from Students;
1|Tom|20|HANG ZHOU
```

这样就创建好了`test.db`,并创建了一张表，往里面存了点数据

## 使用navicat打开SQLite

![](https://cdn.jsdelivr.net/gh/YAO-JIAYE/my_imgs_repo@main/imgs/image-20250716150609316.png)