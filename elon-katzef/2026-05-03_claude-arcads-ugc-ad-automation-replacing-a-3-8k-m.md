---
title_he: "אוטומציה של פרסומות UGC עם Claude ו-Arcads: החלפת סוכנות פרסום יקרה ב-$300 לחודש"
title_en: "Claude + Arcads UGC Ad Automation: Replacing a $3–8K/Month Agency for $300"
source: "https://vt.tiktok.com/ZS9xRvh6f"
creator: "@adamstewartmarketing"
platform: "tiktok"
category: "elon-katzef"
relevance: 3
date_processed: "2026-05-03"
tags: ["ai-agents", "claude-md", "ugc", "marketing-automation", "arcads", "roi"]
---

## תקציר

הסרטון מציג workflow אוטונומי שבו Claude משמש כ-agent שכותב 20 סקריפטים לפרסומות, מדרג כל אחד מ-1 עד 10, ושולח את הטובים ביותר ל-API של Arcads לייצור וידאו UGC. הבסיס הוא קובץ CLAUDE.md (המכונה כאן 'claw.md') שמשמש כ'מוח קבוע' של ה-agent – כולל כללי תזמון, נוסחאות hook, ו-API endpoints. מידי 48 שעות ה-agent מעדכן את הסקריפטים בהתאם לנתוני ביצוע בפועל, מה שמדגים דפוס אוטומציה עם feedback loop רלוונטי לכל ארגון.

## תובנות מפתח

- קובץ CLAUDE.md כ'זיכרון אג'נט': הפטרן של הגדרת כלל-הפעולות של agent בקובץ markdown אחד ניתן ליישום בכל workflow עסקי – רלוונטי גם לתהליכים פנים-ארגוניים בחברת ביטוח
- השוואת ROI חדה: $300/חודש ל-500+ סרטונים מול $3,000–$8,000/חודש ל-8–15 סרטונים בסוכנות מסורתית – טיעון ממשי ומוחשי לשיחות אימוץ AI עם מנהלים בכירים
- דפוס feedback loop של 48 שעות: עדכון אוטומטי של פלט ה-AI לפי ביצוע בפועל – ניתן להקביל לתהליכי underwriting, תביעות, או תקשורת לקוחות בביטוח
- ה-GitHub repo של krusemediallc/arcads-claude-code מכיל סביבת Claude/Cursor מוכנה עם skills ל-Arcads API – משאב מעשי להדגמות agentic AI לאלון

## כלים וספריות

| שם | קישור | תיאור |
|---|---|---|
| [Claude](https://claude.ai) | https://claude.ai | מודל השפה של Anthropic, משמש כ-agent אוטונומי לכתיבה, דירוג, ובחירת סקריפטים |
| [Arcads](https://www.arcads.ai) | https://www.arcads.ai | פלטפורמת AI ליצירת פרסומות UGC וידאו עם 1,000+ שחקני AI, כולל API לאוטומציה |

## ריפוזיטוריז

- https://github.com/krusemediallc/arcads-claude-code

## פריטי פעולה

- [ ] בדוק את תמחור ה-API של Arcads (arcads.ai/features/ai-video-api) להבנת עלות ריאלית למול הטענה של $300/חודש
- [ ] חקור את ה-repo של krusemediallc/arcads-claude-code כ-template מוכן לבניית demo של Claude agent עם CLAUDE.md לאלון
- [ ] הכן הדגמת ROI מבוססת-מספרים (AI vs. שירות מסורתי) כ-framework לשיחות אימוץ AI עם הנהלת חברת הביטוח

## הערות אימות

- ⚠️ טענת '500+ סרטונים ב-$300/חודש' לא מפרטת אם העלות כוללת את ה-API של Arcads או רק את עלות Claude – דורשת בדיקת תמחור נפרדת
- ⚠️ הטענה ש-Claude 'מוריד את הסרטונים לדסקטופ כשהם מוכנים' מרמזת על יכולת polling אוטונומית – יש לאמת שניתן לממש זאת בפועל עם Claude API
- ⚠️ הקריאייטור מציע לשלוח את ה-setup המלא בתמורה לתגובה – סביר שיש כוונה מסחרית/affiliate ולכן יש לנקוט זהירות בנוגע לאמינות הנתונים

