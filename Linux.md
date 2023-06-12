# Linux命令行学习

* 简介
    * 这里学习Linux，主要是指学习Linux命令行的操作。
    * 为什么要学习Linux命令行？ 现在主流的后端服务器都是以Linux为内核的操作系统，因此无论是做后端开发，还是跑机器学习的训练任务，学习Linux命令行是必须的，没有其它选择。

* 常用命令行学习

   * cd, 全称change directory, 后面跟随相对路径或者绝对路径，点击enter之后，就进入相应的文件夹。下面是常见例子。<br />
    
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

   * ls, 全称list，列举出当前文件夹的文件和文件夹内容
    
```console
# 这里的ls带有三个参数，l 代表long list(包含更多有关文件的信息如权限等), h代表human readable（文件大小转为MB）, a代表所有文件（包括隐藏文件）
goodnlp@linux:~$ ls -lha
```

   * pwd
    
```console
# 查看当前文件夹路径，不迷路。
goodnlp@linux:~$ pwd
```

   * du, df

    
```console
# disk used, 计算磁盘使用的的空间，它是直接统计各文件各目录的大小得来的信息
goodnlp@linux:~$ du
```

```console
# disk free, 计算磁盘空闲的的空间，它是通过文件系统磁盘块分配图进行计算出的信息
goodnlp@linux:~$ df
```


   * top，查看正在运行的进程，占用的cpu和内存资源。
    
```console
goodnlp@linux:~$ top
```

   * ps aux
 
```console
# 查看系统所有运行的进程cpu和内存的使用量,进程号pid
goodnlp@linux:~$ ps aux
```

```console
# 查看系统所有python的进程cpu和内存的使用量
goodnlp@linux:~$ ps aux|grep python
```


   * cp

```console
# 复制文件或者文件夹
goodnlp@linux:~$ cp file1 file2
```

   * mv
```console
# 移动文件或者文件夹
goodnlp@linux:~$ mv file1 ./folder
```

   * rm
```console
# 删除文件
goodnlp@linux:~$ rm file1
```

```console
# 删除文件夹
goodnlp@linux:~$ rm -r folder1
```

   * mkdir

```console
# 新建文件夹
goodnlp@linux:~$ mkdir folder1
```

   * chmod

```console
# 改变对一个文件的权限
goodnlp@linux:~$ chmod 777 file1
```

