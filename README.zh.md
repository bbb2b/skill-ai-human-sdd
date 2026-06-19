# 🤖 ai-human-sdd — SDD 人机协作工作法

> 人机协作 SDD 模式 — AI 执行结构 + 用户视角自审，一次性交付完整产品业务闭环。

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

---

## 简介

**ai-human-sdd** 是一种**人机协作的 SDD（Spec-Driven Development）工作法**，用于完整产品的全流程交付。可配合各种 AI 编程助手（Reasonix、Cursor、GitHub Copilot、Claude Code 等）使用。

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

## 如何使用

### 方式一：作为 Prompt 模板直接使用

将 [SKILL.md](SKILL.md) 的内容作为 System Prompt 或上下文提供给 AI 助手即可。

### 方式二：作为参考文档

阅读 SKILL.md，理解 SDD 工作法的流程和原则，手动指导 AI 按步骤执行。

### 方式三：配合 AI 工具

- **Reasonix**: `reasonix skill install` 安装后通过触发词加载
- **Claude Code / Cursor**: 将 SKILL.md 加入项目上下文（Project Rules / .cursorrules）
- **ChatGPT / Claude**: 直接将文档内容粘贴到对话中

---

## 典型工作流

1. **定方向** — AI 给出项目方向选项，你来选
2. **Constitution** — 起草项目核心原则，你审阅
3. **Spec** — 按业务层编写完整功能规格，含验收条件
4. **Plan** — 输出完整技术方案（结构/数据/API/UI规范）
5. **实现管道** — AI 逐层自动化实现，每层经过测试→质量门→UI校验
6. **用户视角自审** — AI 模拟用户走通所有流程，修复问题
7. **交付** — 生成完整交付包（代码+文档+测试报告）

---

## 设计哲学

| 原则 | 说明 |
|------|------|
| 不跳过决策闸门 | 设计阶段每步确认后再推进，避免返工 |
| 一次性设计，Solo 连续性执行 | 设计充分讨论，实现 AI 全权负责 |
| 完整性先行 | 业务逻辑必须闭环，不允许"此功能暂未实现"的断点 |
| 质量门自动拦截 | 测试/构建/代码质量/UI规范在管道内自动检查 |
| 可追溯 | Spec 和 Plan 确认后保存，实现变更记录到 changelog |

---

## 许可证

[MIT](LICENSE) © 2025 xiaojie

---

## 贡献

欢迎提交 Issue 和 PR！请确保：

1. 保持与现有工作流的一致性
2. 更新相关文档
3. 说明改动对设计/实现阶段的影响
