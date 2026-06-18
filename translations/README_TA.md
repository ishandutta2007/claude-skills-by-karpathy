<p align="center">
  <img src="../assets/banner.svg" alt="Karpathy-Inspired Claude Skills Banner" width="100%">
</p>

# கார்பதி-ஈர்க்கப்பட்ட கிளாட் திறன்கள் (Claude Skills) 🚀

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Version](https://img.shields.io/badge/version-1.1.0-blue.svg)](https://github.com/forrestchang/claude-skills-by-karpathy)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://makeapullrequest.com)
<a href="https://github.com/ishandutta2007"><img alt="GitHub followers" src="https://img.shields.io/github/followers/ishandutta2007?label=Follow&style=social" /></a>

> **SEO முக்கிய வார்த்தைகள்**: Claude Skills, AI Coding Best Practices, Karpathy Guidelines, Claude Code Plugin, Cursor Rules, LLM Coding Pitfalls, Sustainable AI Engineering.

எனது புதிய திட்டமான [Multica](https://github.com/multica-ai/multica)-வைப் பாருங்கள் — மீண்டும் பயன்படுத்தக்கூடிய (reusable) **Claude Skills** உடன் கோடிங் ஏஜென்ட்டுகளை இயக்குவதற்கும் நிர்வகிப்பதற்கும் ஒரு ஓப்பன் சோர்ஸ் தளம். 🤖

எக்ஸ் (X)-இல் என்னைப் பின்தொடரவும்: [https://x.com/jiayuan_jy](https://x.com/jiayuan_jy) 🐦

---

[English](../README.md) | [简体中文](./README_ZH.md) | [हिन्दी](./README_HI.md) | [বাংলা](./README_BN.md) | [मराठी](./README_MR.md) | [తెలుగు](./README_TE.md) | தமிழ் | [ગુજરાતી](./README_GU.md) | [اردو](./README_UR.md) | [ಕನ್ನಡ](./README_KN.md)

---

## 🌟 மேலோட்டம் (Overview)

Claude Code-இன் நடத்தையை மேம்படுத்தவும், பொதுவான LLM கோடிங் பிழைகளைக் குறைக்கவும் வடிவமைக்கப்பட்ட **மாடுலர், பிரீமியம் கிளாட் திறன்களின் (Claude Skills)** தொகுப்பு. இந்த கொள்கைகள் AI கோடிங் குறைபாடுகள் குறித்த [ஆண்ட்ரே கார்பதியின் அவதானிப்புகளிலிருந்து](https://x.com/karpathy/status/2015883857489522876) பெறப்பட்டவை.

---

## ⚠️ சிக்கல்கள் (The Problems)

AI மாதிரிகள் பெரும்பாலும்:
1.  ❌ சரிபார்க்காமல் **தவறான அனுமானங்களை** செய்கின்றன.
2.  ❌ குறியீடு மற்றும் API-களைத் தேவையில்லாமல் சிக்கலாக்குகின்றன.
3.  ❌ தங்களுக்குப் புரியாத குறியீடு அல்லது கருத்துகளை (comments) நீக்குகின்றன.
4.  ❌ சிக்கலான பணிகளுக்குத் தெளிவான வெற்றிக் அளவுகோல்கள் இல்லை.

---

## 🛡️ தீர்வு: பிரீமியம் கிளாட் திறன்கள் (Claude Skills)

இந்த மாடுலர் **Claude Skills** நேரடியாக மேலே உள்ள சிக்கல்களைத் தீர்க்கின்றன:

| திறன் (Skill) | விளக்கம் (Description) | தீர்க்கும் சிக்கல்கள் (Addresses) |
| :--- | :--- | :--- |
| 🧠 **கோடிங் செய்யும் முன் சிந்திப்போம்** | தெளிவான பகுத்தறிவு மற்றும் அனுமானங்களை வெளிக்கொணரச் செய்கிறது. | மறைந்திருக்கும் குழப்பம், தவறான அனுமானங்கள். |
| 🍃 **எளிமைக்கே முதலிடம்** | சிக்கலைத் தீர்க்கத் தேவையான குறைந்தபட்ச குறியீடு. ஊகங்கள் வேண்டாம். | அதிகப்படியான சிக்கல், தேவையற்ற அப்ஸ்ட்ராக்ஷன்கள் (abstractions). |
| 🎯 **துல்லியமான மாற்றங்கள்** | தேவையானது மட்டும் மாற்றவும். ஏற்கனவே உள்ள பாணியைப் பின்பற்றவும். | தேவையற்ற மாற்றங்கள், பாணி மாற்றம். |
| ✅ **இலக்கு சார்ந்த செயல்பாடு** | வெற்றிக்கான அளவுகோல்களை வரையறுத்து, சரிபார்க்கப்படும் வரை தொடரவும். | இம்பரேட்டிவ் (Imperative) மற்றும் டிக்லரேட்டிவ் (Declarative) இடைவெளிகள். |

---

## 📦 மாடுலர் கிளாட் திறன்கள் விரிவாக

### 1. கோடிங் செய்யும் முன் சிந்திப்போம் (Think Before Coding)
**அனுமானிக்காதீர்கள். குழப்பத்தை மறைக்காதீர்கள். வர்த்தக பரிமாற்றங்களை (tradeoffs) வெளிப்படுத்துங்கள்.**
இந்தத் திறன் உங்கள் AI கூட்டாளர் ஒரு வரி குறியீட்டைத் தொடுவதற்கு முன்பே தெளிவாகப் பகுத்தறிவதை உறுதி செய்கிறது.

### 2. எளிமைக்கே முதலிடம் (Simplicity First)
**சிக்கலைத் தீர்க்கும் குறைந்தபட்ச குறியீடு. ஊகங்கள் எதுவுமில்லை.**
அதிகப்படியான பொறியியல் (over-engineering) போக்கை எதிர்க்கவும். 200 வரிகள் கொண்ட குறியீட்டை 50 வரிகளில் செய்ய முடிந்தால், அதை மீண்டும் எழுதுங்கள்.

### 3. துல்லியமான மாற்றங்கள் (Surgical Changes)
**தொட வேண்டியதை மட்டும் தொடவும். உங்கள் மாற்றங்களால் ஏற்பட்ட குழப்பத்தை மட்டும் சரிசெய்யவும்.**
துல்லியமான மாற்றங்களில் கவனம் செலுத்துங்கள். நீங்கள் வேறுவிதமாகச் செய்ய விரும்பினாலும், திட்டத்தின் தற்போதைய பாணியுடன் ஒத்துப்போங்கள்.

### 4. இலக்கு சார்ந்த செயல்பாடு (Goal-Driven Execution)
**வெற்றிக்கான அளவுகோல்களை வரையறுக்கவும். சரிபார்க்கப்படும் வரை தொடரவும்.**
தெளிவற்ற பணிகளை குறிப்பிட்ட வெற்றி அளவீடுகளுடன் சரிபார்க்கக்கூடிய இலக்குகளாக மாற்றவும்.

---

## 🚀 நிறுவுதல் (Installation)

### விருப்பம் A: Claude Code செருகுநிரல் (பரிந்துரைக்கப்படுகிறது)

சந்தைப்பகுதியை (marketplace) சேர்த்து **Claude Skills**-ஐ நிறுவவும்:

```bash
/plugin marketplace add forrestchang/claude-skills-by-karpathy
/plugin install claude-skills-by-karpathy@karpathy-skills
```

### விருப்பம் B: CLAUDE.md (ஒவ்வொரு திட்டத்திற்கும்)

```bash
curl -o CLAUDE.md https://raw.githubusercontent.com/forrestchang/claude-skills-by-karpathy/main/CLAUDE.md
```

---

## 🛠️ கருவி ஆதரவு (Tool Support)

*   **Cursor**: எங்கள் திட்ட விதிகளைப் பயன்படுத்தி இந்தத் திறன்களைத் தானாகவே பயன்படுத்துங்கள். **[docs/cursor-setup.md](../docs/cursor-setup.md)** பார்க்கவும்.
*   **உதாரணங்கள்**: **[docs/examples.md](../docs/examples.md)** இல் நிஜ உலக மாற்றங்களைப் பார்க்கவும்.

---

## 🤝 பங்களிப்பு (Contributing)

பங்களிப்புகள் வரவேற்கப்படுகின்றன! உங்களிடம் புதிய **Claude Skill** அல்லது ஏற்கனவே உள்ளவற்றில் மேம்பாடு இருந்தால், தயவுசெய்து ஒரு PR-ஐத் திறக்கவும்.

## 📄 உரிமம் (License)

MIT © [forrestchang](https://github.com/forrestchang)

## 📈 ஸ்டார் வரலாறு (Star History)
<div align="center">
   <a href="https://www.star-history.com/repos=ishandutta2007%2Fclaude-skills-by-karpathy&type=date&legend=bottom-right">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/chart?repos=ishandutta2007/claude-skills-by-karpathy&type=date&theme=dark&legend=bottom-right" />
      <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/chart?repos=ishandutta2007/claude-skills-by-karpathy&type=date&legend=bottom-right" />
      <img alt="Star History Chart" src="https://api.star-history.com/chart?repos=ishandutta2007/claude-skills-by-karpathy&type=date&legend=bottom-right" />
    </picture>
   </a>
</div>
