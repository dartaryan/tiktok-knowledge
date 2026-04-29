---
title_he: "andrej-karpathy-skills: קובץ CLAUDE.md שמכניס משמעת לסוכני קוד AI"
title_en: "andrej-karpathy-skills: A CLAUDE.md File for Disciplined AI Coding Agents"
source: "https://vt.tiktok.com/ZS9UcXpa8"
creator: "@howtowebdev"
platform: "tiktok"
category: "optiplan"
relevance: 4
date_processed: "2026-04-29"
tags: ["claude-code", "ai-agents", "claude-md", "prompt-engineering", "developer-workflow", "coding-best-practices"]
---

## תקציר

ה-repo הוא קובץ CLAUDE.md יחיד שנוצר על ידי Forrest Chang מתוך תצפיות של Andrej Karpathy על כשלים נפוצים של LLM בכתיבת קוד. הוא מכיל 4 עקרונות שמאלצים את סוכן ה-AI לחשוב לפני שכותב, לשמור על פשטות, לנהל diffs נקיים, ולעבוד לפי קריטריוני הצלחה מוגדרים. ניתן להוסיף אותו לכל פרויקט קיים תוך דקה ולהתאים אותו להנחיות ספציפיות לפרויקט.

## תובנות מפתח

- הקובץ מיועד ל-Claude Code אך עובד גם עם Cursor — ניתן להשתמש בו בכל הפרויקטים הפעילים (OptiPlan, TaylorPlayed)
- העיקרון המרכזי: במקום לתת לסוכן פקודות אימפרטיביות, מגדירים קריטריוני הצלחה דקלרטיביים ומאפשרים לו לרוץ עד שהם מתקיימים (Goal-Driven Execution)
- עיקרון ה-simplicity-first מונע over-engineering: אסור להוסיף features שלא התבקשו, abstractions לשימוש חד-פעמי, או error handling לתרחישים שלא יקרו
- הקובץ תוכנן להתמזג עם הנחיות ספציפיות לפרויקט — ניתן להוסיף בסוף TypeScript strict mode, פקודות טסטים, ודפוסי error handling של OptiPlan
- רלוונטי גם ל-shalhevet כחומר הוראה מצוין לקורסי prompt engineering ו-AI literacy

## כלים וספריות

| שם | קישור | תיאור |
|---|---|---|
| [Claude Code](https://claude.ai/code) | https://claude.ai/code | סוכן קוד AI של Anthropic שקורא קודבייסים שלמים ומבצע שינויים אוטונומיים |
| [Cursor](https://cursor.com) | https://cursor.com | עורך קוד מבוסס AI שתומך בקובץ ה-.cursor/rules/karpathy-guidelines.mdc מאותו repo |

## ריפוזיטוריז

- https://github.com/forrestchang/andrej-karpathy-skills

## פריטי פעולה

- [ ] הוסף את ה-CLAUDE.md לפרויקט OptiPlan: echo "" >> CLAUDE.md && curl https://raw.githubusercontent.com/forrestchang/andrej-karpathy-skills/main/CLAUDE.md >> CLAUDE.md
- [ ] לאחר ההוספה, הוסף בסוף הקובץ section ספציפי ל-OptiPlan: TypeScript strict mode, פקודות NX, דפוסי Convex ו-Clerk
- [ ] שקול להוסיף גם ל-TaylorPlayed עם section ספציפי ל-Firebase ו-React 19
- [ ] בדוק את קובץ CURSOR.md ב-repo כדי להגדיר את אותן הנחיות גם ב-Cursor

## הערות אימות

- ⚠️ מספר ה-stars שצוין בסרטון אינו מדויק (הסרטון אמר 'Andre' במקום 'Andrej' — שגיאת תמלול) — לפי מקורות שונים מדובר ב-30k–43k+ stars, המספר משתנה
- ⚠️ טענת הסרטון שה-repo 'מיועד לסוכני קוד AI בכלל' נכונה, אך הקובץ מותאם בראש ובראשונה ל-Claude Code — שימוש עם סוכנים אחרים עשוי לדרוש התאמות

