<p align="center">
  <img src="assets/banner.svg" alt="Karpathy-Inspired Claude Skills Banner" width="100%">
</p>

# Karpathy-Inspired Claude Skills 🚀

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Version](https://img.shields.io/badge/version-1.1.0-blue.svg)](https://github.com/forrestchang/claude-skills-by-karpathy)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://makeapullrequest.com)
<a href="https://github.com/ishandutta2007"><img alt="GitHub followers" src="https://img.shields.io/github/followers/ishandutta2007?label=Follow&style=social" /></a>

> **SEO Keywords**: Claude Skills, AI Coding Best Practices, Karpathy Guidelines, Claude Code Plugin, Cursor Rules, LLM Coding Pitfalls, Sustainable AI Engineering.

Check out my new project [Multica](https://github.com/multica-ai/multica) — an open-source platform for running and managing coding agents with reusable **Claude Skills**. 🤖

Follow me on X: [https://x.com/jiayuan_jy](https://x.com/jiayuan_jy) 🐦

---

## 🌟 Overview

A collection of **modular, premium Claude Skills** designed to drastically improve Claude Code behavior and reduce common LLM coding mistakes. These principles are derived from [Andrej Karpathy's observations](https://x.com/karpathy/status/2015883857489522876) on AI coding pitfalls.

English | [简体中文](./translations/README_ZH.md) | [हिन्दी](./translations/README_HI.md) | [বাংলা](./translations/README_BN.md) | [मराठी](./translations/README_MR.md) | [తెలుగు](./translations/README_TE.md) | [தமிழ்](./translations/README_TA.md) | [ગુજરાતી](./translations/README_GU.md) | [اردو](./translations/README_UR.md) | [ಕನ್ನಡ](./translations/README_KN.md)

---

## ⚠️ The Problems

AI models often:
1.  ❌ **Make wrong assumptions** without checking.
2.  ❌ **Overcomplicate code** and APIs with bloated abstractions.
3.  ❌ **Remove orthogonal code** or comments they don't understand.
4.  ❌ **Lack clear success criteria** for complex tasks.

---

## 🛡️ The Solution: Premium Claude Skills

These modular **Claude Skills** directly address the issues above:

| Skill | Description | Addresses |
| :--- | :--- | :--- |
| 🧠 **Think Before Coding** | Forces explicit reasoning and surfaces assumptions. | Hidden confusion, wrong assumptions. |
| 🍃 **Simplicity First** | Minimal code that solves the problem. No speculation. | Overcomplication, bloated abstractions. |
| 🎯 **Surgical Changes** | Touch only what you must. Match existing style. | Orthogonal edits, style drift. |
| ✅ **Goal-Driven Execution** | Define success criteria and loop until verified. | Imperative vs Declarative gaps. |

---

## 📦 Modular Claude Skills in Detail

### 1. Think Before Coding
**Don't assume. Don't hide confusion. Surface tradeoffs.**
This skill ensures your AI partner explicitly reasons before touching a single line of code.

### 2. Simplicity First
**Minimum code that solves the problem. Nothing speculative.**
Combat the tendency toward overengineering. If 200 lines could be 50, rewrite it.

### 3. Surgical Changes
**Touch only what you must. Clean up only your own mess.**
Focus on precise edits. Match the project's existing style even if you'd do it differently.

### 4. Goal-Driven Execution
**Define success criteria. Loop until verified.**
Transform vague tasks into verifiable goals with specific success metrics.

---

## 🚀 Installation

### Option A: Claude Code Plugin (Recommended)

Add the marketplace and install the **Claude Skills**:

```bash
/plugin marketplace add forrestchang/claude-skills-by-karpathy
/plugin install claude-skills-by-karpathy@karpathy-skills
```

### Option B: CLAUDE.md (Per-Project)

```bash
curl -o CLAUDE.md https://raw.githubusercontent.com/forrestchang/claude-skills-by-karpathy/main/CLAUDE.md
```

---

## 🛠️ Tool Support

*   **Cursor**: Apply these skills automatically using our project rules. See **[docs/cursor-setup.md](docs/cursor-setup.md)**.
*   **Examples**: See real-world transformations in **[docs/examples.md](docs/examples.md)**.

---

## 🤝 Contributing

Contributions are welcome! If you have a new **Claude Skill** or a refinement to existing ones, please open a PR.

## 📄 License

MIT © [forrestchang](https://github.com/forrestchang)

## 📈 Star History
<div align="center">
   <a href="https://www.star-history.com/repos=ishandutta2007%2Fclaude-skills-by-karpathy&type=date&legend=bottom-right">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/chart?repos=ishandutta2007/claude-skills-by-karpathy&type=date&theme=dark&legend=bottom-right" />
      <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/chart?repos=ishandutta2007/claude-skills-by-karpathy&type=date&legend=bottom-right" />
      <img alt="Star History Chart" src="https://api.star-history.com/chart?repos=ishandutta2007/claude-skills-by-karpathy&type=date&legend=bottom-right" />
    </picture>
   </a>
</div>
