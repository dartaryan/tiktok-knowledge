---
title_he: "Claude Code כמנוע מחקר: שילוב Skills, Notebook LM ו-Obsidian לוורקפלו אוטומטי משתפר-עצמי"
title_en: "Claude Code Research Workflow: Combining Skills, NotebookLM and Obsidian into a Self-Improving Pipeline"
source: "https://vt.tiktok.com/ZSumoAT6M/"
creator: "@chase_ai_"
category: "shalhevet"
relevance: 3
date_processed: "2026-03-26"
tags: ["claude-code", "skills", "notebooklm", "obsidian", "research-workflow", "automation"]
---

## תקציר

הסרטון מדגים כיצד לבנות ב-Claude Code וורקפלו מחקר אוטומטי המחבר חיפוש YouTube דרך yt-dlp, ניתוח מידע ב-Notebook LM, ואחסון תובנות ב-Obsidian — הכל דרך מנגנון ה-Skills של Claude Code. הגישה מאפשרת לאגד כמה sub-skills לסופר-סקיל אחד דרך פלאגין Skill Creator הרשמי של Anthropic. הוורקפלו גמיש לחלוטין — ניתן להחליף את מקור הנתונים (YouTube → PDF, מאמרים, מסמכים) ולהתאים לכל תחום.

## תובנות מפתח

- מנגנון Skills ב-Claude Code מאפשר לעטוף וורקפלואים מורכבים לפקודת slash אחת — ניתן לאגד כמה sub-skills לסופר-סקיל אחד דרך Skill Creator, שהוא פלאגין רשמי של Anthropic
- Notebook LM משמש כמנוע ניתוח חיצוני: העיבוד נעשה בענן של Google ולא צורך טוקנים של Claude, ומייצר deliverables כמו אינפוגרפיקה, podcast, mind map וכרטיסיות למידה
- קובץ CLAUDE.md בתוך vault של Obsidian משמש כ'מוח תוך מוח' — אחסון העדפות עבודה שניתן לעדכן אחרי כל ריצה כדי לשפר את התנהגות Claude עם הזמן
- notebooklm-py משתמש ב-API לא-רשמי ובאוטומציה של דפדפן — עלול להישבר עם עדכוני Google; מומלץ להשתמש בחשבון Google ייעודי ולא בחשבון ראשי
- תבנית הוורקפלו (מקור נתונים → Notebook LM → Obsidian + Skill Creator) ניתנת לשימוש חוזר בכל use case — רלוונטי לאימוני AI כדוגמה לגמישות של Claude Code Skills
- הסרטון רלוונטי גם לקטגוריה elon-katzef: הרעיון של ניהול ידע מצטבר עם CLAUDE.md כ'עוזר אישי מאומן' ייתכן שמעניין בהקשר ייעוץ AI לארגון

## כלים וספריות

| שם | קישור | תיאור |
|---|---|---|
| [Claude Code](https://claude.ai/code) | https://claude.ai/code | סביבת פיתוח AI של Anthropic עם מנגנון Skills לבניית וורקפלואים מותאמים אישית |
| [Skill Creator](https://claude.com/plugins/skill-creator) | https://claude.com/plugins/skill-creator | פלאגין רשמי של Anthropic ל-Claude Code — ארבעה מצבי עבודה: Create, Eval, Improve ו-Benchmark לפיתוח Skills מלא ומבוסס-נתונים |
| [notebooklm-py](https://github.com/teng-lin/notebooklm-py) | https://github.com/teng-lin/notebooklm-py | ספריית Python לא-רשמית ל-Google NotebookLM — גישה מלאה דרך CLI ו-AI agents כולל יצירת deliverables, חיפוש אינטרנטי, ואינטגרציה ל-Claude Code |
| [Google NotebookLM](https://notebooklm.google.com) | https://notebooklm.google.com | כלי מחקר של Google המבוסס על Gemini — ניתוח מקורות ויצירת podcast, אינפוגרפיקה, כרטיסיות למידה, slide deck ועוד, עד 50 מקורות לנייטבוק |
| [Obsidian](https://obsidian.md) | https://obsidian.md | אפליקציית ניהול ידע מבוססת Markdown — משמשת כ-vault לשמירת תובנות מחקר, גרף קישורים בין מסמכים, ו-CLAUDE.md לזיכרון מצטבר של Claude |
| [yt-dlp](https://github.com/yt-dlp/yt-dlp) | https://github.com/yt-dlp/yt-dlp | כלי CLI לחיפוש והורדת מידע מ-YouTube — משמש כמקור נתונים ראשי בוורקפלו המחקר של הסרטון |

## ריפוזיטוריז

- https://github.com/teng-lin/notebooklm-py

## פריטי פעולה

- [ ] התקן את פלאגין Skill Creator ב-Claude Code דרך /plugin ולאחר מכן: /skill-creator
- [ ] התקן את notebooklm-py: pip install 'notebooklm-py[browser]' && playwright install chromium, ואז: notebooklm login
- [ ] בנה skill לחיפוש YouTube דרך /skill-creator — תאר שימוש ב-yt-dlp לחיפוש ולהחזרת תוצאות מובנות
- [ ] בנה skill לניהול Notebook LM דרך /skill-creator — ציין את ה-GitHub repo של notebooklm-py כהפניה
- [ ] אגד את שני ה-skills לסופר-סקיל אחד (pipeline skill) באמצעות /skill-creator עם תיאור הוורקפלו המלא
- [ ] הגדר vault של Obsidian כ-working directory ב-Claude Code וצור קובץ CLAUDE.md ראשוני עם העדפות עבודה
- [ ] לאחר כל ריצת וורקפלו, בקש מ-Claude Code לעדכן את CLAUDE.md: 'Update CLAUDE.md to better reflect my work style and output preferences based on our latest session'

## הערות אימות

- ⚠️ notebooklm-py משתמש ב-undocumented RPC protocol של Google — עלול להישבר בכל עדכון Google; ה-ToS של Google אוסרת על גישה אוטומטית (ראה: https://github.com/teng-lin/notebooklm-py)
- ⚠️ הטענה ש'הוורקפלו משתפר לבד עם הזמן' מוגזמת — CLAUDE.md הוא קובץ סטטי שנקרא ב-context; השיפור תלוי בעדכון ידני/מפורש של הקובץ, לא ב-fine-tuning אמיתי
- ⚠️ הטענה שעיבוד ב-Notebook LM לא עולה טוקנים של Claude — נכון לגבי שלב העיבוד, אך העברת התוצאות חזרה ל-Claude Code כן צורכת context window

