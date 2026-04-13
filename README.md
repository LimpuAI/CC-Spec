# CC-Spec - Claude Code 开发工作流系统

<div align="center">

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Claude Code](https://img.shields.io/badge/Claude%20Code-Optimized-purple.svg)

**Fork from [ClaudeCode-Kiro-Workflow](https://github.com/heihuzicity-tech/ClaudeCode-Kiro-Workflow) - 更简洁、更高效、更强大的开发工作流**

[简体中文](./README.md)

</div>

## 🎯 项目简介

CC-Spec 是基于 [ClaudeCode-Kiro-Workflow](https://github.com/heihuzicity-tech/ClaudeCode-Kiro-Workflow) 分支演进而来的 Claude Code 开发工作流系统。在保留原项目核心功能的同时，针对实际使用场景进行了优化精简。

## ✨与原项目的差异

### ✨ 新增命令（CC-Spec 独有）

| 命令 | 功能 | 说明 |
|------|------|------|
| **cc-docs** | 文档生成 | 自动生成项目文档和 API 文档 |
| **cc-review** | 代码审查 | 多维度代码质量审查 |
| **cc-wave** | 批量任务 | 批量执行多个任务 |

### 命令增强

- cc-start 和 cc-end 增加对需求实现过程中项目级的前瞻性探讨记录，遗留专项TODO，以及部分争议问题。
- cc-end 中增加了对 `project-info.md` 的维护

### 新增SKILLS

| SKILL | 功能 | 说明 |
|------|------|------|
| **arch-design-expert** | 架构设计增强，强化设计原则 | cc-start、cc-docs、cc-review 的公共依赖 |
| **backend-expert** | 后端专家的公共技能，强化实操细节 | rust-expert、typescript-expert 的公共依赖 |

### Agents变化

移除原有的所有子Agents(描述过于宽泛没有实操性)，新增如下Agent

| Agent | 功能 | 说明 |
|------|------|------|
| **rust-expert** | rust开发专家 | 基于 backend-expert 基础上增加rust特性细化要求 |
| **typescript-expert** | typescript开发专家 | 基于 backend-expert 基础上增加typescript特性细化要求 |
| **spec-code-reviewer** | 需求实现审查专家 | 核对需求与实现的差异，并检查原则遵循和潜在问题，cc-sync 更侧重在完成度的检查 |

## 🗂️ 所有命令列表

```
.agents/
├── commands/              # 命令集
│   ├── cc-start           # 启动新功能开发
│   ├── cc-next            # 执行下一个任务
│   ├── cc-task            # 查看当前进度
│   ├── cc-save            # 保存工作状态
│   ├── cc-load            # 恢复工作会话
│   ├── cc-sync            # 同步文档与代码
│   ├── cc-analyze         # 智能代码分析
│   ├── cc-think           # 深度需求分析
│   ├── cc-fix             # 快速 Bug 修复
│   ├── cc-end             # 完成功能开发
│   ├── cc-info            # 项目信息管理
│   ├── cc-git             # Git 操作集成
│   ├── cc-docs            # 文档生成（新增）
│   ├── cc-review          # 代码审查（新增）
│   └── cc-wave            # 批量任务（新增）
├── agents/                # 专家 Agent
│   ├── rust-expert
│   ├── typescript-expert
│   └── spec-code-reviewer
└── skills/                # 公共技能
    ├── arch-design-expert
    └── backend-expert
```

## 🚀 快速开始

### 安装

```bash
# 克隆 CC-Spec 仓库
git clone https://github.com/LimpuAI/CC-Spec.git
cd CC-Spec

# 复制到你的项目
cp -r .agents /path/to/your-project/
```

### 基本使用

```bash
# 初始化项目信息
/cc-info

# 开始新功能开发
/cc-start 用户认证功能

# 查看当前任务
/cc-task

# 执行下一批次任务，推荐使用 cc-wave 而不是 cc-next，以充分发挥多Agent并行协作提速
/cc-wave

# 保存进度
/cc-save

# 恢复会话
/cc-load

# 完成功能
/cc-end
```

## 🎯 适用场景

### ✅ 最适合
- 新功能开发（从 0 到 1）
- 复杂需求梳理
- 团队协作项目
- 代码重构任务

### ⚠️ 可选使用
- 简单 Bug 修复（可用 cc-fix 快速处理）
- 实验性原型开发
- 紧急热修复

## 🤝 贡献指南

欢迎贡献代码和建议！

1. Fork 本仓库
2. 创建功能分支
3. 提交更改
4. 发起 Pull Request

### 贡献方向
- 命令优化建议
- 新功能命令
- 文档改进
- Bug 修复

## 📄 许可证

MIT License - 详见 [LICENSE](LICENSE) 文件

## 🔗 相关链接

- [GitHub 仓库](https://github.com/LimpuAI/CC-Spec)
- [原项目: ClaudeCode-Kiro-Workflow](https://github.com/heihuzicity-tech/ClaudeCode-Kiro-Workflow)
- [问题反馈](https://github.com/LimpuAI/CC-Spec/issues)
- [Claude Code 官方文档](https://docs.anthropic.com/en/docs/claude-code)
- [更新日志](./CHANGELOG.md)

---

**版本**: 1.0.0
**发布日期**: 2026年4月
**维护状态**: 活跃开发中
