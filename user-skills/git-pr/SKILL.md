---
name: git-pr
description: Create a pull request with proper title, description, and changelog. When user says "create PR", "open PR", "pull request", or wants to submit changes for review.
allowed-tools: [Bash(git *), Bash(gh *)]
disable-model-invocation: false
---

# Git PR — 创建 Pull Request

自动创建规范的 Pull Request。

## 步骤

1. 确保所有变更已提交：`git status`
2. 确认当前分支：`git branch --show-current`
3. 推送到远程：`git push -u origin <branch>`
4. 生成 PR 内容：
   - 获取分支与主分支的差异：`git log main..HEAD --oneline`
   - 分析变更文件：`git diff --name-only main...HEAD`
5. 创建 PR 标题：简洁描述变更内容
6. PR 描述模板：
   ```markdown
   ## 变更说明
   - 描述主要变更

   ## 变更类型
   - [ ] 新功能
   - [ ] Bug 修复
   - [ ] 重构
   - [ ] 文档

   ## 测试
   - 描述如何测试这些变更

   🤖 Generated with [Claude Code](https://claude.com/claude-code)
   ```
7. 使用 `gh pr create` 创建 PR
