---
title_he: "שלוש Claude Skills לשיפור עיצוב ממשק משתמש מבוסס AI"
title_en: "Three Claude Code Skills to Fix AI-Generated UI Design Slop"
source: "https://www.instagram.com/reel/DYnz1_qMIVv/?igsh=MTF3ZGc3M2dnaXozcA=="
creator: "@Marc Cleroux"
platform: "instagram"
category: "taylor-played"
relevance: 4
date_processed: "2026-05-24"
tags: ["claude-code", "skill-md", "ui-design", "anti-slop", "react", "tailwind", "motion-design"]
---

## תקציר

הסרטון מציג שלושה Claude Code Skills (קבצי SKILL.md) שנועדו לשפר את איכות העיצוב של ממשקים שנוצרים על ידי AI. הכלים פועלים ישירות בתוך Claude Code, Cursor וסביבות דומות, ומונעים פלט גנרי ואחיד ('AI slop'). רלוונטי במיוחד לפרויקט TaylorPlayed שמשתמש ב-React + Tailwind + DaisyUI לממשק צרכני.

## תובנות מפתח

- Taste Skill הוא framework אגנוסטי לסגנון עיצובי — עובד עם React, Vue, Svelte ואחרים — ומגדיר שלושה 'ידיות' מכווננות: DESIGN_VARIANCE, MOTION_INTENSITY, VISUAL_DENSITY (כל אחת בסקלה 1-10)
- Design Motion Principles (של Kyle Zantos — ולא 'Carl Zentos' כפי ששמע המציג) ממזג את גישות העיצוב של שלושה מעצבי תנועה ידועים: Emil Kowalski, Jakub Krehel ו-Jhey Tompkins — ומאפשר audit של אנימציות קיימות
- Impeccable של Paul Bakaus כולל כיום 23 פקודות (לא 18 כפי שנטען בסרטון — ייתכן שהסרטון הוצלם בגרסה ישנה יותר) ומסווג את הפרויקט ל-brand mode לעומת product mode לפני כל עיצוב
- כל שלושת הכלים ניתנים להתקנה בפקודת npx אחת ומשתמשים ב-SKILL.md portable format — תקן פתוח שתומך ב-Claude Code, Cursor, Codex, Gemini CLI ועוד
- רלוונטי גם ל-optiplan (React + TypeScript) לשיפור עיצוב דשבורדים ותצוגות נתונים

## כלים וספריות

| שם | קישור | תיאור |
|---|---|---|
| [Taste Skill](https://tasteskill.dev) | https://tasteskill.dev | קובצי SKILL.md שמונעים מ-AI לייצר ממשקים גנריים — כולל variants מרובים ו-image generation skills לשימוש עם ChatGPT Images |
| [Design Motion Principles](https://github.com/kylezantos/design-motion-principles) | https://github.com/kylezantos/design-motion-principles | Claude Code skill לאודיט ויצירת תנועה (אנימציות) בממשקים, מבוסס על גישות עיצוב של Emil Kowalski, Jakub Krehel ו-Jhey Tompkins |
| [Impeccable](https://impeccable.style) | https://impeccable.style | Claude Code skill עם 23 פקודות (/audit, /polish, /critique, /bolder, /quieter ועוד) ו-7 קבצי reference לעיצוב — נוצר על ידי Paul Bakaus, יוצר jQuery UI |

## ריפוזיטוריז

- https://github.com/Leonxlnx/taste-skill
- https://github.com/kylezantos/design-motion-principles
- https://github.com/pbakaus/impeccable

## פריטי פעולה

- [ ] הרץ `npx skills add https://github.com/Leonxlnx/taste-skill --skill design-taste-frontend` בפרויקט TaylorPlayed (React + Tailwind) ובדוק אם פלט Claude Code משתנה לממשק פחות גנרי
- [ ] הרץ `npx skills add https://github.com/pbakaus/impeccable` ואז `/teach-impeccable` כדי לשמור design context של TaylorPlayed (קהל יעד, אישיות מותג) ב-.impeccable.md
- [ ] הרץ `npx impeccable detect src/` (CLI עצמאי, ללא AI) לסריקת anti-patterns קיימים בממשק TaylorPlayed
- [ ] הרץ `npx skills add https://github.com/kylezantos/design-motion-principles` ובצע audit על אנימציות קיימות בפרויקט

## הערות אימות

- ⚠️ הסרטון מזכיר '18 commands' ל-Impeccable — אך הגרסה הנוכחית (v1.5.1+) כוללת 23 פקודות; ייתכן שהסרטון צולם בגרסה ישנה יותר
- ⚠️ שם היוצר של Design Motion Principles נשמע בסרטון כ-'Carl Zentos' אך GitHub מאשר שמו האמיתי הוא Kyle Zantos (kylezantos)
- ⚠️ הטענה ש-Taste Skill מתחבר ל-'ChatGPT's Image 2 model' — נכון חלקית: הכלי תומך ב-ChatGPT Images ו-Codex image mode אך אין התייחסות ספציפית ל-'Image 2' כמודל נפרד

