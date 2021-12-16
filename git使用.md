- 仓库（Repository）
  - 仓库用来存放项目代码，每个项目对应一个仓库，多个开源项目则有多个仓库

- 收藏（start）

  - 收藏项目，方便下次查看

  复制克隆项目（fork）

![image-20211213104141434](https://typora01c.oss-cn-guangzhou.aliyuncs.com/image-20211213104141434.png)



- 发起请求（push request）

- 关注（watch）
  - 关注项目，当项目更新可以接收到通知

- 事务片卡（issue）
  - 发现代码



# 创建仓库

![image-20211215162151096](https://typora01c.oss-cn-guangzhou.aliyuncs.com/image-20211215162151096.png)

![image-20211215162355968](https://typora01c.oss-cn-guangzhou.aliyuncs.com/image-20211215162355968.png)



# 命令行操作

# Git初始化及仓库创建和操作

1、设置用户名

```
git config --global user.name 'chenjz'
```

2、设置用户名邮箱

```
git config --global user.email '1414116842@qq.com'
```

3、查看设置

```
git config --list
```

查看用户名和邮箱

```
git config user.name
git config user.email
```



# 初始化一个新的Git仓库

1、创建文件夹

```
mkdir test
```

![](https://typora01c.oss-cn-guangzhou.aliyuncs.com/image-20211215225444030.png)



2、初始化仓库

![image-20211215225807746](https://typora01c.oss-cn-guangzhou.aliyuncs.com/image-20211215225807746.png)



3、向仓库中添加文件

```
touch a1.php
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        a1.php

nothing added to commit but untracked files present (use "git add" to track)
```

![](https://typora01c.oss-cn-guangzhou.aliyuncs.com/image-20211215230642342.png)

4、添加暂存区

```
git add a1.php
```

![image-20211215231130551](https://typora01c.oss-cn-guangzhou.aliyuncs.com/image-20211215231130551.png)



5、将文件从暂存区提交到仓库

```
git commit -m 'add a1.php'
```

![image-20211215235201109](https://typora01c.oss-cn-guangzhou.aliyuncs.com/image-20211215235201109.png)



# 修改仓库文件



```
echo 1111 > a1.php
git status
```

![image-20211215235657657](https://typora01c.oss-cn-guangzhou.aliyuncs.com/image-20211215235657657.png)



```
git add a1.php
```

![image-20211216000208167](https://typora01c.oss-cn-guangzhou.aliyuncs.com/image-20211216000208167.png)

提交到仓库

```
git commit -m '修改文件内容提交到仓库'
```

![image-20211216000444329](https://typora01c.oss-cn-guangzhou.aliyuncs.com/image-20211216000444329.png)



# 删除文件

1、删除文件

```
rm -rf a1.php
```

2、从git中删除文件

```
git rm a1.php
```

![image-20211216001132122](https://typora01c.oss-cn-guangzhou.aliyuncs.com/image-20211216001132122.png)



3、提交操作

```
git commit -m '删除了a1.php文件'
```

![image-20211216001106492](https://typora01c.oss-cn-guangzhou.aliyuncs.com/image-20211216001106492.png)



# 远程仓库管理

![image-20211216001931443](https://typora01c.oss-cn-guangzhou.aliyuncs.com/image-20211216001931443.png)



![image-20211216002102186](https://typora01c.oss-cn-guangzhou.aliyuncs.com/image-20211216002102186.png)



Git克隆操作

目的

将远程仓库复制到本地

git clone 仓库地址

git clone https://github.com/chenjzgit2/repo2.git

![image-20211216003459973](https://typora01c.oss-cn-guangzhou.aliyuncs.com/image-20211216003459973.png)

