---
title: Hexo 博客搭建指南
date: 2026-06-30 12:00:00
categories:
  - 技术
  - 博客
tags:
  - hexo
  - github-pages
  - fluid
---

## 为什么选择 Hexo

Hexo 是一个快速、简洁且高效的博客框架，基于 Node.js 构建。

### 优势

1. **速度快** - 几秒钟内即可生成数百个文件
2. **支持 Markdown** - 写作体验极佳
3. **一键部署** - 支持 GitHub Pages、Vercel 等
4. **丰富的主题** - 社区活跃，主题美观

## 安装

```bash
npm install -g hexo-cli
hexo init blog
cd blog
npm install
```

## 常用命令

```bash
hexo new "文章标题"     # 新建文章
hexo generate           # 生成静态文件
hexo server             # 本地预览
hexo deploy             # 部署
```

## 总结

Hexo + Fluid 主题是一个非常棒的博客组合，推荐给大家使用。
