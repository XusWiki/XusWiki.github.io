# Python `os` 模块中关于**文件／路径**常用的函数使用方法

函数名|使用方法
---|---
`getcwd()`|返回当前工作目录
`chdir(path)`|改变工作目录
`listdir(path='.')`|列举指定目录中的文件名（'.'表示当前目录，'..'表示上一级目录）
`mkdir(path)`|创建单层目录，如该目录已存在抛出异常
`makedirs(path)`|递归创建多层目录，如该目录已存在抛出异常，注意：'E:\\a\\b'和'E:\\a\\c'并不会冲突
`remove(path)`|删除文件
`rmdir(path)`|删除单层目录，如该目录非空则抛出异常
`removedirs(path)`|递归删除目录，从子目录到父目录逐层尝试删除，遇到目录非空则抛出异常
`rename(old, new)`|将文件old重命名为new
`system(command)`|运行系统的shell命令
`walk(top)`|遍历top路径以下所有的子目录，返回一个三元组：(路径, [包含目录], [包含文件])

函数可使用定义|定义
---|---
`os.curdir`|指代当前目录（'.'）
`os.pardir`|指代上一级目录（'..'）
`os.sep`|输出操作系统特定的路径分隔符（Win下为'\\'，Linux下为'/'）
`os.linesep`|当前平台使用的行终止符（Win下为'\r\n'，Linux下为'\n'）
`os.name`|指代当前使用的操作系统（包括：'posix',&nbsp;&nbsp;'nt', 'mac', 'os2', 'ce', 'java'）