---
title_he: "Office CLI – כלי שורת פקודה לסוכני AI לאוטומציה של קבצי Word, Excel ו-PowerPoint ללא Microsoft Office"
title_en: "Office CLI – AI Agent-Native CLI for Word/Excel/PowerPoint Without Microsoft Office"
source: "https://vt.tiktok.com/ZSHLDko6o"
creator: "@github.awesome"
platform: "tiktok"
category: "elon-katzef"
relevance: 4
date_processed: "2026-03-30"
tags: ["ai-agents", "office-automation", "cli", "document-processing", "enterprise-ai", "csharp"]
---

## תקציר

Office CLI הוא כלי שורת פקודה (CLI) קוד-פתוח, בינארי יחיד, שמאפשר לסוכני AI לקרוא, לערוך ולהפעיל אוטומציה על קבצי Word, Excel ו-PowerPoint ישירות מהטרמינל — ללא צורך בהתקנת Microsoft Office. הכלי כתוב ב-C# ומשולב עם runtime של .NET מובנה, כך שאין תלויות חיצוניות. הוא רלוונטי במיוחד לסביבות ארגוניות שבהן סוכני AI צריכים לעבד חוזים, דוחות Excel ומצגות פנימיות בצורה אוטומטית.

## תובנות מפתח

- הכלי פותר בעיה מרכזית של סוכני AI בסביבות ארגוניות: חוסר יכולת לגעת בפורמטי Office קנייניים (docx, xlsx, pptx) ללא תוכנת Microsoft המותקנת
- קיים קובץ SKILL.md (~8K טוקנים) שמלמד את ה-agent כיצד להשתמש בכלי — ניתן להדביק ישירות בצ'אט של הסוכן ו-הוא ילמד ויתקין אוטומטית
- תומך בפעולות מתקדמות ב-Excel: נוסחאות, pivot tables, תרשימים, עיצוב מותנה; ב-Word: טבלאות, סגנונות, headers/footers, תוכן עניינים; ב-PowerPoint: אנימציות, מעברים, מודלים תלת-ממדיים
- רלוונטי גם לפרויקט shalhevet להדגמת יכולות סוכני AI בהכשרות — דוגמה חזותית ומרשימה לאוטומציה של משרד
- חלופה אפשרית לתסריטי Python עם python-docx / openpyxl — יתרון: בינארי יחיד ללא ניהול סביבת Python

## כלים וספריות

| שם | קישור | תיאור |
|---|---|---|
| [OfficeCLI](https://github.com/iOfficeAI/OfficeCLI) | https://github.com/iOfficeAI/OfficeCLI | כלי CLI קוד-פתוח לסוכני AI לעבודה עם קבצי Word, Excel ו-PowerPoint — בינארי יחיד, ללא צורך בהתקנת Microsoft Office |

## ריפוזיטוריז

- https://github.com/iOfficeAI/OfficeCLI

## פריטי פעולה

- [ ] התקן את OfficeCLI בסביבת פיתוח מקומית והרץ תסריט ניסיוני: קריאת דוח Excel, שינוי ערך תא, שמירה — לאמת שעובד ללא Office מותקן
- [ ] שלב את SKILL.md של OfficeCLI בהגדרות system prompt של סוכן AI ארגוני ובדוק אוטומציה של חוזה Word לדוגמה
- [ ] הצג ל-Alon תסריט שימוש: סוכן AI שמייצר דוח Excel חודשי לחברת הביטוח מנתוני מסד נתונים, ללא מעורבות אנושית

## הערות אימות

- ⚠️ הטענה 'world's first Office suite designed for AI agents' היא שיווקית ולא ניתנת לאימות — קיימים כלים קודמים לעיבוד Office (python-docx, openpyxl) אם כי לא ממוקדי-agents בצורה זו
- ⚠️ יש לבדוק תמיכה ב-Hebrew/RTL בתוכן Word ו-Excel — קריטי לשימוש בסביבה ישראלית

