<p align="center">
  <img src="../assets/banner.svg" alt="Karpathy-Inspired Claude Skills Banner" width="100%">
</p>

# কার্প্যাথি-অনুপ্রাণিত ক্লড স্কিলস (Claude Skills) 🚀

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Version](https://img.shields.io/badge/version-1.1.0-blue.svg)](https://github.com/forrestchang/claude-skills-by-karpathy)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://makeapullrequest.com)
<a href="https://github.com/ishandutta2007"><img alt="GitHub followers" src="https://img.shields.io/github/followers/ishandutta2007?label=Follow&style=social" /></a>

> **SEO কীওয়ার্ড**: Claude Skills, AI Coding Best Practices, Karpathy Guidelines, Claude Code Plugin, Cursor Rules, LLM Coding Pitfalls, Sustainable AI Engineering.

আমার নতুন প্রজেক্ট [Multica](https://github.com/multica-ai/multica) দেখুন — পুনরায় ব্যবহারযোগ্য (reusable) **Claude Skills** সহ কোডিং এজেন্ট চালানোর এবং পরিচালনা করার জন্য একটি ওপেন-সোর্স প্ল্যাটফর্ম। 🤖

আমাকে X-এ ফলো করুন: [https://x.com/jiayuan_jy](https://x.com/jiayuan_jy) 🐦

---

[English](../README.md) | [简体中文](./README_ZH.md) | [हिन्दी](./README_HI.md) | বাংলা | [मराठी](./README_MR.md) | [తెలుగు](./README_TE.md) | [தமிழ்](./README_TA.md) | [ગુજરાતી](./README_GU.md) | [اردو](./README_UR.md) | [ಕನ್ನಡ](./README_KN.md)

---

## 🌟 ওভারভিউ (Overview)

Claude Code-এর আচরণ উন্নত করতে এবং সাধারণ LLM কোডিং ভুলগুলো কমাতে ডিজাইন করা **মডুলার, প্রিমিয়াম ক্লড স্কিলস (Claude Skills)**-এর একটি সংগ্রহ। এই নীতিগুলো AI কোডিং-এর ত্রুটি নিয়ে [আন্দ্রে কার্প্যাথির পর্যবেক্ষণ](https://x.com/karpathy/status/2015883857489522876) থেকে নেওয়া হয়েছে।

---

## ⚠️ সমস্যাগুলো (The Problems)

AI মডেলগুলো প্রায়ই:
1.  ❌ যাচাই না করেই **ভুল ধারণা** তৈরি করে।
2.  ❌ কোড এবং API-কে অতিরিক্ত জটিল করে তোলে।
3.  ❌ এমন কোড বা কমেন্ট সরিয়ে দেয় যা তারা বুঝতে পারে না।
4.  ❌ জটিল কাজের জন্য সাফল্যের স্পষ্ট মানদণ্ডের অভাব থাকে।

---

## 🛡️ সমাধান: প্রিমিয়াম ক্লড স্কিলস (Claude Skills)

এই মডুলার **Claude Skills** সরাসরি উপরের সমস্যাগুলোর সমাধান করে:

| স্কিল (Skill) | বর্ণনা (Description) | যা সমাধান করে (Addresses) |
| :--- | :--- | :--- |
| 🧠 **কোডিংয়ের আগে চিন্তা করুন** | স্পষ্ট যুক্তি এবং ধারণাগুলো সামনে আনতে বাধ্য করে। | লুকানো বিভ্রান্তি, ভুল ধারণা। |
| 🍃 **সরলতা সবার আগে** | সমস্যা সমাধানের জন্য ন্যূনতম কোড। কোনো অনুমান নয়। | অতিরিক্ত জটিলতা, ভারী অ্যাবস্ট্রাকশন। |
| 🎯 **সুনির্দিষ্ট পরিবর্তন** | শুধুমাত্র যা প্রয়োজন তা স্পর্শ করুন। বিদ্যমান শৈলী বজায় রাখুন। | অপ্রাসঙ্গিক সম্পাদনা, শৈলী পরিবর্তন। |
| ✅ **লক্ষ্য-চালিত সম্পাদন** | সাফল্যের মানদণ্ড নির্ধারণ করুন এবং যাচাই না হওয়া পর্যন্ত লুপ করুন। | ইম্পারেটিভ (Imperative) বনাম ডিক্লারেটিভ (Declarative) ব্যবধান। |

---

## 📦 মডুলার ক্লড স্কিলস বিস্তারিত

### ১. কোডিংয়ের আগে চিন্তা করুন (Think Before Coding)
**ধারণা করবেন না। বিভ্রান্তি লুকাবেন না। ট্রেড-অফগুলো সামনে আনুন।**
এই স্কিলটি নিশ্চিত করে যে আপনার AI পার্টনার কোডের একটি লাইনও স্পর্শ করার আগে স্পষ্টভাবে যুক্তি দেয়।

### ২. সরলতা সবার আগে (Simplicity First)
**ন্যূনতম কোড যা সমস্যার সমাধান করে। অনুমানমূলক কিছু নয়।**
ওভার-ইঞ্জিনিয়ারিংয়ের প্রবণতার বিরুদ্ধে লড়াই করুন। যদি ২০০ লাইন কোড ৫০ লাইনে করা সম্ভব হয়, তবে তা আবার লিখুন।

### ৩. সুনির্দিষ্ট পরিবর্তন (Surgical Changes)
**শুধুমাত্র যা প্রয়োজন তা স্পর্শ করুন। শুধুমাত্র আপনার তৈরি করা অগোছালো অংশ পরিষ্কার করুন।**
সুনির্দিষ্ট সম্পাদনার দিকে মনোযোগ দিন। প্রজেক্টের বিদ্যমান শৈলী বজায় রাখুন, এমনকি যদি আপনি এটি অন্যভাবে করতে পছন্দ করেন তবুও।

### ৪. লক্ষ্য-চালিত সম্পাদন (Goal-Driven Execution)
**সাফল্যের মানদণ্ড নির্ধারণ করুন। যাচাই না হওয়া পর্যন্ত লুপ করুন।**
অস্পষ্ট কাজগুলোকে সুনির্দিষ্ট সাফল্যের মেট্রিক্স সহ যাচাইযোগ্য লক্ষ্যে রূপান্তর করুন।

---

## 🚀 ইনস্টলেশন (Installation)

### অপশন A: Claude Code প্লাগইন (প্রস্তাবিত)

মার্কেটপ্লেস যোগ করুন এবং **Claude Skills** ইনস্টল করুন:

```bash
/plugin marketplace add forrestchang/claude-skills-by-karpathy
/plugin install claude-skills-by-karpathy@karpathy-skills
```

### অপশন B: CLAUDE.md (প্রতি প্রজেক্টে)

```bash
curl -o CLAUDE.md https://raw.githubusercontent.com/forrestchang/claude-skills-by-karpathy/main/CLAUDE.md
```

---

## 🛠️ টুল সাপোর্ট (Tool Support)

*   **Cursor**: আমাদের প্রজেক্টের নিয়মগুলো ব্যবহার করে স্বয়ংক্রিয়ভাবে এই স্কিলগুলো প্রয়োগ করুন। **[docs/cursor-setup.md](../docs/cursor-setup.md)** দেখুন।
*   **উদাহরণ**: **[docs/examples.md](../docs/examples.md)**-এ বাস্তব জগতের রূপান্তরগুলো দেখুন।

---

## 🤝 অবদান (Contributing)

অবদানকে স্বাগত জানানো হয়! আপনার যদি নতুন কোনো **Claude Skill** থাকে বা বিদ্যমানগুলোর কোনো উন্নতি থাকে, তবে অনুগ্রহ করে একটি PR খুলুন।

## 📄 লাইসেন্স (License)

MIT © [forrestchang](https://github.com/forrestchang)

## 📈 স্টার হিস্ট্রি (Star History)
<div align="center">
   <a href="https://www.star-history.com/repos=ishandutta2007%2Fclaude-skills-by-karpathy&type=date&legend=bottom-right">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/chart?repos=ishandutta2007/claude-skills-by-karpathy&type=date&theme=dark&legend=bottom-right" />
      <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/chart?repos=ishandutta2007/claude-skills-by-karpathy&type=date&legend=bottom-right" />
      <img alt="Star History Chart" src="https://api.star-history.com/chart?repos=ishandutta2007/claude-skills-by-karpathy&type=date&legend=bottom-right" />
    </picture>
   </a>
</div>
