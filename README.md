# JDoneChan 个人博客

基于 [Hugo](https://gohugo.io/) 与 [Blowfish](https://blowfish.page/) 的个人博客，使用 GitHub Pages 自动部署。支持全站搜索、文章目录、页内锚点、归档和热门文章展示。

## 本地预览

```bash
hugo server -D
```

打开 `http://localhost:1313/` 预览。

## 发布

将代码推送到 `main` 分支后，`.github/workflows/hugo.yml` 会自动构建并部署到 GitHub Pages。

首次发布前，请在仓库 Settings → Pages → Build and deployment 中将 Source 设置为 **GitHub Actions**。

## 防止敏感信息泄漏

仓库配置了 `.githooks/pre-push` 本地检查和 GitHub Actions Gitleaks 扫描。首次克隆后执行：

```bash
git config core.hooksPath .githooks
```

密钥请存放在 GitHub Actions Secrets 中，不要提交到文章、配置或工作流文件。
