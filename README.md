# 🤖 ai-human-sdd — Reasonix Skill

> 人机协作 SDD 模式 — AI 执行结构 + 用户视角自审，一次性交付完整产品业务闭环。
>
> AI executes structure + user reviews, delivering a complete product business loop in one shot.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

---

## 简介 | Introduction

**ai-human-sdd** 是 [Reasonix](https://github.com/reasonix/reasonix) 的一款技能（skill），定义了一种**人机协作的 SDD（Spec-Driven Development）工作法**，用于完整产品的全流程交付。

核心理念：**AI 负责结构和执行，人负责决策和把关。**

工作流程分为两大阶段：

```
阶段一：设计（Design）
  Constitution → Spec → Plan（含 UI 规范选择）→ 你确认方案

阶段二：实现（Implement）
  按业务层逐层自动化实现 → 测试 → 自审优化 → 交付
```

> 你只需要决策四次：定方向 → 审方案 → 确认自审结果 → 验收交付。
> 中间的编码执行由 AI 全权完成，无需在阶段间做确认。

---

## 安装 | Installation

### 前提 | Prerequisites

- [Reasonix](https://reasonix.dev) 已安装并可用

### 安装技能 | Install the Skill

```bash
# 方式一：从 GitHub 直接安装
reasonix skill install https://raw.githubusercontent.com/<你的GitHub用户名>/skill-ai-human-sdd/main/SKILL.md

# 方式二：克隆仓库后本地安装
git clone https://github.com/<你的GitHub用户名>/skill-ai-human-sdd.git
reasonix skill install ./skill-ai-human-sdd/SKILL.md
```

### 验证 | Verify

```bash
reasonix skill list | grep ai-human-sdd
```

---

## 使用方法 | Usage

在 Reasonix 对话中触发该技能：

| 触发词 | Trigger Phrases |
|--------|----------------|
| "SDD"、"完整产品"、"业务闭环"、"项目启动" | English: "SDD", "full product", "business loop", "new project" |
| "人机协作"、"全量实现"、"solo"、"自审优化" | "one-shot delivery", "human-AI collaboration", "solo mode" |

### 典型工作流 | Typical Workflow

1. **定方向** — AI 给出项目方向选项，你来选
2. **Constitution** — 起草项目核心原则，你审阅
3. **Spec** — 按业务层编写完整功能规格，含验收条件
4. **Plan** — 输出完整技术方案（结构/数据/API/UI规范）
5. **实现管道** — AI 逐层自动化实现，每层经过测试→质量门→UI校验
6. **用户视角自审** — AI 模拟用户走通所有流程，修复问题
7. **交付** — 生成完整交付包（代码+文档+测试报告）

---

## 设计哲学 | Design Philosophy

| 原则 | 说明 |
|------|------|
| 不跳过决策闸门 | 设计阶段每步确认后再推进，避免返工 |
| 一次性设计，Solo 连续性执行 | 设计充分讨论，实现 AI 全权负责 |
| 完整性先行 | 业务逻辑必须闭环，不允许"此功能暂未实现"的断点 |
| 质量门自动拦截 | 测试/构建/代码质量/UI规范在管道内自动检查 |
| 可追溯 | Spec 和 Plan 确认后保存，实现变更记录到 changelog |

---

## 依赖的关联技能 | Dependent Skills

该项目在生产环境中通常与以下 Reasonix 技能配合使用：

| 技能 | 用途 |
|------|------|
| `code-quality` | 编码质量全流程指南 |
| `phase-delegator` | 业务层拆解与 Sub-Agent 并行执行 |
| `design-taste-frontend` | 反 AI 模板化前端设计 |
| `minimalist-ui` | 极简编辑风 UI 规范 |
| `high-end-visual-design` | 高级视觉设计规范 |
| `frontend-design-gddw` | 前端设计 token 系统 |

> **注意**：这些为可选依赖。`ai-human-sdd` 核心工作流不依赖它们，但在前端项目中选择 UI 规范时会用到。

---

## 许可证 | License

[MIT](LICENSE) © 2025 xiaojie

---

## 贡献 | Contributing

欢迎提交 Issue 和 PR！请确保：

1. 保持与现有工作流的一致性
2. 更新相关文档
3. 说明改动对设计/实现阶段的影响
