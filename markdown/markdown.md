# Markdown
Markdown 是一种轻量级标记语言，它允许人们使用易读易写的纯文本格式编写文档。

Markdown 语言在 2004 由约翰·格鲁伯（英语：John Gruber）创建。

Markdown 编写的文档可以导出 HTML 、Word、图像、PDF、Epub 等多种格式的文档。

Markdown 编写的文档后缀为 .md, .markdown。
## 标题
Markdown 标题有两种格式。

1. 使用 `=` 和 `-` 标记一级和二级标题
   `=` 和 `-` 标记语法格式如下：
    ```
    我展示的是一级标题
    =================

    我展示的是二级标题
    -----------------
    ```
2. 使用 `#` 号标记
使用 `#` 号可表示 1-6 级标题，一级标题对应一个 `#` 号，二级标题对应两个 `#` 号，以此类推。
```
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
```
## 段落
Markdown 段落没有特殊的格式，直接编写文字就好，段落的换行是使用两个以上空格加上回车。  
当然也可以在段落后面使用一个空行来表示重新开始一个段落。
## 列表
Markdown 支持有序列表和无序列表。

无序列表使用星号`*`、加号`+`或是减号`-`作为列表标记：
```
* 第一项
* 第二项
* 第三项

+ 第一项
+ 第二项
+ 第三项


- 第一项
- 第二项
- 第三项
```
有序列表使用数字并加上 . 号来表示，如：
```
1. 第一项
2. 第二项
3. 第三项
```
## 区块
Markdown 区块引用是在段落开头使用 `>` 符号 ，然后后面紧跟一个空格符号：
```
> 区块引用
```
另外区块是可以嵌套的，一个 `>` 符号是最外层，两个 `>` 符号是第一层嵌套，以此类推：
```
> 最外层
> > 第一层嵌套
> > > 第二层嵌套
```
**区块中使用列表**

    ```
    > 区块中使用列表
    > 1. 第一项
    > 2. 第二项
    > + 第一项
    > + 第二项
    > + 第三项
    ```
**列表中使用区块**
如果要在列表项目内放进区块，那么就需要在 `>` 前添加四个空格的缩进。
    ```
    * 第一项
        > 菜鸟教程
        > 学的不仅是技术更是梦想
    * 第二项
    ```
## 代码块
**单行使用一个反引号**

    ```
    printf函数定义：`printf()`
    ```

**多行使用3个反引号**

    ```
        ```python
        #!/usr/bin/env python
        import os
        import sys

        def dig(domain, server, type):
        ...
        ```
    ```

    > 开始的3个反引号后可以指定代码块语言
## 链接
```
[链接名称](链接地址)

或者

<链接地址>
``` 
**高级链接**
我们可以通过变量来设置一个链接，变量赋值在文档末尾进行：
```
这个链接用 1 作为网址变量 [Google][1]
这个链接用 runoob 作为网址变量 [Runoob][runoob]
然后在文档的结尾为变量赋值（网址）

  [1]: http://www.google.com/
  [runoob]: http://www.runoob.com/
```
## 图片
Markdown 图片语法格式如下：
```
![alt 属性文本](图片地址)

![alt 属性文本](图片地址 "可选标题")
```
> 图片地址可以是本地相对路径
> Markdown图片也支持类似高级链接变量引用的使用方式
## 表格
Markdown 制作表格使用 | 来分隔不同的单元格，使用 - 来分隔表头和其他行。

语法格式如下：
```
|  表头   | 表头  |
|  ----  | ----  |
| 单元格  | 单元格 |
| 单元格  | 单元格 |
```
**我们可以设置表格的对齐方式**

* `-:` 设置内容和标题栏居右对齐。
* `:-` 设置内容和标题栏居左对齐。
* `:-:` 设置内容和标题栏居中对齐。
```
| 左对齐 | 右对齐 | 居中对齐 |
| :-----| ----: | :----: |
| 单元格 | 单元格 | 单元格 |
| 单元格 | 单元格 | 单元格 |
```
## 流程图
* 横向流程图
    ```
        ```mermaid
        graph LR
        A[方形] -->B(圆角)
            B --> C{条件a}
            C -->|a=1| D[结果1]
            C -->|a=2| E[结果2]
            F[横向流程图]
        ```
    ```
* 竖向流程图
    ```
        ```mermaid
        graph TD
        A[方形] --> B(圆角)
            B --> C{条件a}
            C --> |a=1| D[结果1]
            C --> |a=2| E[结果2]
            F[竖向流程图]
        ```
    ```
## 文本格式
* 粗体
    ```
    **我是粗体**
    ```
* 斜体
    ```
    *这是斜体文字* 
    ```
* 自定义字体大小
    ```
    <font size=4>我是变大的字</font>
    ```
* 调整字体大小
    ```
    <small>字体变小</small>
    <big>字体变大</big>
    ```
* HTML标签
    ```
    使用 <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Del</kbd> 重启电脑
    ```
* 特殊符号转义
    ```
    **文本加粗** 
    \*\* 正常显示星号 \*\*
    ```

