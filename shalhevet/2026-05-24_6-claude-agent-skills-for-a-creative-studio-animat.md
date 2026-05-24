---
title_he: "6 סקילס של Claude לסטודיו קריאייטיב: אנימציה, מחקר תחרותי, קול ותוכן"
title_en: "6 Claude Agent Skills for a Creative Studio: Animation, Competitor Research, Voice DNA & Content"
source: "https://www.instagram.com/reel/DYh0vdAv2_s/"
creator: "@Cindy Zhu"
platform: "instagram"
category: "shalhevet"
relevance: 3
date_processed: "2026-05-24"
tags: ["claude-skills", "claude-code", "remotion", "voice-dna", "elevenlabs", "content-creation", "agent-skills"]
---

## תקציר

הסרטון מציג 6 סקילס (Agent Skills — תוספי יכולות מודולריים) עבור Claude Code שיחד מרכיבים 'סטודיו קריאייטיב' אוטומטי. הכלים מכסים יצירת סרטוני אנימציה (Remotion), מחקר מתחרים (Competitive Ads Extractor), מחקר שוק אוטומטי ברקע (Deep Research), שמירת סגנון כתיבה אישי (Voice DNA), המרת מסמכים לפודקאסט (ElevenLabs), וכתיבת תוכן מחקרי עם ציטוטים (Content Research Writer). כל הסקילס מותקנים דרך פקודת npx אחת ועובדים ישירות בתוך Claude Code. שימו לב: הסרטון מכריז על '7 סקילס' אך מציג בפועל רק 6.

## תובנות מפתח

- סקילס של Claude הם קבצי Markdown מובנים (SKILL.md) המלמדים את Claude כיצד לבצע משימות ספציפיות — מותקנים פעם אחת ופועלים אוטומטית בכל שיחה רלוונטית
- Remotion (פריימוורק ליצירת סרטוני אנימציה ב-React) — הסקיל שלו מלמד את Claude Code את כל ה-API של Remotion, מה שמאפשר ליצור סרטוני אנימציה מקצועיים רק בתיאור טקסטואלי, ללא עריכת וידאו
- Voice DNA מנתח 3-10 דוגמאות כתיבה של המשתמש ומייצר פרופיל JSON מפורט (קצב משפטים, אוצר מילים, סגנון) — פוטנציאל גבוה לסדנאות AI Literacy כהדגמה לאישיות של פלט AI
- Competitive Ads Extractor שולף מודעות מספריות פרסום פתוחות (Facebook Ad Library, LinkedIn) ומנתח messaging, CTAs ותבניות קריאייטיב — כלי שיכול להדגים ערך עסקי מיידי בסדנאות
- ElevenLabs skill יכול להפוך כל מסמך לנארציה של מוזיקאי יחיד או לפודקאסט של שני מארחים אוטומטית — דורש subscription בניגוד לאחרים
- Content Research Writer מסייע בכתיבה end-to-end כולל מחקר, ניהול ציטוטים ופידבק לפי סעיף — מוצא ב-awesome-claude-skills של ComposioHQ

## כלים וספריות

| שם | קישור | תיאור |
|---|---|---|
| [Remotion](https://www.remotion.dev/) | https://www.remotion.dev/ | פריימוורק ליצירת סרטוני וידאו ואנימציה בקוד React/TypeScript; הסקיל שלו מותקן עם `npx skills add remotion-dev/skills` |
| [Competitive Ads Extractor (Claude Skill)](https://github.com/ComposioHQ/awesome-claude-skills/tree/master/competitive-ads-extractor) | https://github.com/ComposioHQ/awesome-claude-skills/tree/master/competitive-ads-extractor | סקיל Claude שמחלץ מודעות מתחרים מ-Facebook Ad Library ו-LinkedIn ומנתח messaging, hooks ו-CTAs עובדים |
| [Deep Research (Claude Skill)](https://github.com/ComposioHQ/awesome-claude-skills) | https://github.com/ComposioHQ/awesome-claude-skills | סקיל agent מולטי-שלבי המריץ ניתוח שוק ומחקר תחרותי ברקע תוך שימוש ב-Gemini Deep Research |
| [Voice DNA Creator (Claude Skill)](https://github.com/az9713/ai-co-writing-claude-skills) | https://github.com/az9713/ai-co-writing-claude-skills | סקיל שמנתח דוגמאות כתיבה ומייצר פרופיל JSON של הקול האישי — סגנון, קצב, אוצר מילים, ביטויים שיש להימנע מהם |
| [ElevenLabs](https://elevenlabs.io/) | https://elevenlabs.io/ | פלטפורמת text-to-speech (TTS) מתקדמת; הסקיל שלה בתוך Claude Code מאפשר המרת מסמכים לנארציה או לפודקאסט דו-מארחים |
| [Content Research Writer (Claude Skill)](https://github.com/ComposioHQ/awesome-claude-skills) | https://github.com/ComposioHQ/awesome-claude-skills | סקיל המסייע בכתיבת תוכן end-to-end: מחקר, ציטוטים, שיפור hooks ופידבק סעיף-סעיף תוך שמירה על קול ייחודי |
| [skills.sh (Agent Skills Registry)](https://skills.sh) | https://skills.sh | ספרייה פתוחה של Agent Skills ל-Claude Code ו-Cursor; נקודת ההתקנה המרכזית עם `npx skills add [שם]` |

## ריפוזיטוריז

- https://github.com/ComposioHQ/awesome-claude-skills
- https://github.com/az9713/ai-co-writing-claude-skills
- https://github.com/remotion-dev/skills

## פריטי פעולה

- [ ] התקן את סקיל Remotion בסביבת פיתוח עם `npx skills add remotion-dev/skills` ונסה ליצור סרטון הסבר קצר על נושא מוכר — טוב להדגמה חיה בסדנת שלהבת
- [ ] בדוק את Voice DNA Creator מ-GitHub של az9713 — נסה להריץ אותו על מספר דוגמאות כתיבה שלך וראה את פרופיל ה-JSON המתקבל; שימוש פוטנציאלי בסדנאות AI Literacy
- [ ] הדגם את Competitive Ads Extractor בסדנת שלהבת הבאה כמקרה שימוש ממשי — מראה ערך עסקי ברור ומיידי ביחס למחקר שוק ידני
- [ ] בחן את ה-awesome-claude-skills repo של ComposioHQ לרשימת כל הסקילס הקיימים — שימושי לבניית catalog לסדנאות

## הערות אימות

- ⚠️ הסרטון מכריז על '7 סקילס' אך מציג בפועל רק 6 — ייתכן שהכותרת שיווקית בלבד או שסקיל אחד נשמט בעריכה
- ⚠️ הטענה ש-'5 מהם חינמיים לחלוטין' לא לגמרי מדויקת: Remotion rendering בענן (Lambda) יכול לעלות כסף; יש לוודא מה כולל ה'חינמי'
- ⚠️ הכותרת בטרנסקריפט כותבת 'ReMotion' עם R גדולה ו-M גדולה — בפועל הכלי נקרא Remotion (ראשון קטן, שני גדול)
- ⚠️ הסרטון מכנה את ElevenLabs בשם '11 laps' — ככל הנראה שגיאת הגייה; יש לוודא שהמאזינים מבינים שמדובר ב-ElevenLabs
- ⚠️ לא ברור אם Competitive Ads Extractor אכן שולף 'live ads' כפי שנטען — Facebook Ad Library מציגה נתונים עם עיכוב מסוים ויש הגבלות API; הטענה על real-time דורשת בדיקה

