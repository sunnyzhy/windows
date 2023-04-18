# FAQ

## U 盘安装 win11 提示找不到 install.wim 文件

解决方法:

1. 转换 U 盘分区格式，以管理员身份运行 cmd：

   ```bash
   convert X：/FS:NTFS
   ```
2. 把 ISO 镜像中的 ```sources/install.wim``` 文件直接拷贝或覆盖到 U 盘的 ```sources``` 目录里
