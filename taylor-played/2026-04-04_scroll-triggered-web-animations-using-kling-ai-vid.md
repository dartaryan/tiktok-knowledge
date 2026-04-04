---
title_he: "אנימציית גלילה לאתרים: Kling AI + Claude Code + WebP Frames"
title_en: "Scroll-Triggered Web Animations Using Kling AI Video + Claude Code Frame Extraction"
source: "https://vt.tiktok.com/ZSHS1d9K5"
creator: "@chase_ai_"
platform: "tiktok"
category: "taylor-played"
relevance: 3
date_processed: "2026-04-04"
tags: ["scroll-animation", "webp", "claude-code", "kling-ai", "web-animation", "ui-effects"]
---

## תקציר

הסרטון מציג טכניקה ליצירת אנימציות גלילה מרשימות לאתרים: יוצרים שני frame-ים (התחלה וסוף), מחברים אותם לסרטון מעבר באמצעות Kling AI (כלי יצירת סרטוני AI), ואז משתמשים ב-Claude Code עם prompt מיוחד כדי לחלץ את כל ה-frame-ים לפורמט WebP וליישם אנימציית גלילה מבוססת-frame-ים. התוצאה היא אנימציית scroll חלקה ומרשימה ויזואלית שנשלטת לפי מיקום הגלילה של המשתמש. הטכניקה רלוונטית לדפי מוצר ב-TailorPlayed כגון אנימציית פריסת לוח משחק או פתיחת קופסה.

## תובנות מפתח

- הזרימה המלאה: תמונת-התחלה + תמונת-סוף ← Kling AI ← MP4 ← Claude Code (חילוץ frame-ים ל-WebP) ← scroll animation באתר
- ה-frame-ים לא מוטמעים כסרטון אלא כרצף תמונות WebP — מה שמאפשר שליטה מדויקת לפי מיקום הגלילה
- Claude Code מסוגל לקבל קובץ MP4 ישירות בתוך ה-prompt ולהתמודד עם כל לוגיקת חילוץ ה-frame-ים
- ה-prompt הספציפי שמנחה את Claude Code כיצד לבנות את ה-scroll animation אינו משותף בסרטון עצמו — זמין רק בקהילה של היוצר
- רלוונטי גם ל-optiplan: ניתן להשתמש בטכניקה דומה לאנימציות הסבר בדף הנחיתה של הפלטפורמה

## כלים וספריות

| שם | קישור | תיאור |
|---|---|---|
| [Claude Code](https://claude.ai/product/claude-code) | https://claude.ai/product/claude-code | כלי קידוד אגנטי של Anthropic שרץ בטרמינל, מסוגל לקרוא קבצים, להריץ פקודות ולממש לוגיקה מורכבת מהנחיות בשפה טבעית |
| [Kling AI](https://klingai.com) | https://klingai.com | כלי יצירת סרטוני AI של Kuaishou — מקבל תמונת-התחלה ותמונת-סוף ומייצר סרטון מעבר חלק ביניהן; מוזכר בסרטון כ-'Cling' |

## פריטי פעולה

- [ ] לחפש את ה-prompt המלא של @chase_ai_ דרך ה-bio שלו ב-TikTok ולשמור אותו לשימוש עתידי
- [ ] לנסות את הטכניקה עבור דף המוצר של TailorPlayed: ליצור frame התחלה (קופסת המשחק סגורה) וframe סוף (קופסה פתוחה עם רכיבים), לייצר סרטון ב-Kling AI, ולהעביר ל-Claude Code לצורך scroll animation
- [ ] לבדוק ש-Claude Code מותקן בסביבת הפיתוח: npm install -g @anthropic-ai/claude-code (או שיטות ההתקנה המעודכנות)

## הערות אימות

- ⚠️ בתמלול נאמר 'Cloud Code' — זו כנראה שמיעה שגויה של 'Claude Code' (כלי Anthropic)
- ⚠️ בתמלול נאמר 'Cling' — זהו ככל הנראה Kling AI (klingai.com), כלי יצירת סרטוני AI של Kuaishou
- ⚠️ ה-prompt הספציפי לא משותף בסרטון — רק ה-bio/קהילה של היוצר מכיל אותו; ייתכן שמדובר בגישה שיווקית לגיוס עוקבים

