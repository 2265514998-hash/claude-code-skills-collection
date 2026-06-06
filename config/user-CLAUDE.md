# 用户级 CLAUDE.md — 全局配置

## 语言和沟通

- 始终使用中文回复
- 代码注释使用中文
- 技术术语保持英文原样

## 工作方式

- 修改代码前先完整阅读相关文件
- 每次修改后运行相关测试
- 使用 `/commit` (git-commit skill) 生成规范的提交信息
- 优先利用已有的 skills 来处理常见任务
- 遇到不确定的情况主动询问而非猜测

## 代码质量

- 保持与项目现有代码风格一致
- 不要引入不必要的抽象层
- 错误处理必须完善
- 避免在代码中硬编码配置值

## 技能使用

- 使用 `/debug` (debug skill) 进行系统化调试
- 使用 `/refactor` (refactor skill) 进行安全重构
- 使用 `/onboard` (onboard skill) 理解新项目
- 使用 `/git-commit` (git-commit skill) 生成规范提交
- 使用 `/git-pr` (git-pr skill) 创建 PR
- 使用 `/session-summary` 生成会话总结
