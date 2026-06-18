<p align="center">
  <img src="../assets/banner.svg" alt="Karpathy-Inspired Claude Skills Banner" width="100%">
</p>

# कार्पॅथी-प्रेरित क्लॉड स्किल्स (Claude Skills) 🚀

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Version](https://img.shields.io/badge/version-1.1.0-blue.svg)](https://github.com/forrestchang/claude-skills-by-karpathy)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://makeapullrequest.com)
<a href="https://github.com/ishandutta2007"><img alt="GitHub followers" src="https://img.shields.io/github/followers/ishandutta2007?label=Follow&style=social" /></a>

> **SEO कीवर्ड**: Claude Skills, AI Coding Best Practices, Karpathy Guidelines, Claude Code Plugin, Cursor Rules, LLM Coding Pitfalls, Sustainable AI Engineering.

माझा नवीन प्रकल्प [Multica](https://github.com/multica-ai/multica) पहा — पुन्हा वापरण्यायोग्य (reusable) **Claude Skills** सह कोडिंग एजंट्स चालवण्यासाठी आणि व्यवस्थापित करण्यासाठी एक ओपन-सोर्स प्लॅटफॉर्म. 🤖

मला X वर फॉलो करा: [https://x.com/jiayuan_jy](https://x.com/jiayuan_jy) 🐦

---

[English](../README.md) | [简体中文](./README_ZH.md) | [हिन्दी](./README_HI.md) | [বাংলা](./README_BN.md) | मराठी | [తెలుగు](./README_TE.md) | [தமிழ்](./README_TA.md) | [ગુજરાતી](./README_GU.md) | [اردو](./README_UR.md) | [ಕನ್ನಡ](./README_KN.md)

---

## 🌟 विहंगावलोकन (Overview)

Claude Code च्या वर्तनात सुधारणा करण्यासाठी आणि सामान्य LLM कोडिंग चुका कमी करण्यासाठी डिझाइन केलेल्या **मॉड्यूलर, प्रीमियम क्लॉड स्किल्स (Claude Skills)** चा संग्रह. ही तत्त्वे AI कोडिंगमधील उणिवांवरील [आंद्रे कार्पॅथी यांच्या निरीक्षणांवरून](https://x.com/karpathy/status/2015883857489522876) घेतली आहेत.

---

## ⚠️ समस्या (The Problems)

AI मॉडेल्स अनेकदा:
1.  ❌ तपासल्याशिवाय **चुकीच्या समजूती** करून घेतात.
2.  ❌ कोड आणि API ला विनाकारण गुंतागुंतीचे बनवतात.
3.  ❌ त्यांना समजत नसलेला कोड किंवा कमेंट्स काढून टाकतात.
4.  ❌ जटिल कामांसाठी यशाच्या स्पष्ट निकषांचा अभाव असतो.

---

## 🛡️ उपाय: प्रीमियम क्लॉड स्किल्स (Claude Skills)

हे मॉड्यूलर **Claude Skills** थेट वरील समस्यांचे निराकरण करतात:

| स्किल (Skill) | वर्णन (Description) | उपाय (Addresses) |
| :--- | :--- | :--- |
| 🧠 **कोडिंगपूर्वी विचार करा** | स्पष्ट तर्क आणि समजूती समोर आणण्यास भाग पाडते. | सुप्त गोंधळ, चुकीच्या समजूती. |
| 🍃 **साधेपणा प्रथम** | समस्या सोडवण्यासाठी किमान कोड. कोणताही अंदाज नाही. | अति-जटिलता, विनाकारण एब्स्ट्रॅक्शन्स. |
| 🎯 **अचूक बदल** | फक्त जे आवश्यक आहे त्यालाच स्पर्श करा. विद्यमान शैलीचे पालन करा. | असंबद्ध संपादन, शैली बदलणे. |
| ✅ **ध्येय-आधारित अंमलबजावणी** | यशाचे निकष परिभाषित करा आणि सत्यापित होईपर्यंत लूप करा. | आदेशात्मक (Imperative) विरुद्ध घोषणात्मक (Declarative) तफावत. |

---

## 📦 मॉड्यूलर क्लॉड स्किल्स सविस्तर

### १. कोडिंगपूर्वी विचार करा (Think Before Coding)
**समजूती करून घेऊ नका. गोंधळ लपवू नका. तडजोडी (tradeoffs) समोर आणा.**
हे स्किल हे सुनिश्चित करते की तुमचा AI पार्टनर कोडची एकही ओळ स्पर्श करण्यापूर्वी स्पष्टपणे तर्क मांडेल.

### २. साधेपणा प्रथम (Simplicity First)
**किमान कोड जो समस्येचे निराकरण करतो. काहीही काल्पनिक नाही.**
ओव्हर-इंजिनियरिंगच्या प्रवृत्तीशी लढा. जर २०० ओळींचे काम ५० ओळींमध्ये होऊ शकत असेल, तर ते पुन्हा लिहा.

### ३. अचूक बदल (Surgical Changes)
**फक्त जे स्पर्श केले पाहिजे त्यालाच स्पर्श करा. फक्त तुमची स्वतःची केलेली घाण साफ करा.**
अचूक संपादनावर लक्ष केंद्रित करा. प्रकल्पाच्या विद्यमान शैलीशी जुळवून घ्या, जरी तुम्हाला ती वेगळ्या प्रकारे करायला आवडली असती तरीही.

### ४. ध्येय-आधारित अंमलबजावणी (Goal-Driven Execution)
**यशाचे निकष परिभाषित करा. सत्यापित होईपर्यंत लूप करा.**
अस्पष्ट कामांना विशिष्ट यश मेट्रिक्ससह सत्यापित करण्यायोग्य लक्ष्यांमध्ये रूपांतरित करा.

---

## 🚀 इन्स्टॉलेशन (Installation)

### पर्याय A: Claude Code प्लगइन (शिफारस केलेले)

मार्केटप्लेस जोडा आणि **Claude Skills** इन्स्टॉल करा:

```bash
/plugin marketplace add forrestchang/claude-skills-by-karpathy
/plugin install claude-skills-by-karpathy@karpathy-skills
```

### पर्याय B: CLAUDE.md (प्रत्येक प्रकल्पासाठी)

```bash
curl -o CLAUDE.md https://raw.githubusercontent.com/forrestchang/claude-skills-by-karpathy/main/CLAUDE.md
```

---

## 🛠️ टूल सपोर्ट (Tool Support)

*   **Cursor**: आमच्या प्रकल्पाचे नियम वापरून ही कौशल्ये स्वयंचलितपणे लागू करा. **[docs/cursor-setup.md](../docs/cursor-setup.md)** पहा.
*   **उदाहरणे**: **[docs/examples.md](../docs/examples.md)** मध्ये वास्तविक जगातील बदल पहा.

---

## 🤝 योगदान (Contributing)

योगदानाचे स्वागत आहे! जर तुमच्याकडे नवीन **Claude Skill** असेल किंवा विद्यमान स्किल्समध्ये सुधारणा असेल, तर कृपया एक PR उघडा.

## 📄 परवाना (License)

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
