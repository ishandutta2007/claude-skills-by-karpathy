<p align="center">
  <img src="../assets/banner.svg" alt="Karpathy-Inspired Claude Skills Banner" width="100%">
</p>

# Karpathy-प्रेरित Claude Skills 🚀

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Version](https://img.shields.io/badge/version-1.1.0-blue.svg)](https://github.com/forrestchang/claude-skills-by-karpathy)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://makeapullrequest.com)
<a href="https://github.com/ishandutta2007"><img alt="GitHub followers" src="https://img.shields.io/github/followers/ishandutta2007?label=Follow&style=social" /></a>

> **SEO Keywords**: Claude Skills, AI Coding Best Practices, Karpathy Guidelines, Claude Code Plugin, Cursor Rules, LLM Coding Pitfalls, Sustainable AI Engineering.

मेरे नए प्रोजेक्ट [Multica](https://github.com/multica-ai/multica) को देखें — पुन: प्रयोज्य (reusable) **Claude Skills** के साथ कोडिंग एजेंटों को चलाने और प्रबंधित करने के लिए एक ओपन-सोर्स प्लेटफॉर्म। 🤖

मुझे X पर फॉलो करें: [https://x.com/jiayuan_jy](https://x.com/jiayuan_jy) 🐦

---

## 🌟 अवलोकन (Overview)

Claude Code के व्यवहार में सुधार करने और सामान्य LLM कोडिंग गलतियों को कम करने के लिए डिज़ाइन किए गए **मॉड्यूलर, प्रीमियम Claude Skills** का एक संग्रह। ये सिद्धांत AI कोडिंग की कमियों पर [Andrej Karpathy के अवलोकनों](https://x.com/karpathy/status/2015883857489522876) से लिए गए हैं।

[English](../README.md) | [简体中文](./README_ZH.md) | हिन्दी 🇮🇳

---

## ⚠️ समस्याएं (The Problems)

AI मॉडल अक्सर:
1.  ❌ बिना जांचे **गलत धारणाएं** बना लेते हैं।
2.  ❌ कोड और API को जटिल बना देते हैं।
3.  ❌ उस कोड या कमेंट्स को हटा देते हैं जिन्हें वे समझ नहीं पाते।
4.  ❌ जटिल कार्यों के लिए सफलता के स्पष्ट मानदंडों की कमी होती है।

---

## 🛡️ समाधान: प्रीमियम Claude Skills

ये मॉड्यूलर **Claude Skills** सीधे ऊपर दी गई समस्याओं का समाधान करते हैं:

| स्किल (Skill) | विवरण (Description) | समाधान (Addresses) |
| :--- | :--- | :--- |
| 🧠 **कोडिंग से पहले सोचें** | स्पष्ट तर्क और धारणाओं को सामने लाने के लिए मजबूर करता है। | छिपी हुई उलझन, गलत धारणाएं। |
| 🍃 **सादगी सबसे पहले** | समस्या को हल करने के लिए आवश्यक न्यूनतम कोड। कोई अटकलें नहीं। | अत्यधिक जटिलता, भारी एब्स्ट्रैक्शंस। |
| 🎯 **सटीक बदलाव** | केवल वही छुएं जो आवश्यक है। मौजूदा शैली का पालन करें। | असंबद्ध संपादन, शैली में बदलाव। |
| ✅ **लक्ष्य-आधारित निष्पादन** | सफलता के मानदंड परिभाषित करें और सत्यापित होने तक लूप करें। | आदेशात्मक (Imperative) बनाम घोषणात्मक (Declarative) अंतराल। |

---

## 📦 मॉड्यूलर Claude Skills विस्तार से

### 1. कोडिंग से पहले सोचें (Think Before Coding)
**धारणाएं न बनाएं। उलझन न छिपाएं। समझौतों (tradeoffs) को सामने लाएं।**
यह स्किल यह सुनिश्चित करता है कि आपका AI पार्टनर कोड की एक भी लाइन छूने से पहले स्पष्ट रूप से तर्क दे।

### 2. सादगी सबसे पहले (Simplicity First)
**न्यूनतम कोड जो समस्या का समाधान करे। कोई अटकलें नहीं।**
ओवरइंजीनियरिंग की प्रवृत्ति से लड़ें। यदि 200 लाइनें 50 हो सकती हैं, तो उन्हें फिर से लिखें।

### 3. सटीक बदलाव (Surgical Changes)
**केवल वही छुएं जो आपको छूना चाहिए। केवल अपनी बनाई गंदगी को साफ करें।**
सटीक संपादन पर ध्यान दें। प्रोजेक्ट की मौजूदा शैली का मिलान करें, भले ही आप इसे अलग तरह से करना पसंद करें।

### 4. लक्ष्य-आधारित निष्पादन (Goal-Driven Execution)
**सफलता के मानदंड परिभाषित करें। सत्यापित होने तक लूप करें।**
अस्पष्ट कार्यों को विशिष्ट सफलता मेट्रिक्स के साथ सत्यापन योग्य लक्ष्यों में बदलें।

---

## 🚀 इंस्टालेशन (Installation)

### विकल्प A: Claude Code प्लगइन (अनुशंसित)

मार्केटप्लेस जोड़ें और **Claude Skills** इंस्टॉल करें:

```bash
/plugin marketplace add forrestchang/claude-skills-by-karpathy
/plugin install claude-skills-by-karpathy@karpathy-skills
```

### विकल्प B: CLAUDE.md (प्रति-प्रोजेक्ट)

```bash
curl -o CLAUDE.md https://raw.githubusercontent.com/forrestchang/claude-skills-by-karpathy/main/CLAUDE.md
```

---

## 🛠️ टूल सपोर्ट (Tool Support)

*   **Cursor**: हमारे प्रोजेक्ट नियमों का उपयोग करके इन स्किल्स को स्वचालित रूप से लागू करें। **[docs/cursor-setup.md](../docs/cursor-setup.md)** देखें।
*   **उदाहरण**: **[docs/examples.md](../docs/examples.md)** में वास्तविक दुनिया के बदलाव देखें।

---

## 🤝 योगदान (Contributing)

योगदान का स्वागत है! यदि आपके पास एक नया **Claude Skill** है या मौजूदा स्किल्स में सुधार है, तो कृपया एक PR खोलें।

## 📄 लाइसेंस (License)

MIT © [forrestchang](https://github.com/forrestchang)

## 📈 स्टार हिस्ट्री (Star History)
<div align="center">
   <a href="https://www.star-history.com/repos=ishandutta2007%2Fclaude-skills-by-karpathy&type=date&legend=bottom-right">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/chart?repos=ishandutta2007/claude-skills-by-karpathy&type=date&theme=dark&legend=bottom-right" />
      <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/chart?repos=ishandutta2007/claude-skills-by-karpathy&type=date&legend=bottom-right" />
      <img alt="Star History Chart" src="https://api.star-history.com/chart?repos=ishandutta2007/claude-skills-by-karpathy&type=date&legend=bottom-right" />
    </picture>
   </a>
</div>
