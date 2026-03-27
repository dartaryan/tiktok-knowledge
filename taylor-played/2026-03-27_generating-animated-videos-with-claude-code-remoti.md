---
title_he: "יצירת סרטוני אנימציה עם Claude Code ו-Remotion — ללא תוכנות עריכה"
title_en: "Generating Animated Videos with Claude Code + Remotion Agent Skill — No Editing Software Needed"
source: "https://vt.tiktok.com/ZSuosm8xj"
creator: "@jagger_b"
category: "taylor-played"
relevance: 3
date_processed: "2026-03-27"
tags: ["claude-code", "remotion", "react", "video-generation", "content-creation", "ai-tools"]
---

## תקציר

ניתן להתקין את ה-Skill של Remotion (ספריית React ליצירת וידאו תכנותי) בתוך Claude Code ולייצר סרטוני אנימציה מלאים באמצעות פרומפטים בלבד. Claude מייצר scenes, תזמון ואסטים, והתוצאה מוצגת אוטומטית ב-Remotion Studio בדפדפן לעריכה. שימושים מוצהרים: טיזרי מוצר, תוכן TikTok ו-Reels, סרטוני הסבר ודמואים פנים-ארגוניים.

## תובנות מפתח

- Remotion בנוי על React — מה שהופך אותו לתואם ישירות לסטאק של taylor-played (React 19 + TypeScript), ומאפשר שילוב עם קוד קיים
- ה-Skill מלמד את Claude Code את ה-API של Remotion, דפוסי אנימציה ו-best practices — אין צורך בהיכרות מוקדמת עם הספרייה
- שלא כמו AI וידאו גנרטיבי (כמו Sora), Remotion מייצר React components שרנדרים פריימים — התוצאה ניתנת לעריכה, לאיטרציה ולשליטה מלאה
- שימוש מסחרי ב-Remotion עשוי לדרוש רישיון חברה בתשלום — חובה לבדוק לפני שימוש בפרויקט taylor-played
- רלוונטי גם ל-shalhevet (יצירת סרטוני הסבר לסדנאות) ול-elon-katzef (דמואים פנים-ארגוניים) — אך taylor-played הוא ה-fit הטוב ביותר לצרכי שיווק מוצר פיזי

## כלים וספריות

| שם | קישור | תיאור |
|---|---|---|
| [Claude Code](https://claude.ai/code) | https://claude.ai/code | סביבת קידוד AI של Anthropic — דורשת מנוי בתשלום |
| [Remotion](https://www.remotion.dev) | https://www.remotion.dev | ספריית React ליצירת סרטוני וידאו תכנותיים — מרנדרת React components לקבצי MP4 |
| [Remotion Agent Skills](https://www.remotion.dev/docs/ai/skills) | https://www.remotion.dev/docs/ai/skills | Skill להתקנה ב-Claude Code שמלמד אותו את ה-API, דפוסי האנימציה וה-best practices של Remotion |

## ריפוזיטוריז

- https://github.com/remotion-dev/remotion

## פריטי פעולה

- [ ] הרץ `npx skills add remotion-dev/skills` בתיקייה ריקה ובדוק יצירת טיזר מוצר לפרויקט taylor-played
- [ ] עיין בתיעוד הרשמי בכתובת https://www.remotion.dev/docs/ai/claude-code לתהליך ההתקנה המלא
- [ ] בדוק את עמוד הרישיון של Remotion לפני שימוש מסחרי — ייתכן שנדרש רישיון חברה בתשלום

## הערות אימות

- ⚠️ הטרנסקריפט טוען 'no editing software needed' — נכון לגרסה ראשונית, אך איטרציות מורכבות עשויות לדרוש היכרות עם קוד React/Remotion
- ⚠️ הטרנסקריפט לא מציין את הצורך במנוי Claude Code בתשלום — מידע חסר קריטי למשתמש חדש
- ⚠️ הביטוי 'full videos' מוגזם — מדובר בסרטוני motion graphics ואנימציה מבוססי React, לא בוידאו עם פוטאז' אמיתי

