<p align="center">
  <img src="../assets/banner.svg" alt="Karpathy-Inspired Claude Skills Banner" width="100%">
</p>

# کارپیتھی سے متاثر کلاڈ اسکلز (Claude Skills) 🚀

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Version](https://img.shields.io/badge/version-1.1.0-blue.svg)](https://github.com/forrestchang/claude-skills-by-karpathy)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://makeapullrequest.com)
<a href="https://github.com/ishandutta2007"><img alt="GitHub followers" src="https://img.shields.io/github/followers/ishandutta2007?label=Follow&style=social" /></a>

> **SEO کلیدی الفاظ**: Claude Skills, AI Coding Best Practices, Karpathy Guidelines, Claude Code Plugin, Cursor Rules, LLM Coding Pitfalls, Sustainable AI Engineering.

میرا نیا پروجیکٹ [Multica](https://github.com/multica-ai/multica) دیکھیں — دوبارہ استعمال کے قابل (reusable) **Claude Skills** کے ساتھ کوڈنگ ایجنٹس کو چلانے اور ان کے انتظام کے لیے ایک اوپن سورس پلیٹ فارم۔ 🤖

مجھے X پر فالو کریں: [https://x.com/jiayuan_jy](https://x.com/jiayuan_jy) 🐦

---

[English](../README.md) | [简体中文](./README_ZH.md) | [हिन्दी](./README_HI.md) | [বাংলা](./README_BN.md) | [मराठी](./README_MR.md) | [తెలుగు](./README_TE.md) | [தமிழ்](./README_TA.md) | [ગુજરાતી](./README_GU.md) | اردو | [ಕನ್ನಡ](./README_KN.md)

---

## 🌟 جائزہ (Overview)

Claude Code کے طرز عمل کو بہتر بنانے اور عام LLM کوڈنگ کی غلطیوں کو کم کرنے کے لیے ڈیزائن کیے گئے **ماڈیولر، پریمیم کلاڈ اسکلز (Claude Skills)** کا مجموعہ۔ یہ اصول AI کوڈنگ کی خامیوں پر [آندرے کارپیتھی کے مشاہدات](https://x.com/karpathy/status/2015883857489522876) سے لیے گئے ہیں۔

---

## ⚠️ مسائل (The Problems)

AI ماڈلز اکثر:
1.  ❌ بغیر چیک کیے **غلط مفروضے** بنا لیتے ہیں۔
2.  ❌ کوڈ اور API کو بلا ضرورت پیچیدہ بنا دیتے ہیں۔
3.  ❌ اس کوڈ یا تبصروں کو ہٹا دیتے ہیں جنہیں وہ سمجھ نہیں پاتے۔
4.  ❌ پیچیدہ کاموں کے لیے کامیابی کے واضح معیار کی کمی ہوتی ہے۔

---

## 🛡️ حل: پریمیم کلاڈ اسکلز (Claude Skills)

یہ ماڈیولر **Claude Skills** براہ راست اوپر دیے گئے مسائل کو حل کرتی ہیں:

| اسکل (Skill) | تفصیل (Description) | حل (Addresses) |
| :--- | :--- | :--- |
| 🧠 **کوڈنگ سے پہلے سوچیں** | واضح استدلال اور مفروضوں کو سامنے لانے پر مجبور کرتا ہے۔ | پوشیدہ الجھن، غلط مفروضے۔ |
| 🍃 **سادگی سب سے پہلے** | مسئلہ حل کرنے کے لیے کم سے کم کوڈ۔ کوئی قیاس آرائی نہیں۔ | ضرورت سے زیادہ پیچیدگی، بھاری تجرید (abstractions)۔ |
| 🎯 **درست تبدیلیاں** | صرف وہی چھوئیں جو ضروری ہے۔ موجودہ انداز (style) کی پیروی کریں۔ | غیر متعلقہ ترامیم، اسٹائل میں تبدیلی۔ |
| ✅ **مقصد پر مبنی نفاذ** | کامیابی کے معیار کی وضاحت کریں اور تصدیق ہونے تک لوپ کریں۔ | حکمیہ (Imperative) بمقابلہ بیانیہ (Declarative) فرق۔ |

---

## 📦 ماڈیولر کلاڈ اسکلز تفصیل سے

### 1. کوڈنگ سے پہلے سوچیں (Think Before Coding)
**مفروضے نہ بنائیں۔ الجھن نہ چھپائیں۔ تجاویز (tradeoffs) سامنے لائیں۔**
یہ اسکل اس بات کو یقینی بناتی ہے کہ آپ کا AI پارٹنر کوڈ کی ایک لائن کو چھونے سے پہلے واضح طور پر استدلال کرے۔

### 2. سادگی سب سے پہلے (Simplicity First)
**کم سے کم کوڈ جو مسئلہ حل کرے۔ کچھ بھی قیاس آرائی پر مبنی نہیں۔**
اوور انجینئرنگ کے رجحان کے خلاف لڑیں۔ اگر 200 لائنوں کا کام 50 لائنوں میں ہو سکتا ہے تو اسے دوبارہ لکھیں۔

### 3. درست تبدیلیاں (Surgical Changes)
**صرف وہی چھوئیں جو آپ کو چھونا چاہیے۔ صرف اپنی بنائی ہوئی گندگی صاف کریں۔**
درست ترمیم پر توجہ دیں۔ پروجیکٹ کے موجودہ اسٹائل سے مطابقت رکھیں، چاہے آپ اسے مختلف طریقے سے کرنا پسند کریں۔

### 4. مقصد پر مبنی نفاذ (Goal-Driven Execution)
**کامیابی کے معیار کی وضاحت کریں۔ تصدیق ہونے تک لوپ کریں۔**
مبہم کاموں کو مخصوص کامیابی کے میٹرکس کے ساتھ قابل تصدیق اہداف میں تبدیل کریں۔

---

## 🚀 انسٹالیشن (Installation)

### آپشن A: Claude Code پلگ ان (تجویز کردہ)

مارکیٹ پلیس شامل کریں اور **Claude Skills** انسٹال کریں:

```bash
/plugin marketplace add forrestchang/claude-skills-by-karpathy
/plugin install claude-skills-by-karpathy@karpathy-skills
```

### آپشن B: CLAUDE.md (فی پروجیکٹ)

```bash
curl -o CLAUDE.md https://raw.githubusercontent.com/forrestchang/claude-skills-by-karpathy/main/CLAUDE.md
```

---

## 🛠️ ٹول سپورٹ (Tool Support)

*   **Cursor**: ہمارے پروجیکٹ کے قوانین کا استعمال کرتے ہوئے ان اسکلز کو خودکار طور پر لاگو کریں۔ **[docs/cursor-setup.md](../docs/cursor-setup.md)** دیکھیں۔
*   **مثالیں**: **[docs/examples.md](../docs/examples.md)** میں حقیقی دنیا کی تبدیلیاں دیکھیں۔

---

## 🤝 تعاون (Contributing)

تعاون کا خیرمقدم ہے! اگر آپ کے پاس نئی **Claude Skill** ہے یا موجودہ اسکلز میں بہتری ہے تو براہ کرم ایک PR کھولیں۔

## 📄 لائسنس (License)

MIT © [forrestchang](https://github.com/forrestchang)

## 📈 اسٹار ہسٹری (Star History)
<div align="center">
   <a href="https://www.star-history.com/repos=ishandutta2007%2Fclaude-skills-by-karpathy&type=date&legend=bottom-right">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/chart?repos=ishandutta2007/claude-skills-by-karpathy&type=date&theme=dark&legend=bottom-right" />
      <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/chart?repos=ishandutta2007/claude-skills-by-karpathy&type=date&legend=bottom-right" />
      <img alt="Star History Chart" src="https://api.star-history.com/chart?repos=ishandutta2007/claude-skills-by-karpathy&type=date&legend=bottom-right" />
    </picture>
   </a>
</div>
