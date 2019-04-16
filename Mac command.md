## Mac command

### 文件时间

在windows下，一个文件有：创建时间、修改时间、存取时间。而在Linux下，一个文件也有三种时间，分别是：存取时间（Access）、修改时间（Modify）、状态改动时间（Change）。

在Linux下没有创建时间的概念，也就是不能知道文件的建立时间，但如果文件建立后就没有修改过，修改时间=建立时间；如果文件建立后，状态就没有改动过，那么状态改动时间=建立时间；如果文件建立后，没有被读取过，那么存取时间=建立时间，因为不好判断文件是否被改过、读过、状态是否变过，所以判断文件的建立时间基本上不可能。



### touch

#### 功能：

- 更改文档或目录的日期时间，包括存取时间和修改时间。
- 新建一个不存在的文件。

### 实例

#### 创建新文件

```shell
iMacDev110:demo bli$ touch test.txt
```

```shell
iMacDev110:demo bli$ stat -x test.txt 
  File: "test.txt"
  Size: 0            FileType: Regular File
  Mode: (0644/-rw-r--r--)         Uid: (1225361723/     bli)  Gid: (   20/   staff)
Device: 1,6   Inode: 1051771    Links: 1
Access: Tue Apr 16 18:55:01 2019
Modify: Tue Apr 16 18:55:01 2019
Change: Tue Apr 16 18:55:01 2019
```

#### 修改文件的创建时间和修改时间

```shell
iMacDev110:demo bli$ touch -t 201211142234.50 test.txt
```

```shell
iMacDev110:demo bli$ stat -x test.txt 
  File: "test.txt"
  Size: 0            FileType: Regular File
  Mode: (0644/-rw-r--r--)         Uid: (1225361723/     bli)  Gid: (   20/   staff)
Device: 1,6   Inode: 1051771    Links: 1
Access: Wed Nov 14 22:34:50 2012
Modify: Wed Nov 14 22:34:50 2012
Change: Tue Apr 16 19:00:20 2019
```







- open -e
- souce
- echo $JAVA_HOME
- stat