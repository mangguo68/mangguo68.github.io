# 个人博客

基于 Hexo + Vivia 主题构建的个人技术博客，记录前端开发、后端技术、全栈开发等相关知识和实战经验。

## 技术栈

- **框架**：Hexo 6.3.0
- **主题**：Vivia
- **前端**：Vue3, React, TypeScript, TailwindCSS
- **后端**：Express, Node.js
- **其他**：Java, Kotlin, Python, Android, Flutter

## 项目结构

```
my-test-blog/
├── source/            # 源码目录
│   ├── _posts/        # 文章目录
│   ├── about/         # 关于页面
│   └── images/        # 图片资源
├── scaffolds/         # 模板文件
├── themes/            # 主题目录
├── _config.yml        # Hexo 配置
├── _config.vivia.yml  # 主题配置
├── package.json       # 项目依赖
└── README.md          # 项目说明
```

## 快速开始

### 1. 安装依赖

```bash
# 安装项目依赖
npm install
```

### 2. 本地开发

```bash
# 启动本地服务器
npm run start

# 或使用 Hexo 命令
hexo server
```

访问 `http://localhost:4000` 查看本地博客。

### 3. 构建与部署

```bash
# 生成静态文件
npm run build

# 部署到 GitHub Pages
npm run deploy

# 一键构建并部署
npm run deploy:all
```

## 文章管理

### 创建新文章

```bash
# 创建新文章
hexo new "文章标题"

# 或使用模板
hexo new post "文章标题"
```

新文章会生成在 `source/_posts/` 目录下，使用 Markdown 格式编写。

### 文章格式

```markdown
---
title: 文章标题
date: 2025-12-01
categories:
  - 分类1
  - 分类2
tags:
  - 标签1
  - 标签2
---

# 文章内容

...
```

## 配置说明

### 站点配置

编辑 `_config.yml` 文件，修改站点信息：

```yaml
# Site
title: 个人博客
subtitle: ''
description: ''
author: mangguo
language: zh-CN

# URL
url: https://mangguo68.github.io

# Deployment
deploy:
  type: git
  repo: https://github.com/mangguo68/mangguo68.github.io.git
  branch: main
```

### 主题配置

编辑 `_config.vivia.yml` 文件，修改主题相关配置：

```yaml
# Header
menu:
  主页: /
  文档: /archives
  关于: /about

# Banner
banner:
  enable: true
  url: /images/1.jpg
  position: center
  onAllPages: true

# Personal info
avatar: /images/avatar.jpg
author: mangguo
subtitle: 一名全栈视角的前端实战派开发者
```

## 部署说明

### 部署到 GitHub Pages

1. **创建仓库**：在 GitHub 上创建 `username.github.io` 仓库
2. **配置部署**：修改 `_config.yml` 中的部署信息
3. **安装部署插件**：
   ```bash
   npm install hexo-deployer-git --save
   ```
4. **执行部署**：
   ```bash
   hexo generate
   hexo deploy
   ```

### 首次部署注意事项

- 首次部署后，GitHub Pages 可能需要 5-10 分钟时间生效
- 如果遇到 404 错误，请耐心等待后刷新页面
- 后续更新文章时，只需执行 `hexo deploy` 即可

## 项目特点

- **模块化设计**：清晰的目录结构，便于维护
- **丰富的主题**：使用 Vivia 主题，支持响应式设计
- **完整的分类**：按技术栈和主题分类，便于内容管理
- **多语言支持**：支持中文内容和国际化
- **性能优化**：静态站点生成，加载速度快

## 相关项目

- **电商平台**：小兔鲜购物平台（前端）
- **Android 应用**：漫画 App（原生开发）
- **全栈项目**：仿小红书（前后端一体化）
- **Nuxt3 项目**：仿简书（基于 Nuxt3 框架）

## 联系信息

- **GitHub**：[mangguo68](https://github.com/mangguo68)
- **博客地址**：[https://mangguo68.github.io](https://mangguo68.github.io)

## License

MIT
