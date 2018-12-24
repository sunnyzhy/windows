# 使用命令来重新获取30天权限
1. 以管理员权限运行cmd.exe

2. 在命令行中输入"SLMGR -REARM "，注意空格

3. 点击Eenter

4. 重启电脑

**该步骤只能使用三次，三次之后再使用就会出现"已超过重新整理的最大允许数量。"**

# 解决上一步无效的方法
1. 打开注册表

2. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsNT\CurrentVersion\SoftwareProtecionPlaform\

3. 双击"SkipRearm"，把数"数值数据"改为"1"
