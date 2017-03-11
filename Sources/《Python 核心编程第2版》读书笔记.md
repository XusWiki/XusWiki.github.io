# 《Python 核心编程 第 2 版》读书笔记
说明:
作者 Wesley J. Chun（陈仲才），人民邮电出版社。适用版本 Python 2.X。

## Python 基础操作

### 变量 & 运算符
变量可以被赋值为：（1）数字变量、（2）字符串、（3）列表、（4）元组<sup>[1]</sup>、（5）字典

`variable = 3.1415926`；变量也可以进行多元赋值，例如：`x, y, z = 1, 2, 3`；多元赋值方法也可用于元组，例如`(x, y, z) = (1, 2, 3)`

数字变量又包含：（1）整数 `int`、（2）长整数 `long`、（3）浮点值 `float`、（4）复数 `complex` 以及（5）布尔值 `bool`。

加|减|乘|除|地板除|取余|乘方|不等
----|----|----|----|----|----|----|----
+|-|\*|/|//|&|**|!=

说明:
Python 2.x 中不等于有两种写法 `!=` 和 `<>`；Python 3.x 只有 `!=` 一种写法。

### 循环 & 条件
if 引导条件语句，意为“一旦……就……”；若有分枝条件，则使用 elif 来引导下一条条件语句；另外，若有备选命令，则使用 else 语句。这一系列命令也被称为“**if-elif-else**”语句。

`if expression:`
　　`if_suite`
`elif expression:`
　　`While_suite`
`else:`
　　`else_suite`

循环分为 while 循环和 for 循环，while 循环规定当满足 while expression 是循环执行命令；for 循环规定当变量在某一序列内时执行命令<sup>[2]</sup>。

`while expression:`
　　`While_suite`

### 文件操作
可以将文件作为变量引用到 Python 程序中，命令为：`variable = open(file_name, access_mode = 'r')`

`file_name` 为文件名；`access_mode` 为访问模式，默认设置为 `r`。

- `r` 为读取模式；
- `w` 为写入模式；
- `+` 为读写模式；
- `b` 为二进制访问模式

### 函数
使用函数处理目标变量的命令为：`function(variable_name)`

另外，也可以定义一个函数：

`def function([arguments]):`
　　`“optional documentation string”`
　　`function_suite`
### 类
创建累命令：
`class ClassName(base_class[es]):`
　　`"optional documentation string"`
　　`static_member_declarations`
　　`method_declarations`
　　
### 模块
导入模块：`import module_name`
一旦模块被导入，就可以将其中的函数直接访问：
`module.function()`
`module.variable`

### 实用函数
- `dir([obj])` 显示对象属性
- `help([obj])` 显示对象文档字符串
- `int(obj)` 将对象转换为整形
- `len(obj)` 返回对象的长度
- `open(fn, mode)` 文件读写操作
- `input(str)` 等待用户输入字符串<sup>[3]</sup>
- `str(obj)` 将对象转换为字符串
- `type(obj)` 返回对象类型

提示:
[1] 字符串、元组、列表都可以被归类为序列。因此这些变量中组成元素的排列顺序是有意义的。
[2] for 条件句可以使用字符串、列表、`range()`、`enumerate()`
[3] 在 Python 2.X 中应当为 `raw_input()`

## Python 基础语法
在 Python 中 `#` 表述注释，程序会自动忽略其后的内容；`\n` 表示换行；`;` 可以把一行内容分割为多个语句；`:` 将代码的头和体分开；使用 `　　`（**缩进**）区分代码块。

### 关键字
Python 关键字备查表：

<center>
[`and`](www.baidu.com) `as`	 `assert` `break`
class	continue		def				del
exec|except|else|elif
finally|for|from|global
if|import|in|is
lambda|not|or|pass
print|raise|return|try
while|with|yield|None
</center>

### Python 模块结构和布局
1. Unix 起始行，向系统说明运行环境 `#/usr/bin/env python`
2. 模块文档，简要介绍模块功能及重要全局变量的含义 `"this is a test module"`
3. 模块导入 `import sys`
4. 变量定义 `debug = True`
5. 类定义语句 `class Fooclass (objectives):` …
6. 函数定义域句 `def test()` …
7. 主程序

## 变量类型：数字
可以调用的数字类型包括整形（`1`）、长整型（`-99999999999L`）<sup>[1]</sup>、布尔型（`bool`）、双精度浮点型（`float`）、十进制浮点型和复数<sup>[1]</sup>。

提示:
[1] 附属包含实部合虚部。关于叙述的讨论见[《虚数的意义，虚数到底是什么》](http://www.guokr.com/post/432219/)。

## 变量类型：序列（一）字符串
## 变量类型：序列（二）列表
## 变量类型：序列（三）元组

## 变量类型（三）字典

