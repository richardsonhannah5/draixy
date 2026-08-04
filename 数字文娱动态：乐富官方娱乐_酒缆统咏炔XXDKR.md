乐富官方娱乐【Q-——333307——】乐富官方娱乐【 辋芷《888yx●vip》 】
乐富官方娱乐【Q-——333307——】乐富官方娱乐【 辋芷《888yx●vip》 】

 从零搭建个人博客：GitHub Pages + Hexo 完整教程（2025最新版）

你是不是也想过拥有一个属于自己的博客？不用买服务器、不用备案、甚至不用花一分钱——GitHub Pages + Hexo 组合，就是目前最流行的免费静态博客解决方案。今天这篇文章，手把手带你从零搭建，全程可视化操作，小白也能轻松上手。

 为什么选择 GitHub Pages + Hexo？

先说说这个组合的优势，看完你就知道为什么大家都推荐它：

- 完全免费：托管在 GitHub 服务器上，无任何费用
- 加载速度快：静态页面，CDN 加速，国内访问也流畅
- 支持自定义域名：可以绑定自己的域名，更显专业
- 写作体验好：支持 Markdown 语法，专注于内容创作
- 版本管理便捷：所有文章都有 Git 历史记录，不怕丢失

 环境准备：你需要安装这些工具

在开始之前，请确保你的电脑已经安装了以下软件：

1. Git：版本控制工具，去 git-scm.com 下载安装即可
2. Node.js：运行环境，建议安装 LTS 版本（长期支持版）
3. 代码编辑器：推荐 VS Code，免费又好用

> 小提示：安装 Node.js 时，记得勾选 "Add to PATH" 选项，否则后续命令行会找不到命令。

 三步搭建你的专属博客

 第一步：创建 GitHub 仓库

登录你的 GitHub 账号，点击右上角 "+" 号，选择 "New repository"。仓库名格式必须是：用户名.github.io（例如：zhangsan.github.io），这样就能直接通过这个地址访问你的博客了。

 第二步：安装 Hexo 并初始化项目

打开终端（Mac 用户用 Terminal，Windows 用户用 PowerShell），依次输入以下命令：

```bash
 全局安装 hexo
npm install -g hexo-cli

 初始化博客项目
hexo init my-blog
cd my-blog

 安装依赖
npm install

 本地预览
hexo server
```

看到终端输出 "Hexo is running at http://localhost:4000" 后，在浏览器访问这个地址，你就能看到默认的博客页面了。

 第三步：部署到 GitHub Pages

在 _config.yml 配置文件中修改部署信息：

```yaml
deploy:
  type: git
  repo: https://github.com/你的用户名/你的用户名.github.io.git
  branch: main
```

然后执行：

```bash
npm install hexo-deployer-git --save
hexo clean
hexo generate
hexo deploy
```

稍等片刻，访问 "你的用户名.github.io"，你的博客就正式上线啦！

 个性化设置：让博客更出彩

 更换主题

Hexo 有丰富的主题市场，推荐几个热门主题：
- Next：经典简洁，功能强大
- Butterfly：颜值高，动画效果好  
- Fluid：清新文艺，适合技术博客

 写文章的命令

```bash
hexo new post "我的第一篇文章"
```

这条命令会在 source/_posts 目录下生成一个 Markdown 文件，用编辑器打开即可开始写作。

 常见问题解决

Q：部署时报错 "Authorization failed"？
A：需要配置 GitHub 的 Personal Access Token，或者改用 SSH 方式连接。

Q：图片显示不出来？
A：在 _config.yml 中设置 `post_asset_folder: true`，并在站点配置中加入 `marked` 插件的 `prependRoot` 选项。

 让更多人看到你的博客

搭建好博客只是第一步，想要获得更多流量，还需要做好 SEO：

1. 添加 SEO 插件：安装 hexo-generator-seo-friendly-sitemap，自动生成 sitemap
2. 优化文章3. 内链建设：在文章中合理添加其他文章的链接
4. 提交搜索引擎：将站点提交到 Google Search Console 和百度站长平台

 部署到国内服务器？试试一键迁移

如果你担心 GitHub 在国内的访问速度，可以考虑使用 Gitee Pages（码云）或者 Vercel 部署，方法类似，只需修改部署仓库地址即可。

---

如果你在搭建过程中遇到任何问题，欢迎在评论区留言，我看到后会及时回复。 觉得这篇文章对你有帮助的话，点个赞支持一下吧！关注我，后续会分享更多博客优化技巧和写作干货。

现在就去动手创建你的第一个博客吧！有任何疑问随时交流，期待看到你的作品上线 🚀

相关推荐：

https://github.com/jarvisdanielle312/mphvpi/blob/main/2026%E6%9D%83%E5%A8%81%E7%9B%98%E7%82%B9%EF%BC%9A%E4%B9%90%E5%AF%8C%E5%A8%B1%E4%B9%90%E6%B3%A8%E5%86%8C_%E5%97%9C%E9%86%8B%E5%A7%91%E6%98%BE%E5%A9%AAGGGNT.md

<img src="https://i.postimg.cc/TwTXPmYs/lefu-00010.png" />

相关推荐：

https://github.com/jarvisdanielle312/mphvpi/commit/83fd066489b93d56078beae9be0f444490232052

<img src="https://i.postimg.cc/wT1Y39gp/lefu-00019.png" />
相关推荐：

https://github.com/rhodesandrea462/zjvmux/blob/main/2026%E5%AE%98%E6%96%B9%E7%88%86%E7%82%B9%EF%BC%9A%E4%B9%90%E5%AF%8C%E5%A8%B1%E4%B9%90%E7%BD%91%E5%9D%80_%E7%9A%87%E5%BB%96%E8%A3%99%E6%B1%B2%E8%AF%9CBIUCQ.md

<img src="https://i.postimg.cc/1XjxMj0W/lefu-00015.png" />
相关推荐：

https://github.com/rhodesandrea462/zjvmux/commit/eb93aab2b8019ed9bcd9df1b44d45f7630e40fc5

<img src="https://i.postimg.cc/50pWQ0XN/lefu-00012.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
