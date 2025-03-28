# windows 修改环境变量，不重启刷新

修改用户变量:

```bash
setx My_Variable "My_Value"
```

修改系统变量:

```bash
setx My_Variable "My_Value" /M
```

向用户变量的 Path 里添加:

```bash
setx PATH "%PATH%;C:\MyNewPath"
```

向系统变量的 Path 里添加:

```bash
setx PATH "%PATH%;C:\MyNewPath"
```

注意：
- 使用setx命令时，如果你想要在变量值中包含引号，需要使用双引号将整个setx命令及其参数括起来，并且在变量值内部使用单引号。
- setx命令通常不会立即生效，直到重新启动命令提示符窗口或者重新启动计算机

查看系统变量：

```bash
echo %My_Variable%
```
