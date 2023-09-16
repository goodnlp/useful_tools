# Git学习

## Git是什么
* Git是一个分布式的版本控制系统，主要用于记录和追踪文件（尤其是文本文件）的修改。
* Git主要用于软件开发中协调，管理，同步一个团队程序员写代码的过程。

## Git基本概念

作为初学者的话，会被这么多区搞糊涂，其实可以简单理解，这四个区中，只有工作区和远程仓库可以直接被人看到，工作区就是某个文件夹和其中包含的文件内容，
远程仓库就是github.com这个网站上某个repo包含的代码文件等。


* 工作区

workspace, 工作区，就是你平时存放项目代码的地方。


* 暂存区

index或者stage , 暂存区，用于临时存放你的改动，事实上它只是一个文件，保存即将提交到文件列表信息。

* 本地仓库

local repository，就是安全存放数据的位置，这里面有你提交到所有版本的数据。其中HEAD指向最新放入仓库的版本。

* 远程仓库

remote repository，远程仓库，托管代码的服务器，可以简单的认为是你项目组中的一台电脑用于远程数据交换。
通常意义上我们业余使用的是这个网站（www.github.com）, 作为远程仓库，每个人可以通过邮箱注册账号进行使用。<br>
有的公司也会购买github的企业版，就不是这个域名了，但是界面和使用方法几乎一模一样。



## 常用指令

准备：登陆github.com，点击页面右上方的加号，点击“new repository”即可创建远程仓库。
本文以本仓库为例，从远程仓库拷贝一份到本地工作区，然后示范下面各种git有关的命令行。

(1) git clone<br />

打开命令行窗口输入如下命令，就可以将远程仓库拷贝到本地电脑上。使用ls命令就可以看到一个userful_tools的文件夹，cd进入这个文件夹，可以看到这个仓库的各种文件。这个本地文件里面的空间就是我们的工作区了。

```console
git clone https://github.com/goodnlp/useful_tools.git
```

(2) git add <br />

承接上文说的，在工作区，可以用vim practice.txt创建一个新的文本文件，然后使用git add 命令将它加入暂存区。
git add 后面接文件或者文件夹名称，可以把相应文件加入暂存区。

```console
git add practice.txt
```

(3) git commit <br />

git commit 后面接文件或者文件夹名称，可以把相应文件加入本地仓库。

```console
git commit practice.txt -m "add practice.txt"
```

(4) git push origin <br />

上文在本地仓库增加了一个新的文件（类似于在本地写了一些新的代码），现在需要将这一个更新推送到远程仓库，使用如下命令行就可以做到。
其中git push orgin就是将本地更新推送到远程仓库的意思，第一个main是本地仓库的名字，第二个main是远程仓库的名字。

```console
git push origin main:main
```

(5) git fetch<br />
如果远程仓库的某个分支代码有更新（如队友更新了代码），则需要先使用git fetch将更新拿到本地，操作如下。
其中origin指的是远程仓库，main指的是仓库分支的名字。


```console
git fetch origin main
```

(6) git merge<br />
使用git fetch 将远程仓库的更新拿到本地后，使用git merge就可以将本地仓库main 和远程仓库origin/main合并起来。比如
practice.txt增加了一行内容后，本地仓库也会增加这一行内容。

本地如果当前处于main分支，使用git merge origin/main 之后，就是将本地仓库main 和远程仓库origin/main合并起来。

```console
git merge origin/main
```

(7) git branch<br />
使用这个命令就可以看到本地仓库的所有分支，开头带有*的就是当前工作分支。
使用git branch -a可以产看所有本地和远程仓库的分支。

```console
git branch
```

使用git branch dev 就可以穿件名字是dev的新分支

```console
git branch dev
```

(8) git checkout<br />
使用如下命令可以切换到dev分支。

```console
git checkout dev
```

(9) git rm <br />

```console
git rm
```

(10) git mv <br />

```console
git mv
```


## 总结

使用git是一个与团队合作的过程，目的是更规范地管理代码，完成软件开发的目的。
所以这是一个更综合的学习过程，使用git的过程也需要会一些基本的linux命令行技能，和使用Vim创建文件的技能。
通过这个教程，可以更近距离的接触和使用开发工具和工作方式和习惯。




