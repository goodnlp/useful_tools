# 开发者实用工具


## 目录
* 引言
* Vim
* Git
* Linux
* 总结

## 引言
* 人工智能时代来临，一起来加入学习AI，变得更强。第一步，掌握一些趁手的工具是必须的，学会下面这些技能，不仅让你“无痛”开发，更能提升工作效率。
* 本项目的目的是提供一个开发者必会的生产力工具教程，包含Vim，Git，Linux。
* 本项目只是一个基本的入门学习上手这些工具的教程，也是笔者在实际工作中的积累，差不都能覆盖绝大部分需求。因为工具使用讲究的是熟能生巧，所以掌握了这些基本的操作使用和熟悉了工具的框架环境，在遇到新的需求可以自行扩展学习在这些工具中的能力就行。<br /> 因此本项目不会囊括一个百科全书式的教程，把使用者吓退，而是提供一个轻松，学习量不大但是刚好够用的教程。



## Vim

## Git


## Linux命令行学习

* 简介
    * 这里学习Linux，主要是指学习Linux命令行的操作。
    * 为什么要学习Linux命令行？ 现在主流的后端服务器都是以Linux为内核的操作系统，开发者首选的mac也是linux命令行操作，因此无论是做后端开发，还是跑机器学习的训练任务，学习Linux命令行是必须的，没有其它选择。

* 常用命令行学习

(1) cd, 全称change directory, 后面跟随相对路径或者绝对路径，点击enter之后，就进入相应的文件夹。下面是常见例子。<br />
    
```console
# 停留在当前文件夹
goodnlp@linux:~$ cd .
```
    
```console
# 回到上一层文件夹
goodnlp@linux:~$ cd ..
```

    
```console
# 回到当前用户的主文件夹
goodnlp@linux:~$ cd ~
```

(2) ls, 全称list，列举出当前文件夹的文件和文件夹内容
    
```console
# 这里的ls带有三个参数，l 代表long list(包含更多有关文件的信息如权限等), h代表human readable（文件大小转为MB）, a代表所有文件（包括隐藏文件）
goodnlp@linux:~$ ls -lha
```

(3) pwd
    
```console
# 查看当前文件夹路径，不迷路。
goodnlp@linux:~$ pwd
```

(4) du, df

    
```console
# disk used, 计算磁盘使用的的空间，它是直接统计各文件各目录的大小得来的信息
goodnlp@linux:~$ du
```

```console
# disk free, 计算磁盘空闲的的空间，它是通过文件系统磁盘块分配图进行计算出的信息
goodnlp@linux:~$ df
```


(5) top，查看正在运行的进程，占用的cpu和内存资源。
    
```console
goodnlp@linux:~$ top
```

(6) ps aux
 
```console
# 查看系统所有运行的进程cpu和内存的使用量,进程号pid
goodnlp@linux:~$ ps aux
```

```console
# 查看系统所有python的进程cpu和内存的使用量
goodnlp@linux:~$ ps aux|grep python
```


(7) cp

```console
# 复制文件或者文件夹
goodnlp@linux:~$ cp file1 file2
```

(8) mv
```console
# 移动文件或者文件夹
goodnlp@linux:~$ mv file1 ./folder
```

(9) rm
```console
# 删除文件
goodnlp@linux:~$ rm file1
```

```console
# 删除文件夹
goodnlp@linux:~$ rm -r folder1
```

(10) mkdir

```console
# 新建文件夹
goodnlp@linux:~$ mkdir folder1
```

(11) chmod

```console
# 改变对一个文件的权限
goodnlp@linux:~$ chmod 777 file1
```



## 总结

以上这三个技能都是基于命令行，也就是在一个黑框框里面输入文字指令，让电脑完成一些操作。
与之相对的是基于图形界面，用户点击就可以完成任务。基于命令行一开始不符合人类的习惯，但是可以完成很多细粒度的精细操作，同时易于批量化和自动化，因此这是值得花精力学习的技能。
学习建议就是，一定要每个命令行都要亲自在电脑上操作，克服新手期的陌生感，用多了就能体会到优越性，越来越喜欢命令行操作，自然而然就掌握甚至擅长这个操作了。

