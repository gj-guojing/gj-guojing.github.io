# GitHub Pages 配置指南

## 关键问题

您的网站没有显示 al-folio 模板的原因是：**GitHub Pages 仍然在使用默认的 Jekyll 3.10.0 构建环境**，而不是我们配置的 GitHub Actions 工作流。

## 解决方案

您需要将 GitHub Pages 的 **Source** 设置从 "Deploy from a branch" 改为 **"GitHub Actions"**：

### 步骤 1：进入 GitHub 仓库设置
1. 打开浏览器，访问您的 GitHub 仓库：`https://github.com/gj-guojing/gj-guojing.github.io`
2. 点击仓库顶部的 **Settings** 标签

### 步骤 2：找到 Pages 设置
1. 在左侧边栏中，向下滚动找到 **Code and automation** 部分
2. 点击 **Pages**（如果找不到，可以使用搜索框搜索 "Pages"）

### 步骤 3：更改构建源
在 **Build and deployment** 部分：
1. 找到 **Source** 选项
2. 当前应该是 **"Deploy from a branch"**
3. 点击下拉菜单，选择 **"GitHub Actions"**
4. 页面会显示可用的 GitHub Actions 工作流
5. 确认您的 `deploy.yml` 工作流被识别

### 步骤 4：保存设置
1. 点击 **Save** 或 **Apply** 按钮保存更改
2. GitHub 会提示您更改已保存

## 验证

完成上述设置后：
1. 访问您的网站：`https://gj-guojing.github.io/`
2. 您应该能看到使用 al-folio 模板的新网站
3. 如果仍然看不到，请清除浏览器缓存或等待几分钟

## 常见问题

### 1. 为什么 GitHub Actions 工作流显示成功，但网站没有更新？
- 因为 GitHub Pages 仍然使用默认构建环境，忽略了 GitHub Actions 生成的文件

### 2. 如何检查 GitHub Pages 的构建日志？
- 在 GitHub Pages 设置页面，您可以查看最近的构建日志

### 3. 为什么网站的 URL 显示正确，但内容不正确？
- 因为 `_config.yml` 中的 `url` 和 `baseurl` 配置已经正确，但构建源设置错误

完成上述设置后，您的网站应该能够成功显示 al-folio 模板的内容！