# ⚡ skill-generator

**把重复的工作，变成一句话的事。**

每次让 AI 帮你做完一件事，下次还想再做一遍？手动复制粘贴 prompt 太累？**skill-generator** 能把你的工作流自动打包成可复用的 Skill，下次直接调用。

---

## 🎯 一句话体验

> 告诉 AI：`生成技能 写周报` → 得到一个专属的周报 Skill → 以后说「写周报」直接出结果

## ✨ 核心能力

| 能力 | 说明 |
|------|------|
| 🏃 **直接执行** | 说需求，立刻干活，不废话 |
| 📋 **先计划** | 先给你看步骤，你点头再执行 |
| 📦 **生成技能** | 把工作流固化成 Skill，下次一键复用 |
| 🧠 **自动学习** | 检测重复任务，主动问你「要不要生成 Skill」 |
| 💬 **简化模式** | 说「简化模式」，AI 用大白话跟你聊 |

---

## 🚀 部署指南 / Deployment Guide

### 📌 前置要求 / Prerequisites

| 项目 | 要求 |
|------|------|
| OpenClaw | 已安装并正常运行 |
| 系统 | Windows / macOS / Linux |

---

### 🪟 Windows 部署 / Windows Deployment

**方法一：手动复制（推荐新手）**

1. 打开 PowerShell，创建目录：
   ```powershell
   mkdir "$env:USERPROFILE\.qclaw\workspace\skills\skill-generator" -Force
   ```

2. 下载 SKILL.md 文件到该目录

3. 重启 OpenClaw 使其加载新 Skill

**方法二：命令行安装**

```powershell
# 克隆仓库
git clone https://github.com/DYF996/skill-generator.git "$env:USERPROFILE\.qclaw\workspace\skills\skill-generator"

# 或者手动下载并解压到该目录
```

---

### 🍎 macOS / Linux 部署

**方法一：手动复制**

```bash
# 创建目录
mkdir -p ~/.qclaw/workspace/skills/skill-generator

# 下载文件
curl -O https://raw.githubusercontent.com/DYF996/skill-generator/main/SKILL.md
mv SKILL.md ~/.qclaw/workspace/skills/skill-generator/

# 或者克隆整个仓库
git clone https://github.com/DYF996/skill-generator.git ~/.qclaw/workspace/skills/skill-generator
```

**方法二：使用 Git**

```bash
git clone https://github.com/DYF996/skill-generator.git ~/.qclaw/workspace/skills/skill-generator
```

---

### ✅ 验证安装 / Verify Installation

安装完成后，说一句话测试一下：

```
生成技能 测试
```

如果 AI 回复了生成技能的流程，说明安装成功！

---

### 🔧 常见问题 / Troubleshooting

| 问题 | 解决方案 |
|------|----------|
| Skill 没有加载 | 重启 OpenClaw |
| 找不到目录 | 检查路径是否有拼写错误 |
| 权限不足 | 给目录设置读写权限 |
| 需要更新 | `git pull` 或重新下载最新版本 |

---

### 📁 推荐目录结构 / Recommended Structure

```
~/.qclaw/workspace/skills/skill-generator/
├── SKILL.md                    # ⭐ 必须文件
├── references/                 # 可选：参考文档
│   ├── skill_spec.md
│   └── interactive_protocol.md
└── README.md                   # 可选：本文件
```

---

## 📖 工作原理

```
你：生成技能 每周汇总销售数据

AI：
┌─────────────────────────────────────────┐
│  📦 正在为你生成「销售周报」Skill...      │
├─────────────────────────────────────────┤
│  ✓ 分析了工作流程                        │
│  ✓ 生成了 SKILL.md 文件                  │
│  ✓ 定义了触发词：销售周报 / 周报 / ...    │
└─────────────────────────────────────────┘

下次：> 销售周报
结果：自动生成一份漂亮的周报！
```

## 💡 适用场景

- 📊 **数据分析**：重复导出报表、生成图表
- 📝 **文档处理**：格式转换、内容整理
- 📧 **邮件处理**：自动生成、批量回复
- 🗂️ **文件管理**：分类整理、批量重命名
- 🔍 **研究调研**：多源搜索、内容汇总

## 🤝 贡献

欢迎提交 Issue 和 PR！如果你有好的想法或者发现了 bug，随时联系我们。

## 📄 License

MIT

---

**Star ⭐ 支持一下，让更多人看到这个项目**
