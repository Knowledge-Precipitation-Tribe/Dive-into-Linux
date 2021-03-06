# 创建文件与修改文件时间

## 文件的时间类型

| 时间类型 | 解释 |
| :---: | :---: |
| modefication time（mtime） | 当文件内容数据更改时，就会更新这个时间。内容数据指的是文件的内容，而不是文件的属性或权限 |
| status time（ctime） | 当文件的状态改变是，就会更新这个时间。就像文件的权限与属性被修改了，就会更新这个时间 |
| access time（atime） | 当文件的内容被引用时，就会更新这个读取时间。举例来说，当我们使用cat 读取文件内容是，就会更新atime |

## 命令

```bash
touch [-acdmt] 文件 
```

参数解释： 

* -a：仅修改访问时间 
* -c：仅修改文件时间，若该文件不存在则不创建新文件 
* -d：后面可以接想要修改的日期而不用目前的日期，也可以用--date="日期或时间" 
* -m：仅修改mtime 
* -t：后面可以接想要修改的时间而不用目前的时间，格式为\[YYMMDDhhmm\]

在默认状态下，如果touch操作的文件存在则文件的三个时间都会更新为目前的时间，如果该文件不存在，则会主动创建一个新的空文件。

