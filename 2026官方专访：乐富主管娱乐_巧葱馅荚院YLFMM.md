乐富主管娱乐【Q-——333307——】乐富主管娱乐【 辋芷《888yx●vip》 】
乐富主管娱乐【Q-——333307——】乐富主管娱乐【 辋芷《888yx●vip》 】

 用 GitHub 托管个人博客，这套自动化部署方案绝了！

你是不是也遇到过这样的烦恼：想搭建个人博客，服务器费钱、备案麻烦、维护还心累？其实，GitHub Pages 就是一个完全免费、且能实现自动化部署的绝佳方案。今天这篇文章，手把手教你如何用 GitHub + Hugo 搭建一套属于自己的免费博客系统。

 为什么建议你选择 GitHub Pages？

首先是 零成本。你不需要购买任何云服务器，代码托管和网页访问都由 GitHub 免费提供。其次是 极客感。用 `git push` 来发文章，才是程序员该有的仪式感。最重要的是，这种方式对 搜索引擎（SEO）非常友好，加载速度快，静态页面天然容易被百度、谷歌收录。

 方案核心：一个仓库，两套分支

我们采用最经典的部署策略。你的博客源码（Hugo 源文件）保存在 `master` 分支，而生成的静态网页文件，会被推送到 `gh-pages` 分支。GitHub Pages 会直接拉取 `gh-pages` 分支的内容作为站点展示。

 手把手部署教程（极简版）

第一步：本地环境准备
安装 Hugo 和 Git 工具。在本地新建站点：`hugo new site my-blog`。

第二步：代码推送与自动化
在仓库的 `Settings -> Pages` 中，将 Source 设置为 `gh-pages` 分支。接下来，只需要提前编写好 GitHub Actions 配置文件（YAML），就能实现 “本地写好文章，push 后自动发版” 的丝滑体验。

```yaml
name: Deploy
on: [push]
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - uses: peaceiris/actions-hugo@v2
      - run: hugo --minify
      - uses: peaceiris/actions-gh-pages@v3
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          publish_dir: ./public
```

第三步：绑定自定义域名
购买一个喜欢的域名，在仓库根目录放一个 `CNAME` 文件，并在域名服务商配置解析记录即可。绑定后，记得去 百度搜索资源平台 提交站点，这样可以加快搜索引擎对你新网站的抓取速度。

 互动一下

这套 `DevOps` 流程看似简单，但能在“免费、高效、自动化”三个维度做到极致。如果你在配置 `Actions` 工作流时遇到报错，或者有其他关于 SEO收录 的小技巧，欢迎在下方评论区留言交流。这里是你的专属技术补给站，点赞收藏，下次部署不迷路！

相关推荐：

https://github.com/martinezkelly827/fwhecg/blob/main/%E5%85%A8%E8%A7%A3%E8%90%BD%E5%9C%B0%E6%95%99%E7%A8%8B%EF%BC%9A%E4%B9%90%E5%AF%8C%E7%BD%91%E5%9D%80%E5%AE%98%E6%96%B9_%E5%88%A0%E5%92%90%E6%88%BF%E5%B9%BD%E9%A1%BFTTGHO.md

<img src="https://i.postimg.cc/wT1Y39gp/lefu-00019.png" />

相关推荐：

https://github.com/martinezkelly827/fwhecg/commit/1f634896db3c3b6d27e853f6d4327770d61f6416

<img src="https://i.postimg.cc/sf6RVMFw/lefu-00017.png" />
相关推荐：

https://github.com/vazquezdarin376/rowkxj/blob/main/2026%E5%AE%98%E6%96%B9%E4%B8%93%E8%AE%BF%EF%BC%9A%E4%B9%90%E5%AF%8C%E7%BD%91%E5%9D%80%E6%B5%8B%E9%80%9F_%E5%92%B3%E6%B3%BB%E5%B8%98%E5%B1%85%E7%97%B9PQSAC.md

<img src="https://i.postimg.cc/xTBDzB1n/lefu-00020.png" />
相关推荐：

https://github.com/vazquezdarin376/rowkxj/commit/f5c3d7b69f39c0e797cbecbef478ef1cbede5748

<img src="https://i.postimg.cc/XqJSfb5x/lefu-00014.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
