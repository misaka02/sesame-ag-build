# Sesame-AG Auto Build (免密构建版)

本项目为 [Sesame-AG/Sesame-AG](https://github.com/Sesame-AG/Sesame-AG) 的自动化免密构建与发布仓库。

## 项目特点

1. **自动同步与构建**：定时监听或手动触发拉取上游官方最新发布版本/Tag。
2. **完全免密**：去除官方 Action 中对 ZIP 压缩包添加的密码保护，生成原生免密 ZIP 与直接可用的 APK 文件。
3. **标准自签名**：使用标准 Android 密钥工具签名（支持 v1 + v2 + v3 签名方案），确保可在 Android 8.0+ 及各类系统、Xposed/LSPosed 环境下直接安装与使用。
4. **多架构全覆盖**：提供 `arm64-v8a`、`armeabi-v7a`、`x86`、`x86_64` 及 `universal` 全架构安装包。

## 下载 Release

直接前往 [Releases 页面](../../releases) 下载最新版本的 APK 或免密 ZIP 压缩包。

## 手动触发构建

1. 点击仓库顶部的 **Actions** 选项卡。
2. 在左侧选择 **Build Sesame-AG (Unencrypted)**。
3. 点击右侧 **Run workflow**：
   - 输入需要构建的 Tag（例如 `4380-0.2.6`，留空默认获取最新发布版本）。
   - 点击 **Run workflow** 即可开始构建。
