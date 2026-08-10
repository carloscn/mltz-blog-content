# mltz-blog-content

我博客 [mltz.tech](https://mltz.tech) 的内容仓库。

- `posts/` — 文章,Markdown/TOML front matter 格式,与 Hugo 的 `content/posts/` 一致
- `static/` — 图片等多媒体资源,会被同步到 Hugo 的 `static/` 目录

## 写新文章

新建 `posts/任意文件名.md`,格式参考已有文章即可,例如:

\`\`\`
+++
date = '2026-08-10T15:00:00+08:00'
draft = false
title = '文章标题'
tags = ['标签1', '标签2']
+++

正文内容(Markdown)。
\`\`\`

## 插入图片

把图片放进 `static/images/`,文章里用 `![描述](/images/xxx.png)` 引用。

## 发布

push 到 main 分支,GitHub Actions 会自动同步到服务器并重新构建站点,几秒到几十秒内生效。
