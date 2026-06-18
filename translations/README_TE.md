<p align="center">
  <img src="../assets/banner.svg" alt="Karpathy-Inspired Claude Skills Banner" width="100%">
</p>

# కార్పతీ-ప్రేరిత క్లాడ్ స్కిల్స్ (Claude Skills) 🚀

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Version](https://img.shields.io/badge/version-1.1.0-blue.svg)](https://github.com/forrestchang/claude-skills-by-karpathy)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://makeapullrequest.com)
<a href="https://github.com/ishandutta2007"><img alt="GitHub followers" src="https://img.shields.io/github/followers/ishandutta2007?label=Follow&style=social" /></a>

> **SEO కీవర్డ్లు**: Claude Skills, AI Coding Best Practices, Karpathy Guidelines, Claude Code Plugin, Cursor Rules, LLM Coding Pitfalls, Sustainable AI Engineering.

నా కొత్త ప్రాజెక్ట్ [Multica](https://github.com/multica-ai/multica) చూడండి — పునర్వినియోగపరచదగిన (reusable) **Claude Skills** తో కోడింగ్ ఏజెంట్లను నడపడానికి మరియు నిర్వహించడానికి ఒక ఓపెన్-సోర్స్ ప్లాట్‌ఫారమ్. 🤖

X లో నన్ను అనుసరించండి: [https://x.com/jiayuan_jy](https://x.com/jiayuan_jy) 🐦

---

[English](../README.md) | [简体中文](./README_ZH.md) | [हिन्दी](./README_HI.md) | [বাংলা](./README_BN.md) | [मराठी](./README_MR.md) | తెలుగు | [தமிழ்](./README_TA.md) | [ગુજરાતી](./README_GU.md) | [اردو](./README_UR.md) | [ಕನ್ನಡ](./README_KN.md)

---

## 🌟 అవలోకనం (Overview)

Claude Code ప్రవర్తనను మెరుగుపరచడానికి మరియు సాధారణ LLM కోడింగ్ తప్పులను తగ్గించడానికి రూపొందించిన **మాడ్యులర్, ప్రీమియం క్లాడ్ స్కిల్స్ (Claude Skills)** సేకరణ. ఈ సూత్రాలు AI కోడింగ్ లోపాలపై [ఆండ్రీ కార్పతీ పరిశీలనల](https://x.com/karpathy/status/2015883857489522876) నుండి తీసుకోబడ్డాయి.

---

## ⚠️ సమస్యలు (The Problems)

AI మోడల్స్ తరచుగా:
1.  ❌ తనిఖీ చేయకుండానే **తప్పుడు అంచనాలు** వేస్తాయి.
2.  ❌ కోడ్ మరియు APIలను అనవసరంగా క్లిష్టతరం చేస్తాయి.
3.  ❌ వాటికి అర్థం కాని కోడ్ లేదా కామెంట్లను తొలగిస్తాయి.
4.  ❌ సంక్లిష్టమైన పనుల కోసం స్పష్టమైన విజయ ప్రమాణాల కొరత ఉంటుంది.

---

## 🛡️ పరిష్కారం: ప్రీమియం క్లాడ్ స్కిల్స్ (Claude Skills)

ఈ మాడ్యులర్ **Claude Skills** నేరుగా పైన పేర్కొన్న సమస్యలను పరిష్కరిస్తాయి:

| స్కిల్ (Skill) | వివరణ (Description) | పరిష్కారం (Addresses) |
| :--- | :--- | :--- |
| 🧠 **కోడింగ్ ముందు ఆలోచించండి** | స్పష్టమైన తార్కికతను మరియు అంచనాలను బయటకు తెస్తుంది. | దాగి ఉన్న గందరగోళం, తప్పుడు అంచనాలు. |
| 🍃 **సరళతకు ప్రాధాన్యత** | సమస్యను పరిష్కరించడానికి అవసరమైన కనీస కోడ్. ఊహలు వద్దు. | మితిమీరిన సంక్లిష్టత, భారీ అబ్స్ట్రాక్షన్లు. |
| 🎯 **ఖచ్చితమైన మార్పులు** | అవసరమైన వాటిని మాత్రమే తాకండి. ఉన్న స్టైల్‌ను అనుసరించండి. | సంబంధం లేని సవరణలు, స్టైల్ మార్పులు. |
| ✅ **లక్ష్య ఆధారిత అమలు** | విజయ ప్రమాణాలను నిర్వచించండి మరియు ధృవీకరించబడే వరకు లూప్ చేయండి. | ఇంపరేటివ్ (Imperative) వర్సెస్ డిక్లరేటివ్ (Declarative) మధ్య అంతరం. |

---

## 📦 మాడ్యులర్ క్లాడ్ స్కిల్స్ వివరంగా

### 1. కోడింగ్ ముందు ఆలోచించండి (Think Before Coding)
**అంచనాలు వేయవద్దు. గందరగోళాన్ని దాచవద్దు. ట్రేడ్-ఆఫ్స్‌ను బయటకు తెండి.**
ఈ స్కిల్ మీ AI భాగస్వామి కోడ్ యొక్క ఒక్క లైన్‌ను కూడా తాకకముందే స్పష్టంగా తార్కికతను వివరించేలా చేస్తుంది.

### 2. సరళతకు ప్రాధాన్యత (Simplicity First)
**సమస్యను పరిష్కరించే కనీస కోడ్. ఊహాజనితమైనది ఏదీ వద్దు.**
ఓవర్‌ ఇంజనీరింగ్ ధోరణితో పోరాడండి. 200 లైన్ల కోడ్‌ను 50 లైన్లలో చేయగలిగితే, దాన్ని మళ్ళీ రాయండి.

### 3. ఖచ్చితమైన మార్పులు (Surgical Changes)
**మీరు తాకవలసిన వాటిని మాత్రమే తాకండి. మీరు చేసిన మార్పులను మాత్రమే శుభ్రం చేయండి.**
ఖచ్చితమైన సవరణలపై దృష్టి పెట్టండి. మీరు విభిన్నంగా చేయాలనుకున్నప్పటికీ, ప్రాజెక్ట్ యొక్క ఉన్న స్టైల్‌తో సరిపోల్చండి.

### 4. లక్ష్య ఆధారిత అమలు (Goal-Driven Execution)
**విజయ ప్రమాణాలను నిర్వచించండి. ధృవీకరించబడే వరకు లూప్ చేయండి.**
అస్పష్టమైన పనులను నిర్దిష్ట విజయ మెట్రిక్స్‌తో ధృవీకరించదగిన లక్ష్యాలుగా మార్చండి.

---

## 🚀 ఇన్‌స్టాలేషన్ (Installation)

### ఆప్షన్ A: Claude Code ప్లగ్ఇన్ (సిఫార్సు చేయబడినది)

మార్కెట్‌ప్లేస్‌ను జోడించి, **Claude Skills** ఇన్‌స్టాల్ చేయండి:

```bash
/plugin marketplace add forrestchang/claude-skills-by-karpathy
/plugin install claude-skills-by-karpathy@karpathy-skills
```

### ఆప్షన్ B: CLAUDE.md (ప్రాజెక్ట్ వారీగా)

```bash
curl -o CLAUDE.md https://raw.githubusercontent.com/forrestchang/claude-skills-by-karpathy/main/CLAUDE.md
```

---

## 🛠️ టూల్ సపోర్ట్ (Tool Support)

*   **Cursor**: మా ప్రాజెక్ట్ రూల్స్ ఉపయోగించి ఈ స్కిల్స్‌ను ఆటోమేటిక్‌గా వర్తింపజేయండి. **[docs/cursor-setup.md](../docs/cursor-setup.md)** చూడండి.
*   **ఉదాహరణలు**: **[docs/examples.md](../docs/examples.md)** లో వాస్తవ ప్రపంచ మార్పులను చూడండి.

---

## 🤝 సహకారం (Contributing)

సహకారాలు స్వాగతించబడతాయి! మీ దగ్గర కొత్త **Claude Skill** ఉంటే లేదా ఉన్నవాటిలో మెరుగుదలలు ఉంటే, దయచేసి PR తెరవండి.

## 📄 లైసెన్స్ (License)

MIT © [forrestchang](https://github.com/forrestchang)

## 📈 స్టార్ హిస్టరీ (Star History)
<div align="center">
   <a href="https://www.star-history.com/repos=ishandutta2007%2Fclaude-skills-by-karpathy&type=date&legend=bottom-right">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/chart?repos=ishandutta2007/claude-skills-by-karpathy&type=date&theme=dark&legend=bottom-right" />
      <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/chart?repos=ishandutta2007/claude-skills-by-karpathy&type=date&legend=bottom-right" />
      <img alt="Star History Chart" src="https://api.star-history.com/chart?repos=ishandutta2007/claude-skills-by-karpathy&type=date&legend=bottom-right" />
    </picture>
   </a>
</div>
