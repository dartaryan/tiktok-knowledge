---
title_he: "עריכת וידאו שיחתית עם Claude Code — הכלי video-use של Browser Use"
title_en: "Conversational AI Video Editing with Claude Code — browser-use/video-use"
source: "https://vt.tiktok.com/ZS9Apr7Fy"
creator: "@creativelyange"
platform: "tiktok"
category: "other"
relevance: 2
date_processed: "2026-04-28"
tags: ["claude-code", "video-editing", "ai-agents", "open-source", "browser-use", "content-creation"]
---

## תקציר

הצוות מאחורי Browser Use שחרר כלי קוד-פתוח בשם video-use, המאפשר עריכת וידאו מלאה דרך שיחה עם Claude Code: מזרוקים קליפים גולמיים לתיקייה, מבקשים בשפה טבעית, ומקבלים final.mp4. הכלי מבצע חיתוך מילים מיותרות, color grading אוטומטי, הוספת כתוביות ואנימציות, ומעריך את עצמו בזמן ריצה. עשוי להיות שימושי ליצירת תוכן שיווקי עבור taylor-played או כדוגמה ל-Claude Code בהדרכות shalhevet.

## תובנות מפתח

- הכלי עובד כ-skill של Claude Code — לא אפליקציה עצמאית אלא הרחבה לסביבת AI coding agent קיימת
- עריכת וידאו מבוססת על קריאת transcript (ElevenLabs Scribe) ולא על ניתוח ויזואלי — ה-LLM לא 'רואה' את הוידאו
- תומך ביצירת אנימציות דרך Manim, Remotion, או PIL בתהליכי sub-agents מקבילים
- זיכרון סשן נשמר ב-project.md — מאפשר המשכיות בין עריכות שונות
- רלוונטי משנית ל-taylor-played: יצירת סרטוני שיווק ל-board game studio, ול-shalhevet: הדגמת יכולות Claude Code בסדנאות

## כלים וספריות

| שם | קישור | תיאור |
|---|---|---|
| [video-use](https://github.com/browser-use/video-use) | https://github.com/browser-use/video-use | כלי עריכת וידאו קוד-פתוח המופעל דרך Claude Code — עריכה שיחתית לקובץ MP4 סופי |
| [Claude Code](https://docs.anthropic.com/en/docs/claude-code) | https://docs.anthropic.com/en/docs/claude-code | סביבת AI coding agent של Anthropic שדרכה מופעל video-use (נזכר בתמלול כ'Cloud Code' — שגיאת שמע) |
| [ElevenLabs Scribe](https://elevenlabs.io) | https://elevenlabs.io | שירות תמלול (בתשלום) הנדרש לניתוח וורד-לוול של הוידאו — dependency חובה |
| [ffmpeg](https://ffmpeg.org) | https://ffmpeg.org | כלי מולטימדיה קוד-פתוח — dependency חובה לעיבוד הוידאו |
| [Manim](https://www.manim.community) | https://www.manim.community | ספריית Python ליצירת אנימציות מתמטיות — בשימוש ליצירת overlays |
| [Remotion](https://www.remotion.dev) | https://www.remotion.dev | ספריית React ליצירת וידאו פרוגרמטית — בשימוש ליצירת אנימציות |

## ריפוזיטוריז

- https://github.com/browser-use/video-use

## פריטי פעולה

- [ ] לבדוק את video-use לצורך יצירת סרטוני הדגמה שיווקיים עבור taylor-played — התקנה: git clone + uv sync + brew install ffmpeg
- [ ] לרשום כדוגמה ל-shalhevet: video-use כהמחשה של multi-agent workflows עם Claude Code בסדנאות AI
- [ ] לוודא כי יש API key של ElevenLabs לפני ניסיון ראשון (נדרש לשלב התמלול)

## הערות אימות

- ⚠️ בתמלול נאמר 'Cloud Code' — כנראה שגיאת שמע, הכוונה ל-Claude Code של Anthropic
- ⚠️ בתמלול נאמר '3.9 stars on GitHub' — לא סביר; GitHub סופר כוכבים במספרים שלמים. כנראה הכוונה ל-3.9k stars, אך יש לאמת
- ⚠️ הטענה שה-agent 'self-evaluates and improves its own mistakes' דורשת בדיקה מעשית — ייתכן שמדובר בהערכה בגבולות חיתוכים בלבד לפי ה-README

