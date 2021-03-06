# Python 命令速查

## 区分 Python 2.X & Python 3.X 运行环境

笔记:
为了以 Python 2.X 环境运行程序，可在程序第一行加入 `#! python2` 或不加入运行环境生命；同时，为了在 Python 2.X 中使用中文，应在下一行输入 `# -*- coding: utf-8 -*-` 或 `# coding=utf-8`。
为了以 Python 3.X 环境运行程序，应在程序第一行加入 `#! python3`。

## 合并&拆分字符串

笔记:
利用 `join()` 函数可以合并字符串。在函数前可以加上一个 `"` 括住的字符，（例如空格 ` `）如此一来，合并好的字符串会包含空格，用以分隔各个来自旧有字符串的元素。

> \>>> list = ['I','like','cats']

> \>>> "\*".join(list)

> 'I\*like\*cats'

笔记:
利用 `split()` 函数可以将一个字符串分割为几个字符串。这个函数可以包含两个参数，其一为分隔符（例如 `","`），代表用来分割字符串的符号；另一个是索引参数，用来表示要分割第几个分割符前的元素（其中 `0` 为不分割，`-1` 为分隔全部元素，如果这个参数缺省的话，也代表要分割全部元素）。

> \>>> str = "I\*like\*cats"

> \>>> str.split("\*")

> ['I like cats']

> \>>> str.split("\*",1)

> ['I', 'like cats']

## 时间、日期函数及其运算

说明:
使用前需先引入事件模块 `import time`，然后利用 `strftime()` 函数调用当前时间。`strftime()` 函数可以指定调用时间的格式。

> \>>> import time

> \>>> year=time.strftime('%Y')
 
<center>
`%Y` 用四位数表示的年份 `%y` 用两位数表示的年份

`%m` 月份 `%B` 月份（文字形式）`%b` 月份（文字缩写形式）

`%d` 日 `%A` 星期中的日（文字形式）`%a` 星期中的日（文字缩写形式）

`%H` 时（24 时制） `%I` 时（12 时制）`%p` 上下午 `%M` 分 `%S` 秒 `%c` 完整日期&时间（文字形式）

`%j` 一年中的天数 `%w` 一年中的星期数

`%x` 当前日期 `%X` 当前时间 `%Z` 当前时区
</center>

## 列表&数组

