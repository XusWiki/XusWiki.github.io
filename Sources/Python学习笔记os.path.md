# `os.path` 模块中关于**路径**常用的函数使用方法

函数名|使用方法
`basename(path)`|去掉目录路径，单独返回文件名
`dirname(path)`|去掉文件名，单独返回目录路径
`join(path1[, path2[, ...]])`|将path1, path2各部分组合成一个路径名
`split(path)`|分割文件名与路径，返回(f_path, f_name)元组。如果完全使用目录，它也会将最后一个目录作为文件名分离，且不会判断文件或者目录是否存在
`splitext(path)`|分离文件名与扩展名，返回(f_name, f_extension)元组
`getsize(file)`|返回指定文件的尺寸，单位是字节
`getatime(file)`|返回指定文件最近的访问时间（浮点型秒数，可用time模块的gmtime()或localtime()函数换算）
`getctime(file)`|返回指定文件的创建时间（浮点型秒数，可用time模块的gmtime()或localtime()函数换算）
`getmtime(file)`|返回指定文件最新的修改时间（浮点型秒数，可用time模块的gmtime()或localtime()函数换算）
`exists(path)`|判断指定路径（目录或文件）是否存在（返回 True 或 False）
`isabs(path)`|判断指定路径是否为绝对路径（返回 True 或 False）
`isdir(path)`|判断指定路径是否存在且是一个目录（返回 True 或 False）
`isfile(path)`|判断指定路径是否存在且是一个文件（返回 True 或 False）
`islink(path)`|判断指定路径是否存在且是一个符号链接（返回 True 或 False）
`ismount(path)`|判断指定路径是否存在且是一个挂载点（返回 True 或 False）
`samefile(path1, paht2)`|判断path1和path2两个路径是否指向同一个文件（返回 True 或 False）