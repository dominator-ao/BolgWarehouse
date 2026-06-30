---
title: Git 常用命令速查表
date: 2026-06-29 18:00:00
categories:
  - 技术
  - 工具
tags:
  - git
  - 版本控制
---

## 基础操作

```bash
git init                    # 初始化仓库
git clone <url>             # 克隆仓库
git add .                   # 添加所有文件
git commit -m "message"     # 提交
git push origin main        # 推送
git pull origin main        # 拉取
```

## 分支操作

```bash
git branch                  # 查看分支
git branch <name>           # 创建分支
git checkout <name>         # 切换分支
git checkout -b <name>      # 创建并切换分支
git merge <name>            # 合并分支
git branch -d <name>        # 删除分支
```

## 撤销操作

```bash
git reset HEAD <file>       # 撤销暂存
git checkout -- <file>      # 撤销修改
git revert <commit>         # 撤销提交
git stash                   # 暂存当前工作
git stash pop               # 恢复暂存
```

## 查看状态

```bash
git status                  # 查看状态
git log --oneline           # 简洁日志
git diff                    # 查看差异
git show <commit>           # 查看提交详情
```

## 实用技巧

```bash
# 修改最后一次提交
git commit --amend

# 查看某个文件的历史
git log --follow <file>

# 搜索代码
git grep "keyword"
```
