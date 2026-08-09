百达登录【Q-——333307——】百达登录【 辋芷《888yx●vip》 】
百达登录【Q-——333307——】百达登录【 辋芷《888yx●vip》 】

 从零部署个人博客：GitHub Pages + Hexo 完整教程

你是不是也收藏过一堆“搭建博客”的文章，结果要么步骤过时，要么报错没人管？今天这篇，我踩完所有坑，给你一条能直接跑通的路线。全程无需服务器，域名免费，还能绑定自己的域名。

 为什么选 Hexo + GitHub Pages？

- 零成本：托管在 GitHub 静态服务器上，一年省下几百块服务器钱。
- 速度快：纯静态页面，国内访问通过 CDN 加速也不慢。
- 易维护：写 Markdown 就行，发布只需一条命令。

当然，如果你想要更现代的方案，也可以试试 VitePress 或 Astro，但今天我们先聊最经典的组合。

 第一步：准备环境（5 分钟）

1. 安装 Node.js：去官网下载 LTS 版本，一路下一步。
2. 安装 Git：Windows 用户记得勾选“添加到 PATH”。
3. 注册 GitHub 账号：这个应该不用教了吧。

 第二步：本地搭建 Hexo（3 分钟）

```bash
npm install hexo-cli -g   全局安装
hexo init my-blog         初始化项目
cd my-blog
npm install               安装依赖
hexo s                    本地预览
```

浏览器打开 `http://localhost:4000`，看到默认页面就说明成功了。

 第三步：部署到 GitHub Pages（重点）

1. 创建仓库：命名为 `用户名.github.io`（必须是这个名字）。
2. 修改配置：打开 `_config.yml`，把 `deploy` 部分改成：

```yaml
deploy:
  type: git
  repo: https://github.com/你的用户名/你的用户名.github.io.git
  branch: main
```

3. 一键部署：

```bash
npm install hexo-deployer-git --save
hexo clean && hexo g && hexo d
```

等 1-2 分钟，访问 `https://用户名.github.io`，你的博客就上线了。

 进阶技巧：让博客更好看、更好搜

- 换主题：去 [Hexo Themes](https://hexo.io/themes/) 挑一个，比如 `NexT` 或 `Fluid`，在主题仓库 README 里按说明安装。
- SEO 优化：安装 `hexo-generator-seo-friendly-sitemap`，同时每个文章标题一定要有核心关键词，我每篇文章都会刻意布局 3-5 个精准词，比如本文的“GitHub Pages 教程”“Hexo 部署”。
- 绑定域名：在仓库 Settings → Pages 里填上你的域名，再解析 CNAME 即可。

 遇到报错怎么办？

- 部署失败：试试 `hexo clean` 清缓存。
- 页面 404：等 5 分钟，或者检查分支是否是 `main` 而非 `master`。
- 图片不显示：把图片存到 `source/images/`，用绝对路径引用。

---

最后留个互动：你目前卡在哪一步？或者你已经部署成功了，欢迎在评论区晒出你的博客地址，我会去参观并帮你提出优化建议。觉得有用的话，点个 Star 支持一下，我会持续更新更深入的教程。

相关推荐：

https://github.com/leeandrea41/grnvxj/blob/main/2026%E7%AC%AC%E4%B8%80%E7%9B%98%E7%82%B9%EF%BC%9A%E7%99%BE%E8%BE%BE%E4%B8%BB%E7%AE%A1%E7%BD%91%E5%9D%80_%E9%9F%A7%E5%89%96%E7%BA%B6%E6%80%A5%E8%82%9AMZAHB.md

<img src="https://i.postimg.cc/g2g50LWJ/mei-nu-bei-jing-zhao-shang-tu-zhi-zuo-(89).png" />

相关推荐：

https://github.com/leeandrea41/grnvxj/commit/be4afcfbd6bf5ae8e6f640df2c085d2c011732a9

<img src="https://i.postimg.cc/ncZwYGVR/mei-nu-bei-jing-zhao-shang-tu-zhi-zuo-(94).png" />
相关推荐：

https://github.com/rodriguezmelinda044/ycqxlg/blob/main/2026%E7%A7%91%E6%8A%80%E7%94%84%E9%80%89%EF%BC%9A%E7%99%BE%E8%BE%BE%E4%B8%BB%E7%AE%A1%E7%99%BB%E5%BD%95_%E6%8D%A3%E8%93%96%E9%A2%87%E9%A9%B6%E8%BF%94NOOPC.md

<img src="https://i.postimg.cc/VvPZhjqz/mei-nu-bei-jing-zhao-shang-tu-zhi-zuo-(90).png" />
相关推荐：

https://github.com/rodriguezmelinda044/ycqxlg/commit/1e8afdf91e135a7d2d8a34caf83b1de8f89adafc

<img src="https://i.postimg.cc/ncZwYGVR/mei-nu-bei-jing-zhao-shang-tu-zhi-zuo-(94).png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
