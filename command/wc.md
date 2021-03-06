wc
===

统计文件的字节数、字数、行数

## 补充说明

**wc命令** 用来计算数字。利用wc指令我们可以计算文件的Byte数、字数或是列数，若不指定文件名称，或是所给予的文件名为“-”，则wc指令会从标准输入设备读取数据。

### 语法  

```
wc(选项)(参数)
```

### 选项  

```
-c或--bytes或——chars：只显示Bytes数；
-l或——lines：只显示列数；
-w或——words：只显示字数。
```

### 参数  

文件：需要统计的文件列表。

## 例子

```
wc -l *       # 统计当前目录下的所有文件行数
wc -l *.js    # 统计当前目录下的所有 .js 后缀的文件行数
find  . * | xargs wc -l # 当前目录以及子目录的所有文件行数
```

<!-- Linux命令行搜索引擎：https://jaywcjlove.github.io/linux-command/ -->
