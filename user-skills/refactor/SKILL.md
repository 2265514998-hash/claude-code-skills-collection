---
name: refactor
description: Systematic code refactoring with safety checks. When user says "refactor", "clean up", "restructure", "improve code quality", or wants to reorganize code.
allowed-tools: [Bash, Read, Grep, Glob, Edit, Write]
disable-model-invocation: false
---

# Refactor — 安全重构

系统化代码重构，确保行为不变。

## 重构原则

1. **行为保持不变** — 重构前后外部行为完全一致
2. **小步快跑** — 每次只做一个原子化变更
3. **测试保护** — 每次变更后运行测试
4. **可回退** — 使用 git 确保可以随时回退

## 重构检查清单

### 开始前
- [ ] 确认代码有测试覆盖
- [ ] `git stash` 保存未提交的变更
- [ ] 理解当前代码的功能

### 重构中
- [ ] 提取重复代码 (DRY)
- [ ] 改善命名 (清晰的变量/函数名)
- [ ] 简化条件逻辑
- [ ] 拆分过大的函数/类
- [ ] 移除死代码
- [ ] 改善错误处理
- [ ] 添加类型注解/类型安全

### 完成后
- [ ] 运行完整测试套件
- [ ] 检查是否有新的 lint 警告
- [ ] 确认 git diff 符合预期
- [ ] 如有性能关键路径，运行基准测试

## 常见重构模式

| 模式 | 场景 |
|------|------|
| Extract Function | 函数过长 |
| Inline Variable | 变量只使用一次 |
| Replace Conditional with Polymorphism | 复杂 if/switch |
| Introduce Parameter Object | 参数过多 |
| Replace Magic Number with Constant | 硬编码数值 |
