# 查看进程

## **1. ps**

查看某个时间点的进程信息。

示例：查看自己的进程

```text
## ps -l
```

示例：查看系统所有进程

```text
## ps aux
```

示例：查看特定的进程

```text
## ps aux | grep threadx
```

## **2. pstree**

查看进程树。

示例：查看所有进程树

```text
## pstree -A
```

## **3. top**

实时显示进程信息。

```text
## top -d
```

## **4. netstat**

查看占用端口的进程

示例：查看特定端口的进程

```text
## netstat -anp | grep port
```

