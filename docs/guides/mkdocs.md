# MkDocs guides

For full documentation visit [mkdocs.org](https://www.mkdocs.org).

## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.

## Deployment to GitHub Pages
- 问题: 2026/05/04 推送dev分支并且 workflow 成功后, 但访问 https://wenbozou.github.io/wb-learn-notes/ 失败
- 尝试解决的步骤:
  - 1. Build and deployment 从 "Deploy from a branch" 切换到 "GitHub Actions
  - 2. 检查 Deploy 日志信息，发现存在警告异常信息，发送给 Copilot 分析并重新生成了ci.yml文件
  - 3. 重新提交代码，触发 workflow，成功部署到 GitHub Pages