---
tags:
  - 建站
  - 写作
---

# 给个人博客选一个轻量的写作流程

> 这是一篇示例文章。替换成你的内容后，也可以删除本提示。

## 用 Markdown 写作

每篇文章保存为一个 `.md` 文件。这样内容容易迁移、版本管理，也不需要先搭建数据库或后台服务。

```text
docs/
├── blog/
│   ├── first-post.md
│   └── weekly.md
└── notes/
```

## 发布

本地预览确认后，将修改推送到 GitHub；配置好 Pages 后，GitHub Actions 可以自动构建并发布网站。
