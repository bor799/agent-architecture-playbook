# Agent Architecture Learning Skill

[English](#english-version) | [中文](#中文版本)

---

## 中文版本

### 简介

这是一个**教学型 AI Skill**，帮助产品架构师通过框架对比真正内化 Agent 架构决策逻辑。

> "不教写代码，教做决策"

### 背景

在学习 Agent 开发过程中，我发现**通过对比不同框架来学习**是最有效的方法。但市面上大多数教程都在教"怎么写代码"，而不是"怎么做架构决策"。

这个 Skill 专门为**产品架构师**设计，专注于：
- 判断产品需要什么级别的 Agent 能力
- 理解框架设计的核心权衡
- 识别 AI 给出的技术方案是否过度工程

### 功能特性

- **自动初始化**：分析文章/框架的定位
- **诊断对话**：快速定位知识盲区
- **引导学习**：用业务场景解释概念
- **记忆机制**：增量学习，持续追踪掌握状况
- **总结沉淀**：每次学习后生成记录
- **跨平台兼容**：同时支持 OpenAI 和 Claude

### 核心框架：四阶模型

```
第一阶：大脑（LLM） → 能思考，不能行动
第二阶：手脚（工具） → 能行动，做完就忘
第三阶：经验（记忆） → 能记住，能自主探索
第四阶：协作（控制） → 用户能实时干预
```

**核心判断**：你的产品需要演进到第几阶？

### 安装

```bash
# 复制 skill 文件到 skills 目录
cp agent-architecture-learning.md ~/.claude/skills/

# （可选）创建学习历史文件
cp agent-learning-history.md ~/.claude/knowledge/
```

### 使用

在对话中直接调用：

```
/skill agent-architecture-learning
```

或提供任何 Agent 框架相关的文章/文档链接。

### 交付物

```
agent-architecture-learning-skill/
├── README.md                          # 本文件
├── agent-architecture-learning.md     # 主 skill 文件
└── docs/
    ├── learning-history-template.md   # 学习记录模板
    ├── framework-comparison.md        # 框架对比参考
    └── scenario-library.md            # 业务场景库
```

### 技术栈

- AI 平台：OpenAI (ChatGPT) + Anthropic (Claude)
- 格式：YAML front matter + Markdown
- 存储：本地文件系统

### 作者

**Murphy** (@bor799)

- 产品架构师，追求极致效率
- GitHub: https://github.com/bor799

### License

MIT

---

## English Version

### Introduction

A **teaching-oriented AI Skill** that helps product architects truly internalize Agent architecture decision logic through framework comparison.

> "Don't teach coding, teach decision-making"

### Background

While learning Agent development, I discovered that **learning by comparing different frameworks** is the most effective method. However, most tutorials focus on "how to write code" rather than "how to make architecture decisions."

This Skill is designed specifically for **product architects**, focusing on:
- Determining what level of Agent capability a product needs
- Understanding core trade-offs in framework design
- Identifying whether AI-generated technical solutions are over-engineered

### Features

- **Auto-initialization**: Analyze article/framework positioning
- **Diagnostic dialogue**: Quickly identify knowledge gaps
- **Guided learning**: Explain concepts using business scenarios
- **Memory mechanism**: Incremental learning with continuous progress tracking
- **Summary & retention**: Generate records after each session
- **Cross-platform compatibility**: Support for both OpenAI and Claude

### Core Framework: Four-Stage Model

```
Stage 1: Brain (LLM) → Can think, cannot act
Stage 2: Hands (Tools) → Can act, forgets after completion
Stage 3: Experience (Memory) → Can remember, can explore autonomously
Stage 4: Collaboration (Control) → User can intervene in real-time
```

**Core Question**: What stage does your product need to evolve to?

### Installation

```bash
# Copy skill file to skills directory
cp agent-architecture-learning.md ~/.claude/skills/

# (Optional) Create learning history file
cp agent-learning-history.md ~/.claude/knowledge/
```

### Usage

Invoke directly in conversation:

```
/skill agent-architecture-learning
```

Or provide any Agent framework-related article/documentation link.

### Deliverables

```
agent-architecture-learning-skill/
├── README.md                          # This file
├── agent-architecture-learning.md     # Main skill file
└── docs/
    ├── learning-history-template.md   # Learning record template
    ├── framework-comparison.md        # Framework comparison guide
    └── scenario-library.md            # Business scenario library
```

### Tech Stack

- AI Platforms: OpenAI (ChatGPT) + Anthropic (Claude)
- Format: YAML front matter + Markdown
- Storage: Local file system

### Author

**Murphy** (@bor799)

- Product Architect, pursuing extreme efficiency
- GitHub: https://github.com/bor799

### License

MIT
