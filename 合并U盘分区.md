# 合并 U 盘分区

打开 cmd，依次输入以下命令：

1. 进入磁盘部分交互环境:

   ```bash
   diskpart
   ```

2. 显示所有的磁盘:

   ```bash
   list disk
   ```

3. 选定U盘，存储设备编号的取值范围是0、1、2:

   ```bash
   sel disk 2
   ```

4. 删除磁盘下的所有分区:

   ```bash
   clean
   ```

5. 在磁盘下创建一个主分区:

   ```bash
   create partition primary
   ```

6. 激活主分区:

   ```bash
   active
   ```

7. 快速格式化主分区为fat32格式:

   ```bash
   format fs=fat32 quick
   ```
