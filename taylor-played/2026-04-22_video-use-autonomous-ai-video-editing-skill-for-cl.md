---
title_he: "video-use: עריכת וידאו אוטונומית עם Claude Code"
title_en: "video-use: Autonomous AI Video Editing Skill for Claude Code"
source: "https://vt.tiktok.com/ZS98ybdPh"
creator: "@howtowebdev"
platform: "tiktok"
category: "taylor-played"
relevance: 3
date_processed: "2026-04-22"
tags: ["claude-code", "video-editing", "open-source", "ai-agent", "content-creation", "automation"]
---

## תקציר

video-use הוא כלי קוד-פתוח שפועל כ-skill בתוך Claude Code ומאפשר עריכת וידאו אוטונומית באמצעות שפה טבעית. מספיק לזרוק תיקייה של צילומים גולמיים — הכלי חותך מילות מילוי, מוסיף כתוביות, מבצע color grading אוטומטי ומייצר אנימציות. רלוונטי ל-TaylorPlayed ליצירת תוכן שיווקי ווידאו מוצר ללא עורך וידאו ייעודי.

## תובנות מפתח

- הכלי משתמש בארכיטקטורת שתי שכבות: שכבת טקסט (transcript + EDL) ושכבת ויזואל (PNG על-פי-דרישה) — ה-LLM אף פעם לא מעבד פריימים גולמיים, מה שחוסך עשרות מיליוני טוקנים
- הכלי מבצע self-evaluation אוטומטי בכל נקודת חיתוך לפני שמציג תוצאה — מה שמפחית שגיאות ידניות
- התקנה פשוטה: clone + symlink לתוך ספריית ה-skills של Claude Code (~/.claude/skills/video-use)
- שימושי ל-TaylorPlayed ליצירת וידאו שיווקי (unboxing, demos, social content) ללא עורך וידאו — הקשר משני: גם ל-shalhevet ליצירת תוכן הדרכה

## כלים וספריות

| שם | קישור | תיאור |
|---|---|---|
| [video-use](https://github.com/browser-use/video-use) | https://github.com/browser-use/video-use | Claude Code skill קוד-פתוח לעריכת וידאו אוטונומית: הסרת מילות מילוי, color grading, כתוביות ואנימציות |
| [Claude Code](https://docs.anthropic.com/en/docs/claude-code) | https://docs.anthropic.com/en/docs/claude-code | סביבת קוד אג'נטית של Anthropic — הכלי פועל בתוכה כ-skill |

## ריפוזיטוריז

- https://github.com/browser-use/video-use

## פריטי פעולה

- [ ] לבדוק את video-use ל-TaylorPlayed: לנסות ליצור סרטון unboxing/demo של משחק לוח מתיקיית צילומים גולמיים
- [ ] לבצע: git clone https://github.com/browser-use/video-use ולקשר ל-~/.claude/skills/video-use
- [ ] לבחון שימוש ב-video-use לייצור תוכן שיווקי לרשתות חברתיות עבור TaylorPlayed ללא עורך וידאו חיצוני

## הערות אימות

- ⚠️ הטרנסקריפט אומר 'cloud code' — ברור שמדובר ב-Claude Code (שגיאת תמלול אוטומטי)
- ⚠️ טענת 'color grading אוטומטי' ו-'animation overlays' מאומתות בקוד הפתוח (Manim/Remotion/PIL) — נראה אמין
- ⚠️ הכלי מ-browser-use org — אותה ארגון כמו כלי האוטומציה של דפדפן; לא בדיוק אותו צוות אך תחת אותו GitHub org

