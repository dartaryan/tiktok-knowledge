---
title_he: "MemPalace — מערכת זיכרון פתוחה ל-AI המבוססת על "ארמון הזיכרון" היווני"
title_en: "MemPalace — Open-Source AI Memory System Inspired by the Ancient Method of Loci"
source: "https://vt.tiktok.com/ZSHCSTCLG"
creator: "@github.awesome"
platform: "tiktok"
category: "optiplan"
relevance: 3
date_processed: "2026-04-11"
tags: ["ai-memory", "mcp", "claude-code", "rag", "local-llm", "open-source"]
---

## תקציר

השחקנית מילה יובוביץ' ומהנדס בשם Ben Sigman שחררו בקוד פתוח מערכת זיכרון ל-LLM בשם MemPalace, שמאחסנת שיחות verbatim ומאורגנת כ"ארמון זיכרון" עם כנפות (wings), אולמות (halls) וחדרים (rooms) — במקום חיפוש שטוח ב-vector database. המערכת משתלבת עם Claude Code דרך 19 כלי MCP, רצה מקומית על ChromaDB ו-SQLite ללא עלויות API, ומשיגה 96.6% על ה-LongMemEval benchmark. עם זאת, קהילת המפתחים מצאה שגיאות מהותיות בתיעוד וחלק מהטענות על הביצועים הן מופרזות.

## תובנות מפתח

- ניתן לקשר את MemPalace ל-Claude Code דרך MCP בפקודה אחת (`claude mcp add mempalace`) ואז Claude ישתמש בו אוטומטית — רלוונטי לכל פרויקט שעובדים עליו עם Claude Code (כולל OptiPlan ו-TaylorPlayed)
- הארכיטקטורה ההיררכית (wing → hall → room) משפרת את דיוק החיפוש ב-34% לעומת flat semantic search — רעיון שניתן לאמץ בתכנון מבני זיכרון לסוכני AI
- אלטרנטיבות מסחריות: Mem0 (19–249$/חודש) ו-Zep (25$/חודש+) — MemPalace חינמי ומקומי לגמרי
- הסרטון מכיל מספר שגיאות עובדתיות: שם הכלי הוא MemPalace (לא Mempalis), שם האלגוריתם הוא AAAK (לא AK), ושם היוצרת הוא Milla (שתי L) ולא Mila

## כלים וספריות

| שם | קישור | תיאור |
|---|---|---|
| [MemPalace](https://github.com/milla-jovovich/mempalace) | https://github.com/milla-jovovich/mempalace | מערכת זיכרון פתוחה ל-LLM, מבוססת ארמון זיכרון, רצה מקומית עם ChromaDB ו-SQLite, משתלבת עם Claude Code דרך MCP |
| [ChromaDB](https://www.trychroma.com/) | https://www.trychroma.com/ | מסד נתונים וקטורי (vector database) לחיפוש סמנטי, רץ מקומית |
| [Mem0](https://github.com/mem0ai/mem0) | https://github.com/mem0ai/mem0 | שכבת זיכרון מסחרית ל-AI agents — אלטרנטיבה בתשלום ל-MemPalace |

## ריפוזיטוריז

- https://github.com/milla-jovovich/mempalace

## פריטי פעולה

- [ ] לנסות להתקין MemPalace על Claude Code בפרויקט OptiPlan: `pip install mempalace` ואז `claude mcp add mempalace -- python -m mempalace.mcp_server` — ולבדוק אם זה משמר context ארכיטקטוני בין sessions
- [ ] לקרוא את ה-README המעודכן ב-GitHub ולעקוב אחרי ה-issues הפתוחים לפני אימוץ — הקהילה מצאה פערים בין התיעוד לקוד האמיתי

## הערות אימות

- ⚠️ הסרטון קורא לכלי 'Mempalis' — השם הנכון הוא MemPalace
- ⚠️ הסרטון קורא לאלגוריתם 'AK' — השם הנכון הוא AAAK
- ⚠️ הסרטון טוען שה-AAAK דוחס 'ללא אובדן משמעות סמנטית' — אבל הצוות עצמו מאשר ש-AAAK הוא lossy ומוריד דיוק מ-96.6% ל-84.2%
- ⚠️ הטענה על '30x lossless compression' הודתה ע"י הצוות כמוגזמת — בפועל AAAK הוא מערכת קיצורים lossy
- ⚠️ ציון ה-100% ב-LongMemEval שנוי במחלוקת: הושג אחרי תיקונים ממוקדים על שאלות כושלות ועם LLM reranking — הציון ה-raw האמין הוא 96.6%
- ⚠️ ה-README מתאר 'contradiction detection' שלא קיים בפועל בקוד
- ⚠️ קיים ויכוח ציבורי על מידת המעורבות הטכנית האמיתית של יובוביץ' בפיתוח

