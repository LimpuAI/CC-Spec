# 更新日志

本项目的变更记录遵循 Keep a Changelog 格式，并尽量遵循语义化版本号。

## [Released]

## [1.0.0] - 2026-04-13

### Added
- **新增命令**: cc-docs (文档生成), cc-review (代码审查), cc-wave (批量任务)
- **新增 Agent**: rust-expert, typescript-expert, spec-code-reviewer
- **新增 Skill**: arch-design-expert, backend-expert

### Changed
- 从原项目 ClaudeCode-Kiro-Workflow 分支并演进，版本从 1.0.0 开始
- **目录迁移**: 将 `.claude/` 下的 agents 和 commands 迁移至 `.agents/` 目录
- **Agent 精简**: 从原有的 6 个专家精简为 3 个

---

> 以下版本为原项目 ClaudeCode-Kiro-Workflow 的历史版本记录

## [2.0.0] - 2025-01

- 革命性重构：在保持 100% 功能完整的前提下大幅精简文档与命令复杂度。
- 架构优化：目录结构更清晰，.specs 文档组织精简且可追踪。
- 开发标准：新增 Shell/服务/端口冲突等统一规范，保证一致性与可移植性。
- 安全机制：会话与 Git 分支保护、数据库自动备份、工作区状态检查等多重保障。
- 会话连续性：cc-save/cc-load 提升跨会话衔接体验。
- 收尾流程：cc-end 自动归档、更新变更日志并支持发布打标签。
- 智能分析：cc-analyze/cc-think 提供多维度分析能力与需求影响评估。

[Unreleased]: https://github.com/LimpuAI/CC-Spec/compare/v1.0.0...HEAD
[1.0.0]: https://github.com/LimpuAI/CC-Spec/releases/tag/v1.0.0
[2.0.0]: https://github.com/heihuzicity-tech/ClaudeCode-Kiro-Workflow/commit/9ea15a5
