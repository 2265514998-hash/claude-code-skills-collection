---
name: onboard
description: Onboard to a new codebase quickly. When user says "onboard me", "explain this project", "how does this work", "understand this codebase", or opens a new project.
allowed-tools: [Bash, Read, Grep, Glob]
disable-model-invocation: false
---

# Onboard — 快速理解代码库

为新代码库生成全面的理解文档。

## 分析维度

### 1. 项目概览
- 读取 README.md、package.json / pyproject.toml / go.mod
- 识别项目类型（web 应用、CLI 工具、库、微服务等）
- 总结核心功能

### 2. 技术栈
- 语言和框架
- 数据库
- 关键依赖

### 3. 目录结构
- 解释主要目录的用途
- 标注关键入口文件

### 4. 架构分析
- 整体架构模式（MVC、微服务、事件驱动等）
- 数据流路径
- API 端点或主要接口

### 5. 核心抽象
- 最重要的类/模块/函数
- 关键的设计模式

### 6. 开发工作流
- 如何构建：从 package.json / Makefile 中查找
- 如何测试
- 如何运行
- 环境变量需求：检查 .env.example

### 7. 注意事项
- 已知的技术债务
- TODO/FIXME 标记
- 性能关键路径
- 安全敏感区域

## 输出格式
```markdown
# <项目名称> 代码库分析

## 📋 概览
## 🛠 技术栈
## 📂 目录结构
## 🏗 架构
## 🔑 核心抽象
## 🚀 开发工作流
## ⚠️ 注意事项
```
