---
name: session-summary
description: Generate a structured summary of the current coding session. When user says "summarize", "session summary", "what did we do", "wrap up", or at end of a long session.
allowed-tools: [Read]
disable-model-invocation: false
---

# Session Summary — 会话总结

生成结构化的会话总结，便于下次继续工作。

## 输出格式

```markdown
# 会话总结 — <日期>

## ✅ 完成的工作
- [x] 具体完成的任务 1
- [x] 具体完成的任务 2

## 🔄 进行中的工作
- [ ] 未完成的任务 1 (进度: 50%)
- [ ] 未完成的任务 2

## 📝 关键决策
1. 决策 1 — 原因
2. 决策 2 — 原因

## 📁 修改的文件
- `path/to/file1.ts` — 修改说明
- `path/to/file2.py` — 修改说明

## 🐛 已知问题
- 问题 1 — 状态/影响

## 🔜 下一步
1. 优先级高的下一步
2. 次要任务

## 💡 备注
- 重要的上下文信息
- 下次继续的提示
```

## 指南
- 从会话上下文中提取所有关键信息
- 标注未完成的 TODO 和 FIXME
- 记录重要的架构决策和原因
- 列出下次会话应该优先处理的事项
