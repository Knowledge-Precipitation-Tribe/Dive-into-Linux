# 查找文件

## which（寻找“执行文件”）

```text
which [-a] command
```

参数：

* a：将所有由PATH目录中可以找到的命令均列出，而不只第一个被找到的命令名称

查找文件（find不常用，其他两个命令利用数据库效率高） 

## whereis（寻找特定文件） 

```text
whereis [-bmsu] 文件或目录名 
```

参数： 

* b：只找二进制格式的文件 
* m：只找在说明文件manual路径下的文件 
* s： 只找source源文件 
* u：查找不在上述三个选项当中的其他特殊文件名

## locate（寻找文件）

```text
locate [-ir] keyword 
```

参数： 

* i：忽略大小写的差异 
* r：后面可接正则表达式的显示方式

## find（寻找文件） 

```text
find [PATH] [option] [action]
```

