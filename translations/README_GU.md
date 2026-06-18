<p align="center">
  <img src="../assets/banner.svg" alt="Karpathy-Inspired Claude Skills Banner" width="100%">
</p>

# કાર્પાથી-પ્રેરિત ક્લોડ સ્કીલ્સ (Claude Skills) 🚀

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Version](https://img.shields.io/badge/version-1.1.0-blue.svg)](https://github.com/forrestchang/claude-skills-by-karpathy)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://makeapullrequest.com)
<a href="https://github.com/ishandutta2007"><img alt="GitHub followers" src="https://img.shields.io/github/followers/ishandutta2007?label=Follow&style=social" /></a>

> **SEO કીવર્ડ્સ**: Claude Skills, AI Coding Best Practices, Karpathy Guidelines, Claude Code Plugin, Cursor Rules, LLM Coding Pitfalls, Sustainable AI Engineering.

મારો નવો પ્રોજેક્ટ [Multica](https://github.com/multica-ai/multica) જુઓ — પુનઃઉપયોગ કરી શકાય તેવા (reusable) **Claude Skills** સાથે કોડિંગ એજન્ટ્સ ચલાવવા અને સંચાલિત કરવા માટેનું એક ઓપન-સોર્સ પ્લેટફોર્મ. 🤖

મને X પર ફોલો કરો: [https://x.com/jiayuan_jy](https://x.com/jiayuan_jy) 🐦

---

[English](../README.md) | [简体中文](./README_ZH.md) | [हिन्दी](./README_HI.md) | [বাংলা](./README_BN.md) | [मराठी](./README_MR.md) | [తెలుగు](./README_TE.md) | [தமிழ்](./README_TA.md) | ગુજરાતી | [اردو](./README_UR.md) | [ಕನ್ನಡ](./README_KN.md)

---

## 🌟 ઝાંખી (Overview)

Claude Code ના વર્તનમાં સુધારો કરવા અને સામાન્ય LLM કોડિંગ ભૂલો ઘટાડવા માટે રચાયેલ **મોડ્યુલર, પ્રીમિયમ ક્લોડ સ્કીલ્સ (Claude Skills)** નો સંગ્રહ. આ સિદ્ધાંતો AI કોડિંગની ખામીઓ પર [આન્દ્રે કાર્પાથીના અવલોકનો](https://x.com/karpathy/status/2015883857489522876) માંથી લેવામાં આવ્યા છે.

---

## ⚠️ સમસ્યાઓ (The Problems)

AI મોડલ્સ ઘણીવાર:
1.  ❌ તપાસ કર્યા વિના **ખોટી ધારણાઓ** બાંધે છે.
2.  ❌ કોડ અને API ને બિનજરૂરી રીતે જટિલ બનાવે છે.
3.  ❌ તે કોડ કે કોમેન્ટ્સ હટાવી દે છે જે તેઓ સમજી શકતા નથી.
4.  ❌ જટિલ કાર્યો માટે સફળતાના સ્પષ્ટ માપદંડોનો અભાવ હોય છે.

---

## 🛡️ ઉકેલ: પ્રીમિયમ ક્લોડ સ્કીલ્સ (Claude Skills)

આ મોડ્યુલર **Claude Skills** સીધી રીતે ઉપરની સમસ્યાઓનું નિરાકરણ લાવે છે:

| સ્કીલ (Skill) | વર્ણન (Description) | ઉકેલ (Addresses) |
| :--- | :--- | :--- |
| 🧠 **કોડિંગ કરતા પહેલા વિચારો** | સ્પષ્ટ તર્ક અને ધારણાઓને સપાટી પર લાવવા માટે દબાણ કરે છે. | છુપાયેલી મૂંઝવણ, ખોટી ધારણાઓ. |
| 🍃 **સરળતા પ્રથમ** | સમસ્યા હલ કરવા માટે ન્યૂનતમ કોડ. કોઈ અટકળો નહીં. | અતિ-જટિલતા, ફૂલેલા એબ્સ્ટ્રેક્શન્સ. |
| 🎯 **સચોટ ફેરફારો** | ફક્ત જે જરૂરી હોય તેને જ સ્પર્શ કરો. હાલની શૈલીને અનુસરો. | અસંબંધિત સંપાદન, શૈલીમાં ફેરફાર. |
| ✅ **ધ્યેય-સંચાલિત અમલીકરણ** | સફળતાના માપદંડો વ્યાખ્યાયિત કરો અને ચકાસણી ન થાય ત્યાં સુધી લૂપ કરો. | ઇમ્પેરેટિવ (Imperative) વિરુદ્ધ ડિક્લરેટિવ (Declarative) અંતર. |

---

## 📦 મોડ્યુલર ક્લોડ સ્કીલ્સ વિગતવાર

### 1. કોડિંગ કરતા પહેલા વિચારો (Think Before Coding)
**ધારણાઓ બાંધશો નહીં. મૂંઝવણ છુપાવશો નહીં. ટ્રેડ-ઓફ્સ સપાટી પર લાવો.**
આ સ્કીલ એ સુનિશ્ચિત કરે છે કે તમારો AI પાર્ટનર કોડની એક પણ લાઇનને સ્પર્શ કરતા પહેલા સ્પષ્ટપણે તર્ક આપે.

### 2. સરળતા પ્રથમ (Simplicity First)
**ન્યૂનતમ કોડ જે સમસ્યાનું નિરાકરણ લાવે છે. કંઈપણ કાલ્પનિક નહીં.**
ઓવર-એન્જિનિયરિંગની વૃત્તિ સામે લડો. જો 200 લાઇનનો કોડ 50 લાઇનમાં થઈ શકતો હોય, તો તેને ફરીથી લખો.

### 3. સચોટ ફેરફારો (Surgical Changes)
**ફક્ત જે તમારે સ્પર્શવું જોઈએ તેને જ સ્પર્શ કરો. ફક્ત તમારી બનાવેલી ગંદકી સાફ કરો.**
ચોક્કસ સંપાદન પર ધ્યાન કેન્દ્રિત કરો. પ્રોજેક્ટની હાલની શૈલી સાથે મેળ મેળવો, ભલે તમે તેને અલગ રીતે કરવા માંગતા હોવ.

### 4. ધ્યેય-સંચાલિત અમલીકરણ (Goal-Driven Execution)
**સફળતાના માપદંડો વ્યાખ્યાયિત કરો. ચકાસણી ન થાય ત્યાં સુધી લૂપ કરો.**
અસ્પષ્ટ કાર્યોને વિશિષ્ટ સફળતા મેટ્રિક્સ સાથે ચકાસી શકાય તેવા લક્ષ્યોમાં રૂપાંતરિત કરો.

---

## 🚀 ઇન્સ્ટોલેશન (Installation)

### વિકલ્પ A: Claude Code પ્લગઈન (ભલામણ કરેલ)

માર્કેટપ્લેસ ઉમેરો અને **Claude Skills** ઇન્સ્ટોલ કરો:

```bash
/plugin marketplace add forrestchang/claude-skills-by-karpathy
/plugin install claude-skills-by-karpathy@karpathy-skills
```

### વિકલ્પ B: CLAUDE.md (પ્રોજેક્ટ દીઠ)

```bash
curl -o CLAUDE.md https://raw.githubusercontent.com/forrestchang/claude-skills-by-karpathy/main/CLAUDE.md
```

---

## 🛠️ ટૂલ સપોર્ટ (Tool Support)

*   **Cursor**: અમારા પ્રોજેક્ટ નિયમોનો ઉપયોગ કરીને આ સ્કીલ્સ આપમેળે લાગુ કરો. **[docs/cursor-setup.md](../docs/cursor-setup.md)** જુઓ.
*   **ઉદાહરણો**: **[docs/examples.md](../docs/examples.md)** માં વાસ્તવિક દુનિયાના પરિવર્તનો જુઓ.

---

## 🤝 યોગદાન (Contributing)

યોગદાન આવકાર્ય છે! જો તમારી પાસે નવી **Claude Skill** હોય અથવા હાલની સ્કીલ્સમાં સુધારો હોય, તો કૃપા કરીને PR ખોલો.

## 📄 લાઇસન્સ (License)

MIT © [forrestchang](https://github.com/forrestchang)

## 📈 સ્ટાર હિસ્ટ્રી (Star History)
<div align="center">
   <a href="https://www.star-history.com/repos=ishandutta2007%2Fclaude-skills-by-karpathy&type=date&legend=bottom-right">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/chart?repos=ishandutta2007/claude-skills-by-karpathy&type=date&theme=dark&legend=bottom-right" />
      <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/chart?repos=ishandutta2007/claude-skills-by-karpathy&type=date&legend=bottom-right" />
      <img alt="Star History Chart" src="https://api.star-history.com/chart?repos=ishandutta2007/claude-skills-by-karpathy&type=date&legend=bottom-right" />
    </picture>
   </a>
</div>
