# 🚀 Claude Code Supercharged

> 全网精选 Claude Code Skills、Commands、配置一站式合集

[![Skills](https://img.shields.io/badge/Skills-178-blue)](./user-skills/)
[![Commands](https://img.shields.io/badge/Commands-12-green)](./user-commands/)
[![Config](https://img.shields.io/badge/Config-Ready-orange)](./config/)

---

## 📂 目录结构

```
.
├── README.md                    # 本文件
├── CLAUDE.md                    # 项目级 Claude Code 配置
├── .gitignore
├── config/
│   ├── user-CLAUDE.md           # 全局用户级 CLAUDE.md
│   └── settings.template.json   # settings.json 模板（已脱敏）
├── user-skills/                 # 178 个精选 Skills
│   ├── git-commit/              # 智能提交
│   ├── git-pr/                  # 自动创建 PR
│   ├── debug/                   # 系统化调试
│   ├── refactor/                # 安全重构
│   ├── onboard/                 # 新项目快速理解
│   ├── session-summary/         # 会话总结
│   ├── spellbook-*/             # 45 个 claude-spellbook 技能
│   ├── ecc-*/                   # 6 个 everything-claude-code 技能
│   └── tpl-*/                   # 120+ 模板（前后端/DevOps/AI/ML）
├── user-commands/               # 12 个 Slash Commands
│   ├── code-review.md
│   ├── feature-dev.md
│   ├── checkpoint.md
│   └── ...
└── repos/                       # 原始仓库（被 .gitignore 忽略）
```

---

## 🔥 精选自以下顶级仓库

| 仓库 | Stars | 贡献 |
|------|-------|------|
| [artubss/SKILLS-CLAUDE-CODE](https://github.com/artubss/SKILLS-CLAUDE-CODE) | — | 120+ 精选模板 |
| [kid-sid/claude-spellbook](https://github.com/kid-sid/claude-spellbook) | — | 45 个专业技术 skills |
| [affaan-m/everything-claude-code](https://github.com/affaan-m/everything-claude-code) | 32k+ | 6 个技能 + 5 个 agent |
| [danielrosehill/Claude-Slash-Commands](https://github.com/danielrosehill/Claude-Slash-Commands) | — | 3 个实用 commands |
| [hesreallyhim/awesome-claude-code](https://github.com/hesreallyhim/awesome-claude-code) | 43k+ | 索引参考 |

---

## ⚡ 快速安装

### 1. 克隆本仓库

```bash
git clone https://github.com/2265514998-hash/PlotPilot.git
cd PlotPilot
```

### 2. 安装到 Claude Code

```bash
# 安装 skills（复制到用户目录）
cp -r user-skills/* ~/.claude/skills/

# 安装 commands
cp user-commands/* ~/.claude/commands/

# 配置 CLAUDE.md（全局）
cp config/user-CLAUDE.md ~/.claude/CLAUDE.md

# 配置 settings.json（先编辑填入你的 API Key）
cp config/settings.template.json ~/.claude/settings.json
```

### 3. 编辑 `~/.claude/settings.json`

填入你的 API Key 和 Base URL。

---

## 🎯 最实用的 6 个自定义 Skills

| Skill | 用法 | 功能 |
|-------|------|------|
| `git-commit` | `/git-commit` 或说 "提交代码" | 智能 Conventional Commits |
| `git-pr` | `/git-pr` 或说 "创建 PR" | 自动生成 PR 描述 |
| `debug` | `/debug` 或说 "调试这个 bug" | 5-WHY 系统化调试 |
| `refactor` | `/refactor` 或说 "重构" | 安全检查清单式重构 |
| `onboard` | `/onboard` 或说 "介绍项目" | 7 维度代码库分析 |
| `session-summary` | `/session-summary` 或说 "总结" | 结构化会话总结 |

---

## 🛠 技能分类

### 前端
React · Vue 3 · Angular · Next.js · Nuxt 3 · Svelte · Remix · Astro · Electron · React Native · Tailwind

### 后端
FastAPI · Django · Express · NestJS · Go Chi · Rust Axum · Elixir Phoenix · GraphQL · Hono · Serverless

### 数据库
PostgreSQL · Redis · MongoDB · Elasticsearch · Prisma · Drizzle · SQLAlchemy

### DevOps
Docker · Kubernetes · Terraform · GitHub Actions · Ansible · Cloud Run · CI/CD

### AI / ML
RAG Pipeline · LangChain · HuggingFace · Vector Search · LLM Ops · YOLO · Airflow · ML Training · OpenAI API

### 架构
System Design · Microservices · Event-Driven · WebSockets · Caching · API Design · Feature Flags · Multi-Tenancy

### 安全 & 质量
Security Audit · Performance · Unit Testing · Integration Testing · Observability · Incident Response

---

## 📝 数据来源

- [artubss/SKILLS-CLAUDE-CODE](https://github.com/artubss/SKILLS-CLAUDE-CODE) — 833+ skills 巨型合集
- [kid-sid/claude-spellbook](https://github.com/kid-sid/claude-spellbook) — 64 skills + 18 commands
- [affaan-m/everything-claude-code](https://github.com/affaan-m/everything-claude-code) — 黑客松冠军全配置
- [danielrosehill/Claude-Slash-Commands](https://github.com/danielrosehill/Claude-Slash-Commands) — 350+ 分类 commands
- [hesreallyhim/awesome-claude-code](https://github.com/hesreallyhim/awesome-claude-code) — 最权威社区索引
- [alexknowshtml/claude-skills](https://github.com/alexknowshtml/claude-skills) — 生产级 skill 集合

---

🤖 Generated with [Claude Code](https://claude.com/claude-code)
