<p align="center">
  <img src="../assets/banner.svg" alt="Karpathy-Inspired Claude Skills Banner" width="100%">
</p>

# ಕಾರ್ಪಾಥಿ-ಪ್ರೇರಿತ ಕ್ಲಾಡ್ ಸ್ಕಿಲ್ಸ್ (Claude Skills) 🚀

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Version](https://img.shields.io/badge/version-1.1.0-blue.svg)](https://github.com/forrestchang/claude-skills-by-karpathy)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://makeapullrequest.com)
<a href="https://github.com/ishandutta2007"><img alt="GitHub followers" src="https://img.shields.io/github/followers/ishandutta2007?label=Follow&style=social" /></a>

> **SEO ಕೀವರ್ಡ್‌ಗಳು**: Claude Skills, AI Coding Best Practices, Karpathy Guidelines, Claude Code Plugin, Cursor Rules, LLM Coding Pitfalls, Sustainable AI Engineering.

ನನ್ನ ಹೊಸ ಪ್ರಾಜೆಕ್ಟ್ [Multica](https://github.com/multica-ai/multica) ನೋಡಿ — ಮರುಬಳಕೆ ಮಾಡಬಹುದಾದ (reusable) **Claude Skills** ನೊಂದಿಗೆ ಕೋಡಿಂಗ್ ಏಜೆಂಟ್‌ಗಳನ್ನು ನಡೆಸಲು ಮತ್ತು ನಿರ್ವಹಿಸಲು ಒಂದು ಓಪನ್ ಸೋರ್ಸ್ ಪ್ಲಾಟ್‌ಫಾರ್ಮ್. 🤖

X ನಲ್ಲಿ ನನ್ನನ್ನು ಫಾಲೋ ಮಾಡಿ: [https://x.com/jiayuan_jy](https://x.com/jiayuan_jy) 🐦

---

[English](../README.md) | [简体中文](./README_ZH.md) | [हिन्दी](./README_HI.md) | [বাংলা](./README_BN.md) | [मराठी](./README_MR.md) | [తెలుగు](./README_TE.md) | [தமிழ்](./README_TA.md) | [ગુજરાતી](./README_GU.md) | [اردو](./README_UR.md) | ಕನ್ನಡ

---

## 🌟 ಅವಲೋಕನ (Overview)

Claude Code ನ ನಡವಳಿಕೆಯನ್ನು ಸುಧಾರಿಸಲು ಮತ್ತು ಸಾಮಾನ್ಯ LLM ಕೋಡಿಂಗ್ ತಪ್ಪುಗಳನ್ನು ಕಡಿಮೆ ಮಾಡಲು ವಿನ್ಯಾಸಗೊಳಿಸಲಾದ **ಮಾಡ್ಯುಲರ್, ಪ್ರೀಮಿಯಂ ಕ್ಲಾಡ್ ಸ್ಕಿಲ್ಸ್ (Claude Skills)** ಸಂಗ್ರಹ. ಈ ತತ್ವಗಳನ್ನು AI ಕೋಡಿಂಗ್ ನ್ಯೂನತೆಗಳ ಕುರಿತು [ಆಂಡ್ರೆ ಕಾರ್ಪಾಥಿಯವರ ಅವಲೋಕನಗಳಿಂದ](https://x.com/karpathy/status/2015883857489522876) ಪಡೆಯಲಾಗಿದೆ.

---

## ⚠️ ಸಮಸ್ಯೆಗಳು (The Problems)

AI ಮಾಡೆಲ್‌ಗಳು ಹೆಚ್ಚಾಗಿ:
1.  ❌ ಪರಿಶೀಲಿಸದೆಯೇ **ತಪ್ಪು ಊಹೆಗಳನ್ನು** ಮಾಡುತ್ತವೆ.
2.  ❌ ಕೋಡ್ ಮತ್ತು API ಗಳನ್ನು ಅನಗತ್ಯವಾಗಿ ಸಂಕೀರ್ಣಗೊಳಿಸುತ್ತವೆ.
3.  ❌ ತಮಗೆ ಅರ್ಥವಾಗದ ಕೋಡ್ ಅಥವಾ ಕಾಮೆಂಟ್‌ಗಳನ್ನು ತೆಗೆದುಹಾಕುತ್ತವೆ.
4.  ❌ ಸಂಕೀರ್ಣ ಕಾರ್ಯಗಳಿಗಾಗಿ ಸ್ಪಷ್ಟ ಯಶಸ್ಸಿನ ಮಾನದಂಡಗಳ ಕೊರತೆಯನ್ನು ಹೊಂದಿರುತ್ತವೆ.

---

## 🛡️ ಪರಿಹಾರ: ಪ್ರೀಮಿಯಂ ಕ್ಲಾಡ್ ಸ್ಕಿಲ್ಸ್ (Claude Skills)

ಈ ಮಾಡ್ಯುಲರ್ **Claude Skills** ನೇರವಾಗಿ ಮೇಲಿನ ಸಮಸ್ಯೆಗಳನ್ನು ಪರಿಹರಿಸುತ್ತವೆ:

| ಸ್ಕಿಲ್ (Skill) | ವಿವರಣೆ (Description) | ಪರಿಹರಿಸುವ ಸಮಸ್ಯೆಗಳು (Addresses) |
| :--- | :--- | :--- |
| 🧠 **ಕೋಡಿಂಗ್ ಮಾಡುವ ಮುನ್ನ ಯೋಚಿಸಿ** | ಸ್ಪಷ್ಟ ತರ್ಕ ಮತ್ತು ಊಹೆಗಳನ್ನು ಹೊರತರಲು ಒತ್ತಾಯಿಸುತ್ತದೆ. | ಗುಪ್ತ ಗೊಂದಲ, ತಪ್ಪು ಊಹೆಗಳು. |
| 🍃 **ಸರಳತೆಗೆ ಮೊದಲ ಆದ್ಯತೆ** | ಸಮಸ್ಯೆಯನ್ನು ಪರಿಹರಿಸಲು ಕನಿಷ್ಠ ಕೋಡ್. ಯಾವುದೇ ಊಹೆಗಳಿಲ್ಲ. | ಅತಿಯಾದ ಸಂಕೀರ್ಣತೆ, ಭಾರೀ ಅಬ್‌ಸ್ಟ್ರಾಕ್ಷನ್‌ಗಳು. |
| 🎯 **ನಿಖರ ಬದಲಾವಣೆಗಳು** | ಅಗತ್ಯವಿರುವುದನ್ನು ಮಾತ್ರ ಸ್ಪರ್ಶಿಸಿ. ಅಸ್ತಿತ್ವದಲ್ಲಿರುವ ಶೈಲಿಯನ್ನು ಅನುಸರಿಸಿ. | ಅಪ್ರಸ್ತುತ ಸಂಪಾದನೆಗಳು, ಶೈಲಿಯ ಬದಲಾವಣೆ. |
| ✅ **ಗುರಿ-ಆಧಾರಿತ ಅನುಷ್ಠಾನ** | ಯಶಸ್ಸಿನ ಮಾನದಂಡಗಳನ್ನು ವ್ಯಾಖ್ಯಾನಿಸಿ ಮತ್ತು ಪರಿಶೀಲಿಸುವವರೆಗೆ ಲೂಪ್ ಮಾಡಿ. | ಇಂಪರೇಟಿವ್ (Imperative) ವರ್ಸಸ್ ಡಿಕ್ಲರೇಟಿವ್ (Declarative) ನಡುವಿನ ಅಂತರ. |

---

## 📦 ಮಾಡ್ಯುಲರ್ ಕ್ಲಾಡ್ ಸ್ಕಿಲ್ಸ್ ವಿವರವಾಗಿ

### 1. ಕೋಡಿಂಗ್ ಮಾಡುವ ಮುನ್ನ ಯೋಚಿಸಿ (Think Before Coding)
**ಊಹೆ ಮಾಡಬೇಡಿ. ಗೊಂದಲವನ್ನು ಮರೆಮಾಡಬೇಡಿ. ಟ್ರೇಡ್-ಆಫ್‌ಗಳನ್ನು ಹೊರತನ್ನಿ.**
ಈ ಸ್ಕಿಲ್ ನಿಮ್ಮ AI ಪಾಲುದಾರ ಕೋಡ್‌ನ ಒಂದು ಸಾಲನ್ನು ಸ್ಪರ್ಶಿಸುವ ಮೊದಲೇ ಸ್ಪಷ್ಟವಾಗಿ ತರ್ಕಿಸುವುದನ್ನು ಖಚಿತಪಡಿಸುತ್ತದೆ.

### 2. ಸರಳತೆಗೆ ಮೊದಲ ಆದ್ಯತೆ (Simplicity First)
**ಸಮಸ್ಯೆಯನ್ನು ಪರಿಹರಿಸುವ ಕನಿಷ್ಠ ಕೋಡ್. ಯಾವುದೂ ಕಾಲ್ಪನಿಕವಲ್ಲ.**
ಓವರ್-ಇಂಜಿನಿಯರಿಂಗ್ ಪ್ರವೃತ್ತಿಯ ವಿರುದ್ಧ ಹೋರಾಡಿ. 200 ಸಾಲುಗಳ ಕೋಡ್ ಅನ್ನು 50 ಸಾಲುಗಳಲ್ಲಿ ಮಾಡಬಹುದಾದರೆ, ಅದನ್ನು ಮತ್ತೆ ಬರೆಯಿರಿ.

### 3. ನಿಖರ ಬದಲಾವಣೆಗಳು (Surgical Changes)
**ನೀವು ಸ್ಪರ್ಶಿಸಬೇಕಾದದ್ದನ್ನು ಮಾತ್ರ ಸ್ಪರ್ಶಿಸಿ. ನೀವು ಮಾಡಿದ ಗೊಂದಲವನ್ನು ಮಾತ್ರ ಸ್ವಚ್ಛಗೊಳಿಸಿ.**
ನಿಖರವಾದ ಸಂಪಾದನೆಗಳ ಮೇಲೆ ಗಮನಹರಿಸಿ. ನೀವು ವಿಭಿನ್ನವಾಗಿ ಮಾಡಲು ಇಷ್ಟಪಟ್ಟರೂ ಸಹ, ಪ್ರಾಜೆಕ್ಟ್‌ನ ಅಸ್ತಿತ್ವದಲ್ಲಿರುವ ಶೈಲಿಗೆ ಹೊಂದಿಸಿ.

### 4. ಗುರಿ-ಆಧಾರಿತ ಅನುಷ್ಠಾನ (Goal-Driven Execution)
**ಯಶಸ್ಸಿನ ಮಾನದಂಡಗಳನ್ನು ವ್ಯಾಖ್ಯಾನಿಸಿ. ಪರಿಶೀಲಿಸುವವರೆಗೆ ಲೂಪ್ ಮಾಡಿ.**
ಅಸ್ಪಷ್ಟ ಕಾರ್ಯಗಳನ್ನು ನಿರ್ದಿಷ್ಟ ಯಶಸ್ಸಿನ ಮೆಟ್ರಿಕ್‌ಗಳೊಂದಿಗೆ ಪರಿಶೀಲಿಸಬಹುದಾದ ಗುರಿಗಳಾಗಿ ಪರಿವರ್ತಿಸಿ.

---

## 🚀 ಅನುಸ್ಥಾಪನೆ (Installation)

### ಆಯ್ಕೆ A: Claude Code ಪ್ಲಗಿನ್ (ಶಿಫಾರಸು ಮಾಡಲಾಗಿದೆ)

ಮಾರ್ಕೆಟ್‌ಪ್ಲೇಸ್ ಸೇರಿಸಿ ಮತ್ತು **Claude Skills** ಸ್ಥಾಪಿಸಿ:

```bash
/plugin marketplace add forrestchang/claude-skills-by-karpathy
/plugin install claude-skills-by-karpathy@karpathy-skills
```

### ಆಯ್ಕೆ B: CLAUDE.md (ಪ್ರಾಜೆಕ್ಟ್-ವಾರು)

```bash
curl -o CLAUDE.md https://raw.githubusercontent.com/forrestchang/claude-skills-by-karpathy/main/CLAUDE.md
```

---

## 🛠️ ಟೂಲ್ ಸಪೋರ್ಟ್ (Tool Support)

*   **Cursor**: ನಮ್ಮ ಪ್ರಾಜೆಕ್ಟ್ ನಿಯಮಗಳನ್ನು ಬಳಸಿಕೊಂಡು ಈ ಸ್ಕಿಲ್‌ಗಳನ್ನು ಸ್ವಯಂಚಾಲಿತವಾಗಿ ಅನ್ವಯಿಸಿ. **[docs/cursor-setup.md](../docs/cursor-setup.md)** ನೋಡಿ.
*   **ಉದಾಹರಣೆಗಳು**: **[docs/examples.md](../docs/examples.md)** ನಲ್ಲಿ ನೈಜ-ಪ್ರಪಂಚದ ರೂಪಾಂತರಗಳನ್ನು ನೋಡಿ.

---

## 🤝 ಕೊಡುಗೆ (Contributing)

ಕೊಡುಗೆಗಳನ್ನು ಸ್ವಾಗತಿಸಲಾಗುತ್ತದೆ! ನಿಮ್ಮಲ್ಲಿ ಹೊಸ **Claude Skill** ಇದ್ದರೆ ಅಥವಾ ಅಸ್ತಿತ್ವದಲ್ಲಿರುವ ಸ್ಕಿಲ್‌ಗಳ ಸುಧಾರಣೆ ಇದ್ದರೆ, ದಯವಿಟ್ಟು PR ಅನ್ನು ತೆರೆಯಿರಿ.

## 📄 ಪರವಾನಗಿ (License)

MIT © [forrestchang](https://github.com/forrestchang)

## 📈 ಸ್ಟಾರ್ ಹಿಸ್ಟರಿ (Star History)
<div align="center">
   <a href="https://www.star-history.com/repos=ishandutta2007%2Fclaude-skills-by-karpathy&type=date&legend=bottom-right">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/chart?repos=ishandutta2007/claude-skills-by-karpathy&type=date&theme=dark&legend=bottom-right" />
      <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/chart?repos=ishandutta2007/claude-skills-by-karpathy&type=date&legend=bottom-right" />
      <img alt="Star History Chart" src="https://api.star-history.com/chart?repos=ishandutta2007/claude-skills-by-karpathy&type=date&legend=bottom-right" />
    </picture>
   </a>
</div>
