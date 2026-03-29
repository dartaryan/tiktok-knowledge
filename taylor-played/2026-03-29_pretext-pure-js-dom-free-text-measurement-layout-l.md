---
title_he: "PreText: ספריית JavaScript למדידת טקסט ללא DOM ו-CSS"
title_en: "PreText: Pure-JS DOM-Free Text Measurement & Layout Library"
source: "https://vt.tiktok.com/ZSHR9TNJb"
creator: "@github.awesome"
platform: "tiktok"
category: "taylor-played"
relevance: 3
date_processed: "2026-03-29"
tags: ["javascript", "text-layout", "performance", "canvas", "dom-free", "animation"]
---

## תקציר

PreText היא ספריית JavaScript/TypeScript חדשה שמבצעת מדידת טקסט ועיצוב שורות מרובות ללא קריאות DOM (כלומר, ללא layout reflow). היא משתמשת ב-canvas.measureText() כדי לבצע מדידה חד-פעמית, ולאחר מכן כל חישוב ה-layout הוא אריתמטיקה טהורה על cache — מה שמאפשר אנימציות טקסט חלקות ב-60fps. הספרייה תומכת ב-DOM, Canvas, SVG ו-server-side rendering.

## תובנות מפתח

- הבעיה שנפתרת: קריאות DOM כמו getBoundingClientRect() ו-offsetHeight גורמות ל-layout reflow — עבור 500 בלוקי טקסט זה עולה 15–30ms לפריים. PreText מביא את זה ל-0.05ms — שיפור של 300–600x לפי הבנצ'מרקים
- האדריכלות דו-שלבית: prepare() רץ פעם אחת כשהטקסט מופיע (מנרמל whitespace, מסמנט עם Intl.Segmenter, מודד דרך canvas), ואז layout() רץ על כל resize בעזרת אריתמטיקה בלבד — ללא DOM, ללא canvas, ללא string allocations
- רלוונטי ל-TailorPlayed בהקשר של Canvas rendering ואנימציות UI מורכבות, למשל visualizations של לוח משחק עם טקסט דינמי
- הספרייה גם שימושית ל-virtual scrolling ורשימות ארוכות שצריכות לחשב גובה פריטים מראש ללא mounting לDOM — פוטנציאל ל-OptiPlan בדשבורדים עם נתונים רבים
- הספרייה שוקלת 15KB בלבד וללא dependencies

## כלים וספריות

| שם | קישור | תיאור |
|---|---|---|
| [PreText (@chenglou/pretext)](https://github.com/chenglou/pretext) | https://github.com/chenglou/pretext | ספריית JavaScript/TypeScript למדידת טקסט multiline וביצוע layout ללא קריאות DOM — תומכת ב-DOM, Canvas, SVG ו-server-side |

## ריפוזיטוריז

- https://github.com/chenglou/pretext

## פריטי פעולה

- [ ] לבדוק אם PreText יכול לשפר ביצועים ב-Canvas-based rendering ב-TailorPlayed (למשל תצוגת רכיבי לוח משחק עם תוויות טקסט)
- [ ] לצפות בדמואים החיים בכתובת chenglou.me/pretext כדי להבין את טווח היכולות
- [ ] לבדוק את השימוש ב-prepareWithSegments() + layoutWithLines() לצורך layout מדויק עם שורות קבועות

## הערות אימות

- ⚠️ הטענה בסרטון '20 שנה של CSS לטקסט' מוגזמת — הבעיה היא ספציפית ל-layout reflow בעת מדידה דינמית, לא CSS בכלל
- ⚠️ הטענה '300–600x מהיר יותר' מגיעה מבנצ'מרקים ספציפיים (500 בלוקים). יש לבדוק ביצועים בתרחישים אמיתיים של האפליקציה
- ⚠️ הספרייה חדשה יחסית — יש לבדוק רמת בשלות ותמיכה בדפדפנים לפני שימוש בפרודקשן

