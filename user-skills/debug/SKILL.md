---
name: debug
description: Systematic debugging workflow. When user says "debug", "fix bug", "why is this broken", "troubleshoot", or reports an error/issue.
allowed-tools: [Bash, Read, Grep, Glob, Edit]
disable-model-invocation: false
---

# Debug — 系统化调试流程

遵循 5-WHY 方法论进行系统化调试。

## 调试流程

### 1. 复现 (Reproduce)
- 理解问题描述，确认触发条件
- 读取相关错误日志和堆栈跟踪
- 如果能复现，记录复现步骤

### 2. 隔离 (Isolate)
- 使用二分法缩小范围（注释代码、git bisect）
- 检查最近的变更：`git log --oneline -10`
- 查找相关的配置文件和环境变量
- 检查依赖版本变更

### 3. 根因分析 (Root Cause)
- 使用 5-WHY 方法追溯根本原因
- 不要只修复表面症状
- 检查是否有类似的潜在问题

### 4. 修复 (Fix)
- 编写最小化的修复代码
- 确保修复不引入新问题
- 添加必要的错误处理

### 5. 验证 (Verify)
- 验证修复是否解决了问题
- 运行相关测试：`npm test` / `pytest` / `go test`
- 检查是否有其他受影响的区域

## 输出格式
```
## 🔍 调试报告

**问题**: <简述>
**根因**: <根本原因>
**修复**: <修复方案>
**影响的文件**: <文件列表>
**验证**: <验证结果>
```
