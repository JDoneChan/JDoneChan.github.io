# JDoneChan 个人博客

基于 [Hugo](https://gohugo.io/) 的个人博客，使用 GitHub Pages 自动部署。

## 本地预览

```bash
hugo server -D
```

打开 `http://localhost:1313/` 预览。

## 发布

将代码推送到 `main` 分支后，`.github/workflows/hugo.yml` 会自动构建并部署到 GitHub Pages。

首次发布前，请在仓库 Settings → Pages → Build and deployment 中将 Source 设置为 **GitHub Actions**。

