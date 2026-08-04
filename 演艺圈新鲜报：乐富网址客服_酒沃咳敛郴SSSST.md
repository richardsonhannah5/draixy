乐富网址客服【Q-——333307——】乐富网址客服【 辋芷《888yx●vip》 】
乐富网址客服【Q-——333307——】乐富网址客服【 辋芷《888yx●vip》 】

 从零搭建个人博客：我用GitHub Pages + Hexo，3小时上线并完成SEO优化

最近不少朋友问我：“想搭一个自己的技术博客，但买服务器、配数据库太麻烦，有没有更轻量的方案？”

我的答案是：GitHub Pages + Hexo。它免费、速度快、支持自定义域名，最关键的是——对搜索引擎非常友好，收录效率高。

这篇文章，我会分享从零搭建的完整步骤，并附上我自己的 SEO 优化经验，帮你少踩坑。

 一、为什么推荐 GitHub Pages？

1. 免费且稳定：无需服务器，直接绑定 GitHub 仓库。
2. 加载速度快：CDN 加速，国内访问体验不错。
3. Markdown 原生支持：写作专注内容，不用管排版。

 二、Hexo 初始化三步走

```bash
 1. 安装 Hexo 脚手架
npm install hexo-cli -g

 2. 初始化博客目录
hexo init my-blog && cd my-blog

 3. 安装部署插件并关联仓库
npm install hexo-deployer-git --save
```

修改站点配置 `_config.yml`：

```yaml
deploy:
  type: git
  repo: https://github.com/你的用户名/你的仓库.git
  branch: main
```

执行 `hexo clean && hexo g && hexo d`，大功告成。

 三、百度收录优化的 3 个关键动作

很多朋友搭建完博客发现百度不收录，问题往往出在主动推送和结构化上。

 1. 提交站点地图（Sitemap）

安装插件：

```bash
npm install hexo-generator-sitemap --save
```

然后在 `_config.yml` 中添加：

```yaml
sitemap:
  path: sitemap.xml
```

去百度搜索资源平台提交你的站点和 sitemap 地址。

 2. 主动推送链接（百度站长后台）

生成推送脚本：

```bash
npm install hexo-baidu-url-submit --save
```

配置推送 token，每次 `hexo d` 后自动向百度提交新链接，收录速度提升 90%。

 3. 优化 TDK 关键词布局

在文章头部 Front-matter 里，明确写好标题、描述、关键词：

```yaml
title: 从零搭建个人博客
description: 使用GitHub Pages和Hexo搭建个人博客，附带百度SEO收录优化教程
keywords: GitHub Pages, Hexo, 博客搭建, 百度收录, SEO优化
```

注意：关键词密度控制在 2%-3%，自然融入正文，不要堆砌。

 四、我的实战数据分享

优化一周后，我的博客：
- 百度收录从 0 → 47 篇
- 日均 UV 从 20 → 150+
- 核心关键词“Hexo 教程”排名进入百度前三页

如果你也想搭建一个能快速收录、搜索可见的个人博客，现在就可以动手试试。

你在搭建过程中遇到的最大坑是什么？欢迎评论区留言，我每条都会回复。 如果文章对你有帮助，点个关注，后续更新更快的 SEO 技巧。

相关推荐：


<img src="https://i.postimg.cc/wT1Y39gp/lefu-00019.png" />

相关推荐：


<img src="https://i.postimg.cc/9McjfTF9/lefu-00009.png" />
相关推荐：


<img src="https://i.postimg.cc/wT1Y39gp/lefu-00019.png" />
相关推荐：


<img src="https://i.postimg.cc/xTBDzB1n/lefu-00020.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
