# runtask

> 紫微智控一键启动任务命令

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 🚀 快速开始

### 安装

```bash
# 一键安装
sudo bash /home/admin/Ziwei/scripts/install-runtask.sh
```

### 使用

```bash
# 交互式模式
runtask

# 命令行模式
runtask TASK-20250227-001 "计算器项目" "Python 命令行计算器"
```

---

## 📋 功能特性

- ✅ **全局命令**: 任何目录都能使用
- ✅ **所有用户**: root 或其他用户都能执行
- ✅ **自动定位**: 自动切换到 Ziwei 目录
- ✅ **交互式**: 逐步提示输入
- ✅ **容错机制**: 失败不阻塞流程
- ✅ **双平台同步**: GitHub + Gitee 自动同步

---

## 🎯 使用方法

### 交互式输入（推荐）

```bash
runtask
```

**屏幕提示**:
```
[1/3] 请输入任务 ID:
  任务 ID: TASK-20250227-001

[2/3] 请输入任务名称:
  任务名称：Python 计算器

[3/3] 请输入任务描述:
  任务描述：创建一个命令行计算器
```

### 命令行参数（快速）

```bash
runtask TASK-20250227-001 "Python 计算器" "创建一个计算器"
```

---

## 📦 安装

### 自动安装（推荐）

```bash
sudo bash /home/admin/Ziwei/scripts/install-runtask.sh
```

### 手动安装

```bash
# 创建符号链接
sudo ln -sf /home/admin/Ziwei/scripts/run-task.sh /usr/local/bin/runtask
sudo chmod +x /usr/local/bin/runtask

# 配置权限
sudo chmod -R 755 /home/admin/Ziwei/scripts/
sudo chmod -R 777 /home/admin/Ziwei/data/
```

---

## 🗑️ 卸载

```bash
sudo bash /home/admin/Ziwei/scripts/uninstall-runtask.sh
```

---

## 📚 文档

- [使用指南](https://github.com/ziwei-control/ziwei-archive)
- [交互式说明](https://github.com/ziwei-control/ziwei-archive)
- [容错机制](https://github.com/ziwei-control/ziwei-archive)

---

## 🔧 配置

### 环境变量

编辑 `/home/admin/Ziwei/.env`:

```bash
# GitHub 配置
GITHUB_TOKEN="your_github_token"
GITHUB_REPO="git@github.com:ziwei-control/ziwei-archive.git"

# Gitee 配置
GITEE_TOKEN="your_gitee_token"
GITEE_REPO_SSH="git@gitee.com:pandac0/ziwei-archive.git"
```

---

## 🎯 使用场景

### 场景 1: 创建计算器项目

```bash
runtask TASK-20250227-001 "Python 计算器" "创建一个命令行计算器"
```

### 场景 2: 创建电商网站

```bash
runtask TASK-20250228-002 "React 电商网站" "完整的电商网站前端"
```

### 场景 3: 创建数据分析脚本

```bash
runtask TASK-20250301-001 "销售数据分析" "Python 数据分析脚本"
```

---

## 📊 完整流程

```
runtask
  ↓
[1/6] 创建项目（GitHub + Gitee）
  ↓
[2/6] 等待仓库准备
  ↓
[3/6] 克隆项目到本地
  ↓
[4/6] 创建任务文件
  ↓
[5/6] 提交并推送到双平台
  ↓
[6/6] 启动紫微智控处理流程
  ↓
T-01 → T-02 → T-03 → 交付 → 归档
```

---

## 🔍 故障排查

### 命令不存在

```bash
which runtask
# 如果为空，重新安装
sudo bash /home/admin/Ziwei/scripts/install-runtask.sh
```

### 权限错误

```bash
sudo chmod +x /usr/local/bin/runtask
sudo chmod -R 755 /home/admin/Ziwei/scripts/
sudo chmod -R 777 /home/admin/Ziwei/data/
```

---

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

---

## 📝 许可证

MIT License

---

## 🔗 链接

- [紫微智控主仓库](https://github.com/ziwei-control/ziwei-archive)
- [Gitee 镜像](https://gitee.com/pandac0/ziwei-archive)

---

**一个命令 `runtask`， anywhere, anytime!** 🚀
