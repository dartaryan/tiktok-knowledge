---
title_he: "Open Design — חלופה קוד-פתוח מקומית ל-Claude Design של Anthropic"
title_en: "Open Design — Local-First Open-Source Alternative to Anthropic's Claude Design"
source: "https://vt.tiktok.com/ZS9Uud3FN"
creator: "@github.awesome"
platform: "tiktok"
category: "taylor-played"
relevance: 3
date_processed: "2026-04-29"
tags: ["open-source", "ui-generation", "claude-design", "local-first", "design-tools", "prototyping"]
---

## תקציר

הסרטון מציג את Open Design, כלי קוד-פתוח ומקומי-ראשוני (local-first) שמחקה את Claude Design של Anthropic — ממשק ייצור UI מבוסס-פרומפטים שרץ בטרמינל. הכלי מתחבר ל-Claude Code, Cursor, Codex, Gemini CLI, OpenCode ו-Qwen, מציג 19 מיומנויות עיצוב ו-71 מערכות עיצוב מותגיות, ומייצא HTML, PDF ו-PowerPoint. ה-'LocalQuen' שנשמע בתמלול הוא ככל הנראה Qwen Code — מודל שפה מקומי של Alibaba.

## תובנות מפתח

- שני פרויקטים נפרדים קיימים: nexu-io/open-design (web app + local daemon, 19 skills, 71 design systems) ו-OpenCoworkAI/open-codesign (אפליקציית Electron, 12 skills) — הסרטון מתייחס ל-nexu-io/open-design לפי המספרים המדויקים
- הכלי לא מכיל agent משלו — הוא מאציל לסוכני הקוד הקיימים במחשב (Claude Code, Cursor, Codex, Gemini CLI, OpenCode, Qwen Code) דרך daemon מקומי
- ייצוא ל-HTML (CSS מוטמע), PDF, PPTX, ZIP ו-Markdown — שימושי ל-TailorPlayed עבור דפי נחיתה, דקים שיווקיים ואבות-טיפוס מוצר
- רלוונטי גם ל-optiplan: הכלי כולל skill-modules לדשבורדים, טבלאות נתונים ודפי תמחור — שיכולים לשמש לגנרציה מהירה של mockups עבור ה-SaaS

## כלים וספריות

| שם | קישור | תיאור |
|---|---|---|
| [Open Design (nexu-io)](https://github.com/nexu-io/open-design) | https://github.com/nexu-io/open-design | חלופה קוד-פתוח מקומית ל-Claude Design — web app + local daemon, 19 design skills, 71 brand design systems |
| [Claude Design (Anthropic)](https://claude.ai/design) | https://claude.ai/design | כלי עיצוב UI מבוסס-פרומפט של Anthropic, מבוסס על Claude Opus 4.7 — סגור, בתשלום, ענן בלבד |
| [Open CoDesign](https://github.com/OpenCoworkAI/open-codesign) | https://github.com/OpenCoworkAI/open-codesign | חלופה קוד-פתוח נוספת ל-Claude Design — אפליקציית Electron, BYOK, multi-model, 12 design skills |
| [Claude Code](https://claude.ai/code) | https://claude.ai/code | סוכן קידוד CLI של Anthropic — אחד מסוכני ה-CLI שאליהם מתחבר Open Design |
| [OpenCode](https://opencode.ai) | https://opencode.ai | סוכן קידוד CLI קוד-פתוח (MIT), תומך ב-75+ ספקים, מבוסס TUI — מתחבר ל-Open Design |
| [Gemini CLI](https://github.com/google-gemini/gemini-cli) | https://github.com/google-gemini/gemini-cli | CLI של Google עבור מודלי Gemini — אחד מסוכני ה-CLI הנתמכים |
| [Cursor](https://cursor.com) | https://cursor.com | עורך קוד מבוסס-AI — נתמך כ-agent ב-Open Design |
| [Qwen Code (Qwen CLI)](https://github.com/QwenLM/qwen-code) | https://github.com/QwenLM/qwen-code | סוכן CLI של Alibaba עבור מודלי Qwen — זוהי ככל הנראה ה-'LocalQuen' מהתמלול |

## ריפוזיטוריז

- https://github.com/nexu-io/open-design

## פריטי פעולה

- [ ] נסה את nexu-io/open-design עם Claude Code ליצירת mockup מהיר לדף נחיתה של TailorPlayed — ייצא HTML ישירות לתוך ה-Vite project
- [ ] בדוק את ה-skill module של דשבורדים ב-Open Design ליצירת אב-טיפוס מהיר לממשקי optiplan (data tables, dashboards)

## הערות אימות

- ⚠️ 'LocalQuen' בתמלול הוא טעות תמלול — על פי ה-repo הרשמי מדובר ב-Qwen (ספציפית Qwen Code של Alibaba), לא בכלי בשם LocalQuen
- ⚠️ הסרטון מציין '19 design skills' ו-'71 brand-grade design systems' — מאומת מול ה-README של nexu-io/open-design
- ⚠️ הפרויקט בגרסה מוקדמת מאוד (v0.1.x בעת פרסום) — ייתכנו שינויים מהירים ב-API ובתכונות

