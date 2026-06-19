# 🤖 ai-human-sdd — SDD Human-AI Collaboration Methodology

> AI executes structure + user reviews, delivering a complete product business loop in one shot.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

> **🌐 中文版 👉 [README.zh.md](README.zh.md)**

---

## Introduction

**ai-human-sdd** is a **human-AI collaborative SDD (Spec-Driven Development) methodology** for end-to-end product delivery. It works with various AI coding assistants (Reasonix, Cursor, GitHub Copilot, Claude Code, etc.).

Core philosophy: **AI handles structure and execution; humans make decisions and review.**

The workflow has two phases:

```
Phase 1: Design
  Constitution → Spec → Plan (incl. UI style selection) → You approve

Phase 2: Implement
  Layer-by-layer automated delivery → Testing → Self-review → Ship
```

> You only make **four decisions**: set direction → review the plan → confirm self-review → accept delivery.
> AI handles all coding, testing, and optimization in between without interrupting you.

---

## How to Use

### Option 1: Use as a Prompt Template

Paste the contents of [SKILL.md](SKILL.md) as a system prompt or context to your AI assistant.

### Option 2: Use as a Reference

Read SKILL.md to understand the SDD workflow and principles, then guide your AI assistant through the steps manually.

### Option 3: Integrate with AI Tools

- **Reasonix**: Install via `reasonix skill install` and trigger by keywords
- **Claude Code / Cursor**: Add SKILL.md to project context (Project Rules / .cursorrules)
- **ChatGPT / Claude**: Paste the document directly into the conversation

---

## Typical Workflow

1. **Set Direction** — AI presents project options; you choose
2. **Constitution** — Draft core principles; you review
3. **Spec** — Write full feature specs by business layer with acceptance criteria
4. **Plan** — Output complete technical plan (structure / data / API / UI spec)
5. **Implementation Pipeline** — AI implements layer by layer with testing → quality gates → UI checks
6. **User Perspective Self-Review** — AI simulates the user journey, fixes issues
7. **Delivery** — Generate complete delivery package (code + docs + test report)

---

## Design Philosophy

| Principle | Description |
|-----------|-------------|
| No skipped decision gates | Every step in the design phase requires confirmation before proceeding |
| One-shot design, solo continuous execution | Full discussion upfront, AI handles all coding autonomously |
| Completeness first | Business logic must form a closed loop — no "coming soon" placeholders |
| Automatic quality gates | Tests, builds, code quality, UI consistency checked automatically |
| Traceability | Spec and Plan are saved; implementation changes are logged |

---

## License

[MIT](LICENSE) © 2025 xiaojie

---

## Contributing

Issues and PRs welcome! Please ensure:

1. Consistency with the existing workflow
2. Update related documentation
3. Explain the impact on design/implementation phases
