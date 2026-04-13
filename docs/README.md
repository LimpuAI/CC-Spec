# CC-Spec - Claude Code Development Workflow System

<div align="center">

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Claude Code](https://img.shields.io/badge/Claude%20Code-Optimized-purple.svg)

**Fork from [ClaudeCode-Kiro-Workflow](https://github.com/heihuzicity-tech/ClaudeCode-Kiro-Workflow) - Simpler, More Efficient, More Powerful**

[简体中文](../README.md)

</div>

## 🎯 Project Overview

CC-Spec is a Claude Code development workflow system forked and evolved from [ClaudeCode-Kiro-Workflow](https://github.com/heihuzicity-tech/ClaudeCode-Kiro-Workflow). While preserving the core functionality of the original project, it has been optimized and streamlined for real-world usage scenarios.

### 📊 Core Features

| Feature | Description |
|---------|-------------|
| **Documentation Reduction** | 48.4% fewer lines compared to original |
| **Command Optimization** | 64.2% reduction in average command length |
| **12 Commands** | Complete development workflow: start, execute, save, restore, analyze, fix, wrap-up |
| **Development Standards** | Unified Shell/service/port specifications |
| **Security Mechanisms** | Database backup, Git branch protection, workspace checks |
| **Session Continuity** | cc-save/cc-load for seamless cross-session connection |

## ✨ New Commands (CC-Spec Exclusive)

| Command | Feature | Description |
|---------|---------|-------------|
| **cc-docs** | 📚 Doc Generation | Auto-generate project and API documentation |
| **cc-review** | 🔍 Code Review | Multi-dimensional code quality review |
| **cc-wave** | 🌊 Batch Tasks | Execute multiple tasks in batch |

## 🗂️ Command List

```
.agents/
├── commands/              # Command set
│   ├── cc-start.md        # 🚀 Start new feature development
│   ├── cc-next.md         # ⚡ Execute next task
│   ├── cc-task.md         # 📊 View current progress
│   ├── cc-save.md         # 💾 Save work state
│   ├── cc-load.md         # 🔄 Restore work session
│   ├── cc-sync.md         # 📝 Sync docs and code
│   ├── cc-analyze.md      # 🔍 Smart code analysis
│   ├── cc-think.md        # 🧠 Deep requirement analysis
│   ├── cc-fix.md          # 🐞 Quick bug fix
│   ├── cc-end.md          # 🏁 Complete feature development
│   ├── cc-info.md         # ℹ️ Project info management
│   ├── cc-git.md          # 🔗 Git operations
│   ├── cc-docs.md         # 📚 Doc generation (New)
│   ├── cc-review.md       # 🔍 Code review (New)
│   └── cc-wave.md         # 🌊 Batch tasks (New)
└── agents/                # Expert Agents
    ├── rust-expert.md
    ├── typescript-expert.md
    └── spec-code-reviewer.md
```

## 🚀 Quick Start

### Installation

```bash
# Clone CC-Spec repository
git clone https://github.com/LimpuAI/CC-Spec.git
cd CC-Spec

# Copy to your project
cp -r .agents /path/to/your-project/
```

### Basic Usage

```bash
# Initialize project info
/cc-info

# Start new feature development
/cc-start user authentication

# Check current task
/cc-task

# Execute next task
/cc-next

# Save progress
/cc-save

# Restore session
/cc-load

# Complete feature
/cc-end
```

## 🆚 Differences from Original Project

CC-Spec has been optimized from [ClaudeCode-Kiro-Workflow](https://github.com/heihuzicity-tech/ClaudeCode-Kiro-Workflow) in the following ways:

1. **Documentation Reduction**: 48.4% fewer lines for better readability
2. **Command Optimization**: 64.2% shorter average command length, lower token consumption
3. **Naming**: kiro-* → cc-* for cleaner naming
4. **Development Standards**: Added Shell/service/port specifications for consistency
5. **Security Enhancement**: Database backup, Git branch protection, workspace checks
6. **Session Continuity**: Improved cc-save/cc-load context recovery

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create feature branch
3. Commit changes
4. Submit Pull Request

## 📄 License

MIT License - See [LICENSE](../LICENSE) file for details

## 🔗 Links

- [GitHub Repository](https://github.com/LimpuAI/CC-Spec)
- [Original Project: ClaudeCode-Kiro-Workflow](https://github.com/heihuzicity-tech/ClaudeCode-Kiro-Workflow)
- [Issue Tracker](https://github.com/LimpuAI/CC-Spec/issues)
- [Claude Code Documentation](https://docs.anthropic.com/en/docs/claude-code)
- [Changelog](../CHANGELOG.md)

---

**Version**: 1.0.0
**Release Date**: April 2026
**Status**: Actively Maintained