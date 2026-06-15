---
title_he: "סוכן קוד חינמי בטרמינל עם Nemotron 3 Ultra של NVIDIA דרך OpenRouter"
title_en: "Free Frontier Coding Agent in Terminal: NVIDIA Nemotron 3 Ultra via OpenRouter + OpenCode"
source: "https://www.instagram.com/reel/DZhwQM7qYIB/?igsh=MXNnN2poNnMxNXYz"
creator: "@Build With AI"
platform: "instagram"
category: "optiplan"
relevance: 4
date_processed: "2026-06-15"
tags: ["coding-agent", "open-source", "nvidia", "terminal", "openrouter", "free-model"]
---

## תקציר

הסרטון מציג שילוב בין OpenCode (סוכן קוד open-source שרץ בטרמינל) לבין Nemotron 3 Ultra של NVIDIA — מודל MoE בעל 550B פרמטרים עם חלון הקשר של מיליון טוקן, זמין בחינם דרך OpenRouter. ההגדרה פשוטה: התקנת OpenCode, פתיחת חשבון OpenRouter חינמי, חיבור המפתח דרך /connect ובחירת המודל דרך /models. ניתן גם לנסות את המודל ישירות בדפדפן ב-build.nvidia.com.

## תובנות מפתח

- Nemotron 3 Ultra הוא MoE (Mixture-of-Experts) — 550B פרמטרים סה"כ אך רק ~55B פעילים לכל טוקן, מה שמאפשר מהירות של 300+ טוקנים/שנייה — פי 2.5-4 מהר יותר מ-GPT-5
- OpenCode הוא כלי provider-agnostic: ניתן לחבר אליו Claude, OpenAI, Gemini, OpenRouter, מודלים מקומיים דרך Ollama — גמישות מלאה ללא נעילת ספק
- חלון הקשר של מיליון טוקן מאפשר לקרוא codebase שלם — רלוונטי מאוד לפרויקט OptiPlan עם NX monorepo גדול
- OpenCode תומך ב-Plan mode (Tab) לסקירת תוכנית לפני ביצוע שינויים — בטיחות חשובה בעבודה על codebase ייצורי
- רלוונטי גם לפרויקט taylor-played: OpenCode תומך ב-Gemini ו-Firebase workflows, וניתן לחבר אותו לכל מודל בחינם

## כלים וספריות

| שם | קישור | תיאור |
|---|---|---|
| [NVIDIA Nemotron 3 Ultra](https://build.nvidia.com/nvidia/nemotron-3-ultra) | https://build.nvidia.com/nvidia/nemotron-3-ultra | מודל שפה open-weight של NVIDIA, 550B פרמטרים (MoE, 55B פעילים), חלון הקשר 1M טוקן, מהיר במיוחד לסוכנים |
| [OpenCode](https://opencode.ai) | https://opencode.ai | סוכן קוד open-source שרץ בטרמינל, תומך ב-75+ ספקי מודלים, כולל LSP integration ו-Plan/Build modes |
| [OpenRouter](https://openrouter.ai) | https://openrouter.ai | שער API מאוחד לגישה למאות מודלים כולל Nemotron Ultra — מאפשר גישה חינמית למודלים נבחרים |
| [NVIDIA NIM (build.nvidia.com)](https://build.nvidia.com) | https://build.nvidia.com | פלטפורמת הדגמה ו-inference חינמית של NVIDIA בדפדפן לניסיון מודלים ללא הגדרה |

## ריפוזיטוריז

- https://github.com/sst/opencode

## פריטי פעולה

- [ ] התקן OpenCode בטרמינל: curl -fsSL https://opencode.ai/install | bash (או npm i -g opencode-ai@latest)
- [ ] פתח חשבון חינמי ב-OpenRouter בכתובת openrouter.ai, צור API key
- [ ] בתוך פרויקט OptiPlan, הפעל opencode ואז /connect ← בחר OpenRouter ← הדבק מפתח
- [ ] בצע /models וחפש 'Nemotron 3 Ultra' עם תג free לבדיקת זמינות החינמיות
- [ ] השתמש ב-Plan mode (Tab) לפני כל שינוי בקוד ייצורי ב-OptiPlan
- [ ] נסה את המודל תחילה בדפדפן ב-build.nvidia.com לפני הגדרת כלי

## הערות אימות

- ⚠️ הטענה '550 billion parameters' — נכון אך מטעה: מדובר במודל MoE עם 55B פרמטרים פעילים בלבד לכל טוקן, לא 550B פעילים
- ⚠️ הטענה 'beats most of them' — מוגזמת: Nemotron Ultra מוביל בין מודלי open-weight אמריקאיים אך נופל מ-Kimi K2.6 הסיני ב-6 נקודות על מדד Intelligence Index
- ⚠️ זמינות חינמית ב-OpenRouter — יש לאמת: נכון למועד פרסום הסרטון, התמחור ב-OpenRouter לא היה מתועד בצורה ציבורית. ייתכן שה-free tier מוגבל או השתנה
- ⚠️ הפקודה '/connect' — יש לאמת בגרסת OpenCode העדכנית (הכלי מתעדכן מהר)

