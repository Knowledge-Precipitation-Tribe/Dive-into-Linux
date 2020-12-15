# 文件操作命令

## 文件标识符含义

![&#x6765;&#x6E90;&#xFF1A;https://blog.csdn.net/zhuoya\_/article/details/77418413](../.gitbook/assets/image%20%2813%29.png)

Linux中以`.`开头的文件为隐藏文件

## 拷贝文件或目录

```text
cp [选项] [原文件或目录] [目标目录]
```

选项中：

* -r复制目录
* -p连带文件属性一起复制
* -d若原文件是链接文件则复制链接属性
* -a相当于-pdr

## 移动文件或目录

```text
mv [选项] [源文件或目录] [目标目录]
```

选项中：

* **-b**: 当目标文件或目录存在时，在执行覆盖前，会为其创建一个备份。
* **-i**: 如果指定移动的源目录或文件与目标的目录或文件同名，则会先询问是否覆盖旧文件，输入 y 表示直接覆盖，输入 n 表示取消该操作。
* **-f**: 如果指定移动的源目录或文件与目标的目录或文件同名，不会询问，直接覆盖旧文件。
* **-n**: 不要覆盖任何已存在的文件或目录。
* **-u**：当源文件比目标文件新或者目标文件不存在时，才执行移动操作。

通过mv命令还可以实现重命名操作。

## 删除文件

```text
rm [-rf] [文件名/目录名]
```

其中：

* -r代表删除目录
* -f代表强制删除

## 软连接

为了省下存储空间，都会使用链接的方式来对资源进行饮用，类似于在Windows系列中我们可以使用快捷方式，在mac和Linux中我们我们可以使用软链接的方式。

### 创建软链接

命令格式

```bash
ln  -s  [源文件或目录]  [目标文件或目录]
```

例如：

当前路径创建test 引向/var/www/test 文件夹 

```bash
ln –s  /var/www/test  test
```

创建/var/test 引向/var/www/test 文件夹 

```bash
ln –s  /var/www/test   /var/test 
```

### 删除软链接

和删除普通的文件是一眼的，删除都是使用rm来进行操作

```bash
rm –rf 软链接名称
```

例如：

删除test

```bash
rm –rf test
```

### 修改软链接

```bash
ln –snf  [新的源文件或目录]  [目标文件或目录]
```

这将会修改原有的链接地址为新的地址

例如：

创建一个软链接

```bash
ln –s  /var/www/test   /var/test
```

修改指向的新路径

```bash
ln –snf  /var/www/test1   /var/test
```

## 硬链接

{% embed url="https://www.ibm.com/developerworks/cn/linux/l-cn-hardandsymb-links/" %}

\_\_

