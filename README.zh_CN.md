# 用于快速创建分支社区网站的模板项目

## 用法

1. 复刻（Fork）此仓库
2. 在得到的复刻仓库中，点击“Settings”
3. 在设置页面中点击左侧栏的“Pages”
4. 在"Build and deployment"区域的“Source”下拉选项中选择“GitHub Actions”
5. 推送任意变动到此仓库之中

然后，你的网站稍后就会自动完成部署了。

你可以通过点击在你的复刻仓库主页右侧的“Environments”之下的“github-pages”链接来查看部署状态，也可以使用此时页面中展示的“View deployment”按钮来访问部署所得到的站点。

您可以任意对此仓库进行修改，网站的内容会在您的修改推送成功后自动进行更新。

## 在本地预览效果

此站点模板基于 [HUGO](https://gohugo.io/) 静态网站生成工具。你可以从系统的包管理工具，或是通过官方网站等途径获取并安装 HUGO。你从 HUGO 官方网站等途径了解到的任何 HUGO 知识也可以被直接应用到此模板站点之上。

> **note**
> deepin **v20** 仓库中所附带的 `hugo` 版本略有过时。如果你在使用 deepin v20，请考虑从 [GitHub](https://github.com/gohugoio/hugo/releases/) 获取 HUGO 的可执行文件来使用 HUGO，或者从类如 [`Nix`](https://nixos.org/) 的其它包管理平台来安装 HUGO。

这里提供一个简要的步骤来帮助你快速上手：

0. 首先确保你已经 `cd` 到了仓库的根目录下（指包含着 config.toml 与 README.md 的目录下）
1. 确保 HUGO 已经安装好了：`hugo version`
2. 启动一个本地服务器：`hugo server`（默认可从 `http://localhost:1313/` 访问）
3. 创建一个新的博客帖子：`hugo new post/your-post-title.md`（新文件会创建到 `content/post/your-post-title.md`，请注意，新的帖子会默认是草稿 `draft` 状态）
4. 启动一个可以访问草稿帖子的本地服务器：`hugo server -D`
5. 快速浏览所有可用命令：`hugo -h`

## 主题

此仓库中包含了一个名为 [up-business-theme](https://themes.gohugo.io/themes/up-business-theme/) 的主题，此仓库所附带的此主题的版本为 `5144bddd81373502200e43ba8fb7f62f33e2e075`。为了使使用此仓库的过程变得尽可能简单，我们没有以 git 子模块的形式附带主题仓库。
