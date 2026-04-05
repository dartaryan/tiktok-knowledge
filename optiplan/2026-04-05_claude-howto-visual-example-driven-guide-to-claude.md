---
title_he: "claude-howto: מדריך ויזואלי מלא לשימוש מתקדם ב-Claude Code — מ-prompts בסיסיים עד אורקסטרציה"
title_en: "claude-howto: Visual Example-Driven Guide to Claude Code — From Basic Prompts to AI Orchestration"
source: "https://vt.tiktok.com/ZSHUM7m8p"
creator: "@github.awesome"
platform: "tiktok"
category: "optiplan"
relevance: 4
date_processed: "2026-04-05"
tags: ["claude-code", "ai-orchestration", "mcp-servers", "hooks", "subagents", "developer-productivity"]
---

## תקציר

הריפו `claude-howto` הוא מדריך ויזואלי ומונחה-דוגמאות ל-Claude Code (כלי הפיתוח האינטראקטיבי של Anthropic בטרמינל), המכסה 10 מודולים מ-slash commands ועד multi-agent orchestration, hooks מותאמים אישית, skills ו-MCP servers — עם תבניות copy-paste מוכנות לשימוש ודיאגרמות Mermaid המסבירות את מנגנון הפעולה הפנימי. מסלול הלימוד המובנה אורך 11–13 שעות וכולל פקודת `/self-assessment` שמריצים ישירות ב-Claude Code ומייצרת מפת-דרכים אישית על בסיס הפערים הקיימים. הריפו רלוונטי לכל פרויקט פיתוח פעיל, ובפרט ל-optiplan שבו Claude Code משמש יומיומית.

## תובנות מפתח

- הריפו מכסה 117+ פיצ'רים ותבניות, כולל slash commands, subagents, skills, plugins, MCP servers, hooks ו-memory — הכל עם קבצי copy-paste מוכנים להתקנה
- פקודת `/self-assessment` (Quick = 2 דקות, Deep = 5 דקות) מייצרת פרופיל-מיומנות אישי ומסלול לימוד — כלי מצוין לזיהוי פיצ'רים של Claude Code שעדיין לא מנוצלים
- Hooks מאפשרים אוטומציה event-driven עם 25 אירועים ו-4 סוגי hooks (command, prompt, http, agent) — שימושיים לולידציה לפני כתיבת קוד קריטי ב-optiplan
- Plugins הם יחידה מאוחדת של commands + agents + MCP + hooks — ניתן להתקין workflow שלם (כגון pr-review או devops-automation) בפקודה אחת
- דוגמת `/review-pr` מדגימה orchestration מלא: טעינת project memory → קריאה ל-GitHub MCP → האצלה ל-code-reviewer subagent ול-test-engineer subagent → סינתזה — דפוס ישיר לפיתוח ב-optiplan
- רלוונטי גם לפרויקט shalhevet: המדריך עצמו הוא דוגמה מצוינת לאופן הצגת יכולות Claude Code בהכשרות AI

## כלים וספריות

| שם | קישור | תיאור |
|---|---|---|
| [claude-howto](https://github.com/luongnv89/claude-howto) | https://github.com/luongnv89/claude-howto | מדריך ויזואלי open-source (MIT) ל-Claude Code עם תבניות, hooks, subagents, skills ו-MCP servers מוכנים לשימוש |
| [Claude Code](https://docs.anthropic.com/en/docs/claude-code/overview) | https://docs.anthropic.com/en/docs/claude-code/overview | כלי הפיתוח האינטראקטיבי של Anthropic — agent קידוד שרץ בטרמינל ומסוגל לקרוא, לכתוב ולהריץ קוד |

## ריפוזיטוריז

- https://github.com/luongnv89/claude-howto

## פריטי פעולה

- [ ] לשכפל את https://github.com/luongnv89/claude-howto ולהריץ `/self-assessment` ב-Claude Code כדי לזהות פיצ'רים לא מנוצלים ולקבל מפת-דרכים אישית
- [ ] להעתיק תבניות subagents מ-04-subagents/ לתיקיית .claude/agents/ בפרויקט optiplan — להגדיר subagents ייעודיים ל-code-review, testing ותיעוד
- [ ] לקרוא את מודול 06-hooks/ ולהגדיר לפחות hook אחד מסוג PreToolUse ל-ולידציה אוטומטית לפני פעולות Bash קריטיות
- [ ] להתקין את GitHub MCP מ-05-mcp/ לניהול PRs ו-issues ישירות מהטרמינל מבלי לעזוב את סביבת הפיתוח
- [ ] לעיין ב-LEARNING-ROADMAP.md ולתכנן סשן 2–3 שעות לרמה 2 (hooks + MCP + subagents) בסוף השבוע

## הערות אימות

- ⚠️ הריפו מציין תאימות ל-Claude Code 2.1+ וגרסה v2.2.0 (מרץ 2026) — יש לוודא שגרסת Claude Code המותקנת תומכת בפיצ'רים כמו agent hooks ו-auto permission mode (מסומן כ-Research Preview)
- ⚠️ פקודת /fork שונה ל-/branch ב-v2.1.77 — ייתכן שחלק מהפקודות במדריך דורשות בדיקת עדכניות לגרסה המותקנת
- ⚠️ הריפו מציין 90% מ-Claude Code power לא מנוצל — טענה שיווקית, אך תומכת על ידי רשימת 117+ פיצ'רים מתועדים

