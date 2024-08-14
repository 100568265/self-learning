# 1.交叉编译sqlite3程序



### 1.下载源码

链接: [http://www.sqlite.org/download.html](https://cloud.tencent.com/developer/tools/blog-entry?target=http%3A%2F%2Fwww.sqlite.org%2Fdownload.html&source=article&objectId=2164569)

下载`sqlite-autoconf-3270200.tar.gz`



### 2.生成Makefile

解压并进入源码目录

```shell
tar xvf sqlite-autoconf-3270200.tar.gz
cd sqlite-autoconf-3270200
```



## 3.生成Makefile文件

> --host=交叉编译工具链的前缀 --prefix=编译安装的目录./configure --host=arm-none-linux-gnueabi --prefix=~/sqlite3-arm





### 4.编译安装

```shell
make -j4
make install
```





## 5.移植

1.将bin下的sqlite3可执行文件复制到开发板rootfs的/usr/bin目录下

2.将include下的所有文件复制到开发板rootfs的/usr/include目录下，如果没有该目录则创建

3.将lib下的所有文件复制到开发板rootfs的/usr/lib目录下