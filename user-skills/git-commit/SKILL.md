---
name: git-commit
description: Generate conventional commit messages and commit changes. When user says "commit", "commit changes", "generate commit message", or wants to commit code.
allowed-tools: [Bash(git *)]
disable-model-invocation: false
---

# Git Commit — 智能提交

分析当前 staged 和 unstaged 的变更，生成符合 [Conventional Commits](https://www.conventionalcommits.org/) 规范的提交信息。

## 步骤

1. 运行 `git status` 和 `git diff --staged` 查看当前变更
2. 如果没有 staged 的文件，运行 `git diff` 和 `git diff --name-only` 查看所有变更
3. 分析变更内容，确定 type：
   - `feat`: 新功能
   - `fix`: Bug 修复
   - `refactor`: 代码重构
   - `perf`: 性能优化
   - `style`: 代码格式
   - `docs`: 文档更新
   - `test`: 测试相关
   - `chore`: 构建/工具/依赖
   - `ci`: CI/CD 变更
4. 生成 commit message 格式：`<type>(<scope>): <description>`
5. 展示给用户确认，确认后执行 `git add` 和 `git commit`
6. 提交信息末尾自动添加 `Co-Authored-By: Claude Opus 4.8 <noreply@anthropic.com>`
