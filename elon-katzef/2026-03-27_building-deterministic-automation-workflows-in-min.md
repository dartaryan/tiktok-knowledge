---
title_he: "בניית אוטומציות דטרמיניסטיות תוך דקה עם Claude Code ו-n8n דרך MCP"
title_en: "Building Deterministic Automation Workflows in Minutes with Claude Code + n8n via MCP"
source: "https://vt.tiktok.com/ZSuKcuKxG/"
creator: "@garethklapproth"
category: "elon-katzef"
relevance: 4
date_processed: "2026-03-27"
tags: ["claude-code", "n8n", "mcp", "workflow-automation", "sop-automation", "no-code"]
---

## תקציר

הסרטון מדגים כיצד חיבור Claude Code (כלי הקידוד של Anthropic) ל-n8n (פלטפורמת אוטומציית workflows) דרך שרת MCP מאפשר בניית כלי אוטומציה מלאים בדקה אחת — ללא כתיבת קוד ידנית. המדגם כולל יצירת כלי לניתוח אתרי אינטרנט הכולל ממשק טופס ו-LLM של OpenAI. הנקודה המעשית למנהלים: נהלים מתועדים (SOPs) ניתן להזין ישירות ל-Claude Code, שיבנה את האוטומציה אוטומטית.

## תובנות מפתח

- אוטומציה 'דטרמיניסטית' פירושה שה-AI בונה workflow עם פלט צפוי ומבוקר — ולא מייצר תשובות חופשיות. זה חשוב לסביבה ארגונית.
- SOPs (נהלי עבודה מתועדים) הם חומר גלם מושלם לבניית אוטומציות: מזינים את הנוהל ל-Claude Code, הוא בונה workflow ב-n8n אוטומטית.
- n8n מציעה מעל 1,200 nodes לאינטגרציות (Gmail, Slack, Salesforce, SAP וכו') — שילוב עם Claude Code דרך MCP הופך אותה לכלי עוצמתי לאוטומציה ארגונית ללא צוות פיתוח.
- הדמו מציג בניית כלי ניתוח אתרים שכולל ממשק גרפי, קריאת LLM ותצוגת תוצאות — בדקה בודדת. זה רלוונטי מאוד כדוגמת 'quick win' להצגה בפני הנהלה.
- רלוונטי גם לפרויקט shalhevet — הדמו הקצר מאוד מתאים להצגה בסדנאות AI כדי להמחיש קפיצת יכולת לפרטיקציפנטים לא-טכניים.

## כלים וספריות

| שם | קישור | תיאור |
|---|---|---|
| [Claude Code](https://docs.anthropic.com/en/docs/claude-code) | https://docs.anthropic.com/en/docs/claude-code | כלי CLI של Anthropic לקידוד אוטונומי — מקבל הנחיה ומממש קוד/workflows בצורה עצמאית |
| [n8n](https://n8n.io) | https://n8n.io | פלטפורמת אוטומציה של workflows בקוד פתוח עם מעל 1,200 integrations, ניתנת להרצה עצמית (self-hosted) או בענן |
| [n8n-mcp](https://github.com/czlonkowski/n8n-mcp) | https://github.com/czlonkowski/n8n-mcp | שרת MCP (Model Context Protocol) שמחבר בין Claude Code/Desktop לבין n8n, מאפשר ל-AI לבנות ולנהל workflows ישירות |
| [MCP (Model Context Protocol)](https://modelcontextprotocol.io) | https://modelcontextprotocol.io | פרוטוקול תקני המאפשר למודלי AI להתחבר לכלים חיצוניים ולבצע פעולות בעולם האמיתי |
| [OpenAI API](https://platform.openai.com) | https://platform.openai.com | ה-LLM שנבחר בתוך ה-workflow לניתוח האתר — ניתן להחליף בכל מודל אחר |

## ריפוזיטוריז

- https://github.com/czlonkowski/n8n-mcp

## פריטי פעולה

- [ ] להכין רשימה של 3-5 SOPs פשוטים מחברת הביטוח (למשל: תהליך הגשת תביעה, אונבורדינג לקוח חדש) ולנסות להזין אחד ל-Claude Code עם הוראה לבנות workflow ב-n8n.
- [ ] להתקין את n8n-mcp על ידי הרצת `npx n8n-mcp` ולחבר ל-Claude Code — ראה הוראות ב-https://github.com/czlonkowski/n8n-mcp/blob/main/docs/CLAUDE_CODE_SETUP.md
- [ ] לשקול להשתמש בדמו הזה (Claude Code בונה כלי ב-n8n תוך דקה) כ'wow moment' בהצגה בפני המנכ"ל לצורך שכנוע אימוץ AI בארגון.
- [ ] לבדוק אם n8n מציעה nodes רלוונטיים לתעשיית הביטוח (CRM, ERP, מסמכי תביעות) לפני בניית POC ארגוני.

## הערות אימות

- ⚠️ הטענה 'בניתי את זה בדקה אחת' — סביר שההגדרה הראשונית (התקנת n8n, חיבור MCP, קנפוג API keys) לוקחת זמן משמעותי יותר. הדקה מתייחסת לבניית ה-workflow הספציפי לאחר שהסביבה כבר מוגדרת.
- ⚠️ לא ברור איזה MCP GitHub repo ספציפי הוצג בסרטון — הסבירות הגבוהה ביותר היא czlonkowski/n8n-mcp שהוא הפופולרי ביותר, אך ייתכן שמדובר בריפו אחר.
- ⚠️ הטענה על 'deterministic automation' — n8n workflows אכן דטרמיניסטיים, אך ה-LLM בתוכם (OpenAI) אינו דטרמיניסטי כברירת מחדל. יש להגדיר temperature=0 לקבלת תוצאות עקביות.

