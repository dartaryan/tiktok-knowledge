---
title_he: "Ruflo (לשעבר Claude Flow) — פלטפורמת תזמור Multi-Agent לפיתוח תוכנה עם Claude Code"
title_en: "Ruflo (formerly Claude Flow) — Multi-Agent Orchestration Platform for Claude Code Development"
source: "https://vt.tiktok.com/ZSH1d9VY3"
creator: "@nicksadler.io"
category: "taylor-played"
relevance: 3
date_processed: "2026-03-27"
tags: ["multi-agent", "claude-code", "orchestration", "open-source", "mcp", "cost-optimization"]
---

## תקציר

Ruflo הוא framework (מסגרת עבודה) לתזמור Multi-Agent בקוד פתוח, שהופך את Claude Code לפלטפורמת פיתוח עם 60+ agents מתמחים הפועלים במקביל — מתכנן, כותב קוד, מריץ בדיקות, בודק אבטחה — תוך שיתוף זיכרון ולמידה מתמשכת בין ריצות. הכלי תומך גם ב-LLM אחרים (GPT, Gemini, מודלים מקומיים) ומנתב משימות פשוטות למודלים זולים יותר כדי לחסוך בעלויות API. הפרויקט אומת כקיים ב-GitHub עם 27,000+ כוכבים (נכון למרץ 2026), ופתוח לחלוטין ללא עלות נוספת.

## תובנות מפתח

- Ruflo היא גרסה הנוכחית של Claude Flow — הרפו GitHub הוא ruvnet/ruflo, ניתן להתקין עם npx ruflo@latest init
- המערכת כוללת 60+ agent מתמחים (coder, tester, reviewer, architect, security ועוד) עם זיכרון משותף ולמידה רציפה — דפוס orchestrator/specialist שרלוונטי לארכיטקטורת Multi-Agent ב-taylor-played
- Smart routing מנתב משימות פשוטות למודלים זולים/מקומיים דרך WASM ומשימות מורכבות למודל האופטימלי — הרעיון ישים גם ב-Gemini API integration של taylor-played
- תוכן שניתן לשימוש גם ב-optiplan: הכלי בנוי ב-TypeScript עם MCP (Model Context Protocol) ותומך ב-React/TypeScript workflows
- ספירת הכוכבים בסרטון (14,000) מיושנת — נכון לבדיקה במרץ 2026 הריפו עומד על 27,100+ כוכבים
- התקנה מהירה: npx ruflo@latest init --wizard, או הוספה כ-MCP server ל-Claude Code: claude mcp add ruflo -- npx -y ruflo@latest mcp start

## כלים וספריות

| שם | קישור | תיאור |
|---|---|---|
| [Ruflo (formerly Claude Flow)](https://github.com/ruvnet/ruflo) | https://github.com/ruvnet/ruflo | פלטפורמת תזמור Multi-Agent בקוד פתוח ל-Claude Code — 60+ agents מתמחים, זיכרון משותף, ניתוב חכם בין מודלים, 313 כלי MCP |
| [Claude Code](https://claude.ai/code) | https://claude.ai/code | סביבת הפיתוח של Anthropic ש-Ruflo מרחיב לפלטפורמת Multi-Agent |
| [MCP (Model Context Protocol)](https://modelcontextprotocol.io) | https://modelcontextprotocol.io | פרוטוקול סטנדרטי לחיבור כלים חיצוניים ל-Claude — Ruflo מספק 313+ כלי MCP |

## ריפוזיטוריז

- https://github.com/ruvnet/ruflo

## פריטי פעולה

- [ ] לבחון שימוש ב-Ruflo כ-development tool לפרויקט taylor-played: הרץ npx ruflo@latest init --wizard בתוך repo הפרויקט וצפה כיצד agents מתמחים (coder/tester/reviewer) מתאמים עבודה
- [ ] לחקור את דפוס ה-smart routing של Ruflo (משימה פשוטה → WASM/מודל זול, מורכבת → מודל מיטבי) כהשראה לארכיטקטורת Multi-Agent ב-taylor-played עם Gemini API
- [ ] לבדוק את ה-plugin SDK של Ruflo ואת IPFS marketplace לרעיונות נוספים לארכיטקטורת orchestrator/specialist

## הערות אימות

- ⚠️ טענת '75% חיסכון בעלויות Claude API' — לא נמצא אימות מדויק לנתון זה בתיעוד הרשמי; הריפו מציין smart routing ו-WASM לביצוע מקומי אך ללא אחוז מדויק זה
- ⚠️ טענת 'מדורג מספר 1 ב-agent frameworks ב-GitHub' — קשה לאמת; ספירת הכוכבים בסרטון (14,000) מיושנת, הריפו עומד על 27,100+ כוכבים נכון לבדיקה
- ⚠️ הסרטון מציג תוכן פרסומי-וויראלי אופייני ל-TikTok עם הגזמות ('most powerful on the planet') — הכלי עצמו אמיתי ופעיל, אך כדאי לבדוק עצמאית לפני שימוש בפרודקשן

