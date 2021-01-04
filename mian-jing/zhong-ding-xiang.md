# 重定向

## 重定向符号

| 符号 | 含义 |
| :--- | :--- |
| &gt; | 输出重定向到一个文件或设备，覆盖原来的文件 |
| &gt;! | 输出重定向到一个文件或设备，强制覆盖原来的文件 |
| &gt;&gt; | 输出重定向到一个文件或设备，追加原来的文件 |
| &lt; | 输出重定向到一个程序 |

## 标准错误重定向符号

| 符号 | 含义 |
| :--- | :--- |
| 2&gt; | 将一个标准错误输出重定向到一个文件或设备，覆盖原来的文件 |
| 2&gt;&gt; | 将一个标准错误输出重定向到一个文件或设备，追加到原来的文件 |
| 2&gt;&1 | 将一个标准错误输出重定向到标准输出，1就代表标准输出 |
| &gt;& | 将一个标准错误输出重定向到一个文件或设备，覆盖原来的文件 |
| \|& | 将一个标准错误管道输送到另一个命令作为输入 |
