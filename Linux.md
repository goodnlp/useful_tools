# Linux命令行学习

* 简介
    * 这里学习Linux，主要是指学习Linux命令行的操作。
    * 为什么要学习Linux命令行？ 现在主流的后端服务器都是以Linux为内核的操作系统，因此无论是做后端开发，还是跑机器学习的训练任务，学习Linux命令行是必须的，没有其它选择。

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
# 停留在当前文件夹
goodnlp@linux:~$ ls -lha
```

(3) pwd
    
```console
# 查看当前文件夹路径，不迷路。
goodnlp@linux:~$ pwd
```

(4) du, df

    
```console
# 停留在当前文件夹
goodnlp@linux:~$ du
```

(5) top，查看正在运行的进程，占用的cpu和内存资源。
    
```console
goodnlp@linux:~$ top
```

(6) ps aux
 
```console
# 查看系统所有运行的进程
goodnlp@linux:~$ ps aux
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
# 删除文件或者文件夹
goodnlp@linux:~$ rm file1
```

(10) mkdir

```console
# 增加文件夹
goodnlp@linux:~$ mkdir folder1
```

(11) chmod

```console
# 改变对一个文件的权限
goodnlp@linux:~$ chmod 777 file1
```

