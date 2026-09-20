# 美西朝阳团

这是一个纯静态旅行手册网页，适合通过 GitHub 仓库连接 Cloudflare Pages 发布。

## 项目结构

- `public/index.html`：完整网页
- `public/assets/west-coast-hero.png`：首页封面图
- `wrangler.toml`：Cloudflare Pages 输出目录配置

## Cloudflare Pages 设置

连接本 GitHub 仓库后使用以下设置：

- Framework preset：`None`
- Build command：留空
- Build output directory：`public`

保存并部署后，Cloudflare Pages 会生成一个可分享的 `pages.dev` 链接。之后每次向 GitHub 推送更新，Cloudflare Pages 都会自动重新发布。

## 本地预览

在项目根目录运行：

```powershell
python -m http.server 4173 --directory public
```

然后打开 `http://127.0.0.1:4173/`。
