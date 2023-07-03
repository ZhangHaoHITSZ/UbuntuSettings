# Git入门

Copyright (C) 2022, HITCRT_VISION, all rights reserved.  
Author:BG2EDG(928330305@qq.com)  
Time:2022-06-29  

## 必会内容

| git                       |
| ------------------------- |
| git config                |
| git status                |
| git add                   |
| git commit                |
| git push                  |
| git pull                  |
| git branch                |
| git merge                 |
| .gitignore编写            |
| 将本地仓库同步到远程Gitee |

## 教程链接及推荐顺序

&emsp;&emsp;推荐新手从[廖雪峰Git教程开始](https://www.liaoxuefeng.com/wiki/896043488029600/)，包含了绝大多数指令，最好按照他的例程走一遍，然后再看[Gitee的Git教程](https://gitee.com/help/articles/4104)中的[Git 仓库基础操作](https://gitee.com/help/articles/4114)和[Git的基本概念/常用命令及实例](https://gitee.com/help/articles/4110)两篇巩固基本概念。如果有兴趣更深入了解Git,可以去看[Pro Git](https://gitee.com/progit/)。  
&emsp;&emsp;学会Git的基本操作后可以开始尝试[在Gitee上新建仓库](https://gitee.com/help/articles/4105)，过程中可能会需要[配置公钥&私钥](https://blog.csdn.net/Think_kill/article/details/122977468)。

## 注意事项

1. 使用git commit指令时会打开编辑器编辑commit信息，通常默认为vim，使用下面指令可将默认编辑器改为vscode  

    ```bash
    git config --global core.editor "code --wait"

    ```

2. 提交git时检查子目录是否运行过git init，如果运行过则子目录会被当做子模块，提交到远程后可能无法访问，文件夹出现如下形式。
![git嵌套](assets/git_inside_dir.png)
解决方式是在 **子目录下(不是根目录，比如上图中的./camera路径下)** 运行```ls -a```查看有无.git文件夹，如果有运行```rm -rf .git```，在重新commit和push即可。  

## 扩展阅读

一些高级内容，有git使用基础的同学可以试着玩玩，不做要求
[1] [git stash](https://blog.csdn.net/qq_38425719/article/details/107792754)  
[2] [git-commit -- 代码提交风格 -- Commitizen 插件安装与配置（vscode）](https://blog.csdn.net/huaqi_/article/details/122706900)
[3] [git commit 提交信息规范入门(配合vscode)](https://blog.csdn.net/weixin_40780243/article/details/108900691)
[4] [git删除commit的历史大文件记录](https://blog.csdn.net/u011840205/article/details/117479877)
