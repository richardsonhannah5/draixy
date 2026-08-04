乐富官方主管【Q-——333307——】乐富官方主管【 辋芷《888yx●vip》 】
乐富官方主管【Q-——333307——】乐富官方主管【 辋芷《888yx●vip》 】

 从零搭建个人博客：GitHub Pages + Hugo 完整指南

> 想拥有一个完全属于自己的技术博客？不花一分钱，不用买服务器，这篇教程带你 30 分钟上线。

 为什么要用 GitHub Pages 建博客

很多开发者每天刷 GitHub，却不知道它自带免费静态托管服务。相比市面上各种博客平台，GitHub Pages + Hugo 方案有四个不可替代的优势：

1. 完全免费：无需云服务器，无限流量
2. 版本管理：所有文章都是 Git 仓库文件，历史可追溯
3. 极致速度：纯静态页面，CDN 加速，国内访问流畅
4. 自定义域名：支持绑定自己的域名，SEO 友好

 第一步：环境准备（3分钟）

本地安装需要三样东西：

- Git：版本管理工具（官网下载安装）
- Hugo：静态站点生成器（macOS 用 `brew install hugo`，Windows 用 Chocolatey）
- 代码编辑器：VS Code 或任意文本编辑器

安装完成后，打开终端输入 `hugo version`，看到版本号即安装成功。

 第二步：创建博客项目（5分钟）

```bash
 创建新站点
hugo new site my-blog
cd my-blog

 初始化 Git 仓库
git init

 安装一个漂亮的主题（以 PaperMod 为例）
git submodule add https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod
```

在 `config.toml` 配置文件中添加主题名称：

```toml
theme = "PaperMod"
```

然后创建第一篇

```bash
hugo new posts/first-post.md
```

 第三步：写文章并本地预览（5分钟）

用编辑器打开刚才生成的 `.md` 文件，删掉默认内容，写上你的第一段文字。注意文章头部必须保留，这是 Hugo 识别文章的元数据：

```yaml
---
title: "我的第一篇文章"
date: 2024-01-01T10:00:00+08:00
draft: false
---
```

运行 `hugo server` 启动本地服务，浏览器访问 `http://localhost:1313` 即可实时预览效果。

 第四步：部署到 GitHub（10分钟）

1. 新建仓库：在 GitHub 创建仓库，命名为 `你的用户名.github.io`
2. 推送代码：

```bash
git add .
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/你的用户名/你的用户名.github.io.git
git push -u origin main
```

3. 开启 Pages 服务：进入仓库 Settings → Pages，Source 选择 `GitHub Actions`，Hugo 官方有自动部署工作流，GitHub 会自动识别并构建。

等待 2-3 分钟，访问 `https://你的用户名.github.io` 就能看到你的博客上线了。

 常见问题与技巧

Q：如何绑定自定义域名？
在仓库 Settings → Pages 中填写域名，然后在 DNS 服务商添加 CNAME 解析即可。

Q：每次写文章都要手动部署吗？
不需要。GitHub Actions 配置好之后，每次 `git push` 都会自动重新构建。

Q：文章分类和标签怎么弄？
在文章头部添加 `categories` 和 `tags` 字段即可，Hugo 会自动生成聚合页面。

进阶技巧：利用 GitHub Actions 的定时任务，可以自动拉取外部数据生成博客文章，实现真正的"数字花园"。

 写在最后

博客建好只是开始，持续输出才是核心。建议每篇技术文章都配上可运行的代码示例和效果 Demo，这样读者更容易产生互动。如果想看云原生、CI/CD 相关的进阶玩法，欢迎在评论区留言，我下期继续分享。

如果你在搭建过程中遇到问题，截图发在评论区，我看到会第一时间回复。

相关推荐：

https://github.com/sheppardrandall419/okbjfs/blob/main/%E8%BF%9B%E9%98%B6%E5%AE%9E%E6%93%8D%E6%8C%87%E5%8D%97%EF%BC%9A%E4%B9%90%E5%AF%8C%E4%B8%BB%E7%AE%A1%E5%A8%B1%E4%B9%90_%E4%B8%8B%E5%8D%A6%E9%80%9F%E6%B2%BF%E5%96%9CLFFSY.md

<img src="https://i.postimg.cc/XNH0VrMC/lefu-00016.png" />

相关推荐：

https://github.com/sheppardrandall419/okbjfs/commit/426347e4b75e70528b049a59836e339e43144ec9

<img src="https://i.postimg.cc/XJx6BJpR/lefu-00011.png" />
相关推荐：

https://github.com/martinezjessica6229/eyvqwl/blob/main/2026%E7%A7%91%E6%8A%80%E7%88%86%E7%82%B9%EF%BC%9A%E4%B9%90%E5%AF%8C%E4%B8%BB%E7%AE%A1%E5%AE%98%E6%96%B9_%E5%B1%A5%E8%B4%B8%E8%B7%83%E9%A2%90%E6%8D%B6JPRTH.md

<img src="https://i.postimg.cc/xTBDzB1n/lefu-00020.png" />
相关推荐：

https://github.com/martinezjessica6229/eyvqwl/commit/d8fe8cf51f4b4ee33e3089a9ee370c4e566aa69c

<img src="https://i.postimg.cc/50pWQ0XN/lefu-00012.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
