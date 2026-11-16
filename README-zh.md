# 个人学术主页（基于 AcadHomepage 思路）

这是一个可部署到 GitHub Pages 的英文个人学术主页工程。它保留了 [RayeRen/AcadHomepage](https://github.com/RayeRen/acad-homepage.github.io) 的核心信息架构：个人侧栏、主页分区、GitHub Pages 部署与可选 Scholar 引用统计。已依据 Yulin Teng 提供的 CV 和研究定位填入核心内容；GitHub 用户名、个人头像及公开学术主页链接仍待补齐。

## 使用步骤

1. 在 GitHub 新建公开仓库，名称必须是 `YOUR_GITHUB_USERNAME.github.io`。
2. 将本目录全部文件推送至该仓库的 `main` 分支。
3. 依次替换 `_config.yml`、`_pages/about.md` 与 `images/avatar.svg` 中的占位内容；详细资料见 [CUSTOMIZE-ME.md](CUSTOMIZE-ME.md)。
4. 在仓库 **Settings → Pages → Build and deployment** 选择 **GitHub Actions**。推送后 Actions 会自动构建，网址为 `https://YOUR_GITHUB_USERNAME.github.io`。

## 本地预览（可选）

安装 Ruby 与 Bundler 后运行：

```powershell
bundle install
bundle exec jekyll serve
```

然后访问 `http://127.0.0.1:4000`。

## 引用统计（可选）

原模板通过 Google Scholar 爬虫与 GitHub Action 更新引用。由于该过程需要你的 Scholar ID、仓库密钥以及对爬虫合规/稳定性的自行确认，本起始工程默认未启用。仅添加个人 Scholar 链接不需要此功能。

## 致谢

信息架构参考 [AcadHomepage](https://github.com/RayeRen/acad-homepage.github.io)；视觉主题使用 [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes)。请在二次发布时遵循各上游项目的许可证。

