---
title_he: "Ruflo: פלטפורמת אורקסטרציה של 60+ סוכני AI מקביליים ל-Claude Code"
title_en: "Ruflo (formerly Claude Flow): Multi-Agent Orchestration Framework for Claude Code"
source: "https://vt.tiktok.com/ZSuKoa9Wk"
creator: "@nicksadler.io"
category: "taylor-played"
relevance: 3
date_processed: "2026-03-27"
tags: ["multi-agent", "claude-code", "orchestration", "mcp", "open-source", "developer-tools"]
---

## תקציר

Ruflo (לשעבר Claude Flow) הוא framework בקוד פתוח המאפשר הרצה מקבילית של 60+ סוכני AI מיוחדים בתוך Claude Code, כאשר כולם חולקים זיכרון ולומדים מכל ריצה. הכלי מציע ניתוב חכם תלת-שכבתי: משימות פשוטות ל-WASM חינמי, משימות בינוניות למודל זול, ומשימות מורכבות למודל האופטימלי. לפי המפתחים, הניתוב החכם מוביל לחיסכון של עד 75% בעלויות API ולהגברת יעילות ה-Claude subscription פי 2.5.

## תובנות מפתח

- ארכיטקטורת סוכנים מיוחדים: מתכנן, מקודד, בודק ומאבטח רצים במקביל ומשתפים זיכרון – תבנית orchestrator/specialist מובנית
- ניתוב חכם 3-שכבות: WASM (חינמי) → מודל זול → מודל אופטימלי; בחירה אוטומטית לפי מורכבות המשימה
- Ruflo משתלב ל-Claude Code דרך MCP (Model Context Protocol) – 259 כלים זמינים ישירות בסשן
- הכלי לומד מכל ריצה ומאחסן patterns מוצלחים, מה שמוביל לניתוב טוב יותר לאורך זמן
- רלוונטי גם ל-optiplan: TypeScript-first, WASM acceleration, ומבנה hierarchical topology מתאים לפיתוח full-stack מורכב

## כלים וספריות

| שם | קישור | תיאור |
|---|---|---|
| [Ruflo (formerly Claude Flow)](https://github.com/ruvnet/ruflo) | https://github.com/ruvnet/ruflo | פלטפורמת אורקסטרציה של סוכני AI לסביבת Claude Code; v3.5 הוא ה-release הראשון הסטבילי, עם 60+ סוכנים ו-259 כלי MCP |
| [Claude Code](https://docs.anthropic.com/en/docs/claude-code/overview) | https://docs.anthropic.com/en/docs/claude-code/overview | סוכן הקידוד של Anthropic שאליו Ruflo מתחבר דרך MCP |
| [MCP (Model Context Protocol)](https://modelcontextprotocol.io) | https://modelcontextprotocol.io | פרוטוקול חיבור בין סוכני AI לכלים חיצוניים; הבסיס לאינטגרציה של Ruflo עם Claude Code |
| [agentic-flow](https://github.com/ruvnet/agentic-flow) | https://github.com/ruvnet/agentic-flow | ספריית ה-reinforcement learning הבסיסית שמפעילה את מנגנון הלמידה של Ruflo |

## ריפוזיטוריז

- https://github.com/ruvnet/ruflo
- https://github.com/ruvnet/claude-flow

## פריטי פעולה

- [ ] להריץ `npx ruflo@latest init --wizard` בפרויקט TailorPlayed לבדיקת זמן onboarding
- [ ] לבדוק אם ניתוב ה-WASM אכן מאפס עלויות על משימות קידוד חוזרות (refactoring, type fixes)
- [ ] לחקור את ה-hierarchical topology עבור swarm של agents: architect → coder → tester – תבנית ישימה ב-OptiPlan ו-TailorPlayed

## הערות אימות

- ⚠️ הסרטון טוען '14,000 כוכבים' – הריפו הנוכחי (ruflo) מציג 26k+ כוכבים; הנתון בסרטון שייך כנראה לריפו הישן (claude-flow) בזמן הצילום
- ⚠️ טענת 'חיסכון של 75% בעלויות API' מגיעה מה-README של הפרויקט בלבד, ללא benchmark עצמאי
- ⚠️ הגדרת '#1 in agent frameworks on GitHub' היא הצהרה עצמית של המפתחים ולא אומתה על ידי גורם חיצוני
- ⚠️ הטענה 'getting smarter every single run' מבוססת על מנגנון ReasoningBank – יש לבדוק עד כמה השיפור מדיד בפועל

