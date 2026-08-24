# Agent 架构决策手册

> **Don't teach framework syntax. Practice architecture decisions.**

大多数 Agent 教程从「怎么写代码」开始。这个项目从另一个问题开始：**面对一个真实产品，究竟需要多少 Agent 能力，什么时候继续演进反而是过度工程？**

## 四阶模型

```text
1. 大脑：LLM
   能理解和生成，但不能行动

2. 手脚：Tools
   能调用外部能力，但做完容易失去状态

3. 经验：Memory / State
   能保留上下文，形成持续工作过程

4. 协作：Control / Human-in-the-loop
   人能观察、干预、纠错和承担最终责任
```

真正的问题不是「哪个框架最好」，而是：

> **你的业务场景需要演进到哪一阶？新增复杂度解决了什么具体失败？**

## Skill 怎样工作

- 先识别产品目标与当前约束；
- 对比不同 Agent 框架的设计取舍；
- 用业务场景解释 Tool、Memory、Planning 与 Control；
- 识别 AI 生成方案里的过度工程；
- 把每次学习沉淀成可继续调用的判断记录。

## 内容

```text
agent-architecture-learning.md   Skill 入口
docs/framework-comparison.md     框架比较
docs/scenario-library.md         场景库
docs/learning-history-template.md 学习记录模板
```

## 使用

将 `agent-architecture-learning.md` 复制到支持 Markdown Skill 的 Agent 环境，再提供一个具体产品或架构材料进行对比学习。

## My role

我负责把「学习 Agent 技术」重新定义为「训练产品架构判断」，并设计四阶模型、场景驱动的对话流程与停止条件。这个项目也是我从纯技术学习走向产品架构思维的早期记录。
