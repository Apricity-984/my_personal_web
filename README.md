# 个人博客

基于 Material for MkDocs 的中文个人网站。文章以 Markdown 保存，构建结果是可托管的静态网站。

## 本地预览

```powershell
py -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
mkdocs serve
```

打开终端显示的本地地址即可预览。保存 Markdown 文件后，页面会自动刷新。

## 发布到 GitHub Pages

1. 将本目录推送到 GitHub 仓库的 `main` 分支。
2. 在仓库设置中启用 GitHub Pages，并选择 `gh-pages` 分支作为发布来源。
3. 后续推送到 `main` 时，`.github/workflows/deploy.yml` 会自动构建并发布。

## 开始定制

- 在 `mkdocs.yml` 修改站点名称、描述、作者和导航目录。
- 在 `docs/index.md` 替换首页介绍。
- 在 `docs/about.md` 填写个人简介和联系方式。
- 在 `docs/blog/` 和 `docs/notes/` 新建 Markdown 文章，并将页面加入 `mkdocs.yml` 的 `nav`。
- 将 `requirements.txt` 中的版本范围收紧为你实际使用的版本，以便复现构建环境。
