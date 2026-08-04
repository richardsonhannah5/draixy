乐富app【Q-——333307——】乐富app【 辋芷《888yx●vip》 】
乐富app【Q-——333307——】乐富app【 辋芷《888yx●vip》 】

 从零搭建个人博客：GitHub Pages + Hexo 完整教程（2025最新版）

还在羡慕别人拥有专属博客？其实你只需要一个GitHub账号，10分钟就能免费搭建一个高颜值、支持HTTPS的个人网站。本文将手把手教你完成部署，小白也能轻松上手。

 为什么选择GitHub Pages + Hexo？
- 零成本：完全免费，无需购买服务器和域名
- 高度可定制：上千款Hexo主题任选，轻松打造个性化网站
- SEO友好：生成纯静态页面，加载速度快，利于百度收录
- 版本管理：基于Git生态，文章修改记录清晰可溯

 三步快速部署你的博客

 第一步：环境准备
需要安装Node.js（建议LTS版本）、Git工具，并注册GitHub账号。在终端输入 `node -v` 和 `git --version` 验证环境是否配置成功。

 第二步：本地构建站点
打开终端，执行以下命令创建博客框架：
```bash
npm install -g hexo-cli
hexo init my-blog
cd my-blog
npm install
hexo server
```
浏览器访问 `http://localhost:4000`，看到默认页面即表示成功。

 第三步：部署到GitHub
1. 新建一个名为 `你的用户名.github.io` 的仓库
2. 修改根目录 `_config.yml` 中的部署配置：
```yaml
deploy:
  type: git
  repo: https://github.com/你的用户名/你的用户名.github.io.git
  branch: main
```
3. 执行部署命令，等待2-5分钟即可通过公网访问：
```bash
hexo clean && hexo generate && hexo deploy
```

 高级优化：让博客更好用
- 绑定专属域名：在仓库Settings的Pages选项中填写自定义域名，并添加CNAME解析
- 安装百度统计：在主题配置中嵌入统计代码，掌握访客数据
- 提交站点收录：前往百度站长平台提交sitemap.xml，加速内容被搜索引擎抓取

 常见问题排查
- 页面无法访问：请检查仓库名称是否与用户名完全一致
- 样式丢失：在 `_config.yml` 中确认 `url` 和 `root` 路径设置正确
- 部署报错：重新安装 hexo-deployer-git 插件即可解决

现在你会搭建自己的博客了吗？如果遇到问题，欢迎在评论区留言，我会逐一解答。已经搭建成功的朋友，不妨分享你的博客链接，让大家一起学习交流。下期将讲解如何用GitHub Actions实现自动发布文章，敬请期待！

相关推荐：

https://github.com/martinezjessica6229/eyvqwl/blob/main/2026%E6%9D%83%E5%A8%81%E7%94%84%E9%80%89%EF%BC%9A%E4%B9%90%E5%AF%8C%E5%BC%80%E6%88%B7%E5%AE%98%E7%BD%91_%E9%82%93%E6%B9%9B%E9%A2%87%E6%BB%A5%E9%B2%81UHUVO.md

<img src="https://i.postimg.cc/1XjxMj0W/lefu-00015.png" />

相关推荐：

https://github.com/martinezjessica6229/eyvqwl/commit/9225b7de693829b8a090419b920b578d046fa6c7

<img src="https://i.postimg.cc/9McjfTF9/lefu-00009.png" />
相关推荐：

https://github.com/sheppardrandall419/okbjfs/blob/main/2026%E7%A7%91%E6%8A%80%E7%94%84%E9%80%89%EF%BC%9A%E4%B9%90%E5%AF%8C%E5%BC%80%E6%88%B7%E6%B3%A8%E5%86%8C_%E6%B8%8D%E6%AD%89%E9%93%B0%E7%B2%97%E7%9B%8ENUAVN.md

<img src="https://i.postimg.cc/wT1Y39gp/lefu-00019.png" />
相关推荐：

https://github.com/sheppardrandall419/okbjfs/commit/6940e0b2e1b1e87c7ca6fe603cc4317a3b84c6d9

<img src="https://i.postimg.cc/9McjfTF9/lefu-00009.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
