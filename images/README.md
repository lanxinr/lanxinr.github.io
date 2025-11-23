# 图片下载说明

由于 Google Sites 的图片 URL 需要认证权限，无法直接通过命令行下载。

## 手动下载图片的方法

如果您想将图片保存到本地，请按照以下步骤操作：

1. **打开原始网站**：访问 https://www.lanxinr.com/home

2. **右键点击图片**，选择"图片另存为"或"Save image as"

3. **保存到 images 目录**，文件名如下：
   - `hero-background.jpg` - 页面顶部的背景图片
   - `behaviorism.jpg` - Behaviorism 部分的图片
   - `cognitivism.jpg` - Cognitivism 部分的图片
   - `social-learning.jpg` - Social Learning 部分的图片

4. **更新 HTML 文件**：下载图片后，需要将 `home.html` 中的图片 URL 替换为本地路径：
   - 将 `https://lh3.googleusercontent.com/...` 替换为 `images/文件名.jpg`

## 当前状态

目前 `home.html` 使用的是原始 Google 图片 URL，这样可以确保图片正常显示（需要网络连接）。

如果您已经手动下载了图片，可以修改 `home.html` 中的图片路径为本地路径。

