# Linux入门

Copyright (C) 2022, HITCRT_VISION, all rights reserved.  
Author:BG2EDG(928330305@qq.com)  
Time:2022-06-28  

## Linux、Ubuntu、Shell和Terminal

从技术上来说，李纳斯•托瓦兹开发的 Linux 只是一个内核。**内核（Kernel）指的是一个提供设备驱动、文件系统、进程管理、网络通信等功能的系统软件**，内核并*不是一套完整的操作系统*，它只是操作系统的核心。一些组织或厂商将 Linux 内核与各种软件和文档包装起来，并提供系统安装界面和系统配置、设定与管理工具，就构成了 Linux 的发行版本，Ubuntu就是众多发行版之一。  
Linux 的各个发行版本使用的是同一个 Linux 内核，因此在内核层不存在什么兼容性问题，每个版本有不一样的感觉，只是在发行版本的最外层（由发行商整合开发的应用）才有所体现。我们使用的**Ubuntu是一个以桌面应用为主的Linux操作系统**。Ubuntu基于Debian发行版和Gnome桌面环境，由社区组织维护，完全免费。  
在 Linux 内核的发展过程中，各种 Linux 发行版本起了巨大的作用，正是它们推动了 Linux 的应用，从而让更多的人开始关注 Linux。因此，把 Red Hat、Ubuntu、SUSE 等直接说成 Linux 其实是不确切的，它们是 Linux 的发行版本，更确切地说，应该叫作“以Linux为核心的操作系统软件包”。  
**Shell则是一个命令行解释器**，是Linux内核的一个外壳，负责外界与Linux内核的交互。Shell接收用户或者其他应用程序的命令，然后将这些命令转化成内核能理解的语言并传给内核，内核执行命令完成后将结果返回给用户或者应用程序。  
**终端（Terminal）的作用是提供一个命令的输入输出环境**，在Linux下使用组合键```ctrl+alt+T```打开的就是终端。当你打开一个Terminal时，操作系统会将Terminal和Shell关联起来，当我们在Terminal中输入命令后，Shell就负责解释命令。  

### 总结

+ Linux发行版=Linux内核+软件工具+系统界面  
+ Ubuntu是一个由社区维护的免费Linux发行版  
+ Shell是Kernel和用户之间的桥梁，功能是命令解释器（command Interpreter）  
+ Terminal是提供命令输入输出环境的工具  

## 基本指令

### 必会指令

具体指令操作见黑马教程，要熟练掌握的包含:基本指令中的所有，进阶指令中的管道\|，高级指令ps,top,find,kill,ifconfig,reboot,shutdown,uname,man。其余指令使用频率较低，了解即可。此部分建议在Linux环境下都操作一遍看看有什么效果，如果想了解更多小技巧建议到b站听[[MIT]计算机科学课堂中学不到的知识 The Missing Semester of Your CS Education(2020)](https://www.bilibili.com/video/BV1x7411H7wa?spm_id_from=333.337.search-card.all.click)的前两讲。  

### 注意事项

网上很多教程中可能有诸如 ```vim main.cpp``` 形式的指令，含义是使用vim编辑器打开某个文件。vim编辑器因其充分使用键盘的特点受到众多程序员追捧，但其学习具有一定难度，不建议在竞培营阶段在该方面投入过多精力，后期有兴趣可以自学。遇到该类命令可以利用Ubuntu自带编辑器gedit或vscode打开，即使用  ```gedit main.cpp``` 或   ```code main.cpp```  代替。

## 重要概念

[第5章 用户身份与文件权限 | 《Linux就该这么学》 (linuxprobe.com)](https://www.linuxprobe.com/basic-learning-05.html)

+ [5.1 用户身份与能力](https://www.linuxprobe.com/basic-learning-05.html#51)
+ [5.2 文件权限与归属](https://www.linuxprobe.com/basic-learning-05.html#52)
+ [5.3 文件的特殊权限](https://www.linuxprobe.com/basic-learning-05.html#53)
+ [5.6 su命令与sudo服务](https://www.linuxprobe.com/basic-learning-05.html#56_susudo)
要求：明确常见的用户权限包含哪些，如何变更用户权限，了解chmod和sudo命令的用法
[第6章 存储结构与管理硬盘 | 《Linux就该这么学》 (linuxprobe.com)](https://www.linuxprobe.com/basic-learning-06.html)
+ [6.1 一切从“/”开始](https://www.linuxprobe.com/basic-learning-06.html#61)
+ [6.9 软硬方式链接](https://www.linuxprobe.com/basic-learning-06.html#69)
要求：sudo的用法;“Linux系统中一切皆文件”;软链接添加方法

## 参考资料

[1][shell命令以及运行原理和Linux权限](https://blog.csdn.net/weixin_57675461/article/details/122962403)
[2][终端(terminal)、shell区别与联系](https://blog.csdn.net/weixin_38214171/article/details/90050340)
