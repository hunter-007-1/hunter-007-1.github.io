# Iron Blog

> 记录学习，热爱技术，向着全栈和 AI Agent 方向努力。

个人技术博客，基于 [Hexo](https://hexo.io/) 构建，使用 [Butterfly](https://butterfly.js.org/) 主题，部署于 [GitHub Pages](https://hunter-007-1.github.io/)。

## 技术栈

- **框架**: [Hexo](https://hexo.io/) 8.x
- **主题**: [hexo-theme-butterfly](https://github.com/jerryc127/hexo-theme-butterfly) 5.5.5
- **部署**: GitHub Pages（通过 hexo-deployer-git）
- **搜索**: 本地搜索（hexo-generator-searchdb）

## 主要功能

- 暗色模式（跟随系统自动切换）
- PJAX 无刷新页面切换
- 本地文章搜索
- 文章字数统计与预计阅读时间
- APlayer 音乐播放器
- Live2D 看板娘
- 粒子连线背景 + 点击烟花效果
- 不蒜子 PV/UV 统计
- Share.js 社交分享
- 代码块 Mac 风格高亮

## 本地开发

### 环境要求

- [Node.js](https://nodejs.org/) >= 18
- [Git](https://git-scm.com/)

### 安装依赖

```bash
npm install
```

### 启动本地服务器

```bash
npm run server
```

访问 `http://localhost:4000` 预览博客。

### 生成静态文件

```bash
npm run build
```

### 自动部署到 GitHub Pages

向 `main` 分支提交文章或配置后，GitHub Actions 会自动构建并发布网站，无需在本地运行部署命令。

### 手动部署（备用）

```bash
npm run deploy
```

## 目录结构

```
my-blog/
├── source/             # 博客源文件（Markdown 文章、页面）
│   ├── _posts/         # 文章
│   ├── about/          # 关于页面
│   ├── categories/     # 分类页面
│   ├── tags/           # 标签页面
│   └── link/           # 友链页面
├── scaffolds/          # 文章模板
├── themes/             # 主题文件
├── public/             # 生成的静态文件（Git 忽略）
├── .deploy_git/        # 部署缓存（Git 忽略）
├── _config.yml         # Hexo 主配置
├── _config.butterfly.yml  # Butterfly 主题配置
└── package.json
```

## 写作

新建文章：

```bash
npx hexo new "文章标题"
```

在 `source/_posts/` 下编辑生成的 `.md` 文件即可。

## 许可

[CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)
