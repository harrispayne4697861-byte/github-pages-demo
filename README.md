# GitHub Pages 部署示例

这是一个最小静态网页，用来验证 GitHub 到 GitHub Pages 的自动部署链路。

## 发布内容

网页只从 `site/` 文件夹发布，因此仓库中的工作流、说明文件不会作为网站内容公开。

## 首次设置

1. 打开仓库的 **Settings → Pages**，将 **Build and deployment → Source** 设为 **GitHub Actions**。
2. 打开仓库的 **Actions** 页面，确认 `Deploy static site to GitHub Pages` 成功。
3. 在 **Settings → Pages** 中打开生成的网站链接。

以后每次推送到 `main`，GitHub Actions 会自动重新发布 `site/`。

## 权限范围

工作流只授予读取仓库内容、发布 Pages 和获取部署身份令牌所需的权限；没有仓库写入权限，也不需要保存部署密钥。
