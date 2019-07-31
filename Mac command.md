## Mac command

### 文件时间

在windows下，一个文件有：创建时间、修改时间、存取时间。而在Linux下，一个文件也有三种时间，分别是：存取时间（Access）、修改时间（Modify）、状态改动时间（Change）。

**Access time(atime):**是指取用文件的时间，所谓取用，常见的操作有：使用编辑器查看文件内容，使用cat命令显示文件内容，使用cp命令把该文件（即来源文件）复制成其他文件，或者在这个文件上运用grep sed more less tail head 等命令，凡是读取而不修改文件的操作，均会改变文件的Access time.  

**Modify time(mtime)：**是指修改文件内容的时间，只要文件内容有改动（如使用转向输出或转向附加的方式）或存盘的操作，就会改变文件的 Modify time，**平常我们使用ls –l查看文件时，显示的时间就是Modify time**

**Change time(ctime):**是指文件属性或文件位置改动的时间，如使用 chmod，chown, mv 指令或者使用 ln 做文件的硬是连接，就会改变文件的Change time. 



在Linux下没有创建时间的概念，也就是不能知道文件的建立时间，但如果文件建立后就没有修改过，修改时间=建立时间；如果文件建立后，状态就没有改动过，那么状态改动时间=建立时间；如果文件建立后，没有被读取过，那么存取时间=建立时间，因为不好判断文件是否被改过、读过、状态是否变过，所以判断文件的建立时间基本上不可能。

### stat

#### 功能

- 查看文件信息
- 查看文件系统信息

#### 注意

Mac OS 的 stat 选项与 linux 的选项不同

#### 实例

##### 查看文件信息

```shell
libodeMacBook-Pro:~ gzhennaxia$ stat -x /Users/gzhennaxia/Documents/command.md 
16777221 1873801 -rw-r--r-- 1 gzhennaxia staff 0 3476 "Apr 16 22:21:31 2019" "Apr 16 22:21:30 2019" "Apr 16 22:21:30 2019" "Apr 16 21:28:16 2019" 4096 8 0x40 /Users/gzhennaxia/Documents/GitHub/filebackup/Mac command.md
```

Mac OS 下需要加 -x 选项才能格式化输出

```shell
libodeMacBook-Pro:~ gzhennaxia$ stat -x /Users/gzhennaxia/Documents/command.md 
  File: "/Users/gzhennaxia/Documents/command.md"
  Size: 3794         FileType: Regular File
  Mode: (0644/-rw-r--r--)         Uid: (  501/gzhennaxia)  Gid: (   20/   staff)
Device: 1,5   Inode: 1873850    Links: 1
Access: Tue Apr 16 22:22:11 2019
Modify: Tue Apr 16 22:22:09 2019
Change: Tue Apr 16 22:22:09 2019
```

##### 查看文件修改时间

```shell
libodeMacBook-Pro:~ gzhennaxia$ stat -f %Sm /Users/gzhennaxia/Documents/command.md 
Apr 16 22:34:06 2019
```

### touch

#### 功能：

- 更改文档或目录的日期时间，包括存取时间和修改时间。
- 新建一个不存在的文件。

#### 实例

##### 创建新文件

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

##### 修改文件的创建时间和修改时间

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

### open

#### 功能

- 打开文件
- 在 finder 中打开目录

#### 实例

##### 打开文件

```shell
libodeMacBook-Pro:~ gzhennaxia$ open /Users/Documents/GitHub/text.txt
```

##### 强制使用 TextEdit 打开文件

```shell
libodeMacBook-Pro:~ gzhennaxia$ open -e /Users/Documents/GitHub/text.txt
```

##### 在 finder 中打开目录

```shell
libodeMacBook-Pro:~ gzhennaxia$ open /Users/gzhennaxia/Documents/
```

### souce

#### 作用

- 执行脚本

#### 实例

```shell
libodeMacBook-Pro:~ gzhennaxia$ source .bash_profiles
```

### echo

#### 作用

- 用于字符串的输出

#### 实例

##### 显示变量值

```shell
libodeMacBook-Pro:~ gzhennaxia$ echo $PATH
/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin
```

### pbcopy

#### 作用

- 复制到剪切板

#### 实例

##### 将 SSH 中的公钥复制到剪切板

```shell
$ pbcopy < ~/.ssh/id_rsa.pub
# or
$ cat ~/.ssh/id_rsa.pub | pbcopy
```

