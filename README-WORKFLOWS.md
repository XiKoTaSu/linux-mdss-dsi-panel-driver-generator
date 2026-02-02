# Panel Driver Generator

> 简单几步，自动生成Linux面板驱动

## 🎯 快速使用

### 1. 上传文件
将你的文件上传到仓库input文件夹：
- **FDT文件**：生成面板驱动
- **DT.IMG文件**：分解QCDT镜像

### 2. 运行工作流
1. 进入仓库的 **Actions** 页面
2. 选择 **Panel Driver Generator CI**
3. 点击 **Run workflow**
4. 输入文件名：
   - `fdt_filename`：FDT文件名（可选）
   - `dtimg_filename`：DT.IMG文件名（可选）
5. 点击 **Run workflow**

### 3. 下载结果
工作流完成后，在 **Releases** 页面下载处理结果。

## 📁 文件说明

### 输入文件
- **FDT文件**：`.dts` 或 `.dtb` 格式
- **DT.IMG文件**：QCDT格式（包含多个dtb）

### 输出文件
处理完成后包含：
- 面板驱动代码（.c/.h文件）
- 设备树文件
- 相关配置文件

## ⚙️ 注意事项
- DT.IMG是QCDT格式，由多个dtb组成
- 只需输入文件名，无需完整路径
- 结果自动打包发布
