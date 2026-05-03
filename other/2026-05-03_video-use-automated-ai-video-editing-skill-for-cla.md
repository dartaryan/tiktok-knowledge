---
title_he: "Video-Use: כלי עריכת וידאו אוטומטי מבוסס Claude Code"
title_en: "Video-Use: Automated AI Video Editing Skill for Claude Code"
source: "https://vt.tiktok.com/ZS9x7e1wS"
creator: "@creativelyange"
platform: "tiktok"
category: "other"
relevance: 2
date_processed: "2026-05-03"
tags: ["claude-code", "video-editing", "ai-automation", "browser-use", "content-creation"]
---

## תקציר

Video-Use הוא כלי קוד פתוח מבית browser-use המאפשר לשחרר קטעי וידאו לתוך תיקייה, ואז Claude Code (שהיוצרת קוראת לו 'Cloud Code') מבצע את העריכה ומפיק קובץ final.mp4 מוכן. הכלי עובד דרך תמלול אודיו (ElevenLabs) ומבצע חיתוכים על בסיס גבולות מילים, הסרת מילות מילוי, והוספת כתוביות. הטענות על color grading, פילטרים ואנימציות מוטלות בספק לאור תיעוד ה-repo האמיתי.

## תובנות מפתח

- הכלי אינו 'צופה' בוידאו — הוא קורא את התמלול בשתי שכבות: transcript עם timestamps ברמת מילה + תמונות on-demand, בדומה לגישת browser-use ל-DOM
- לאחר עריכה ראשונית, הכלי מריץ self-evaluation loop שבוחן כל גבול חיתוך ומתקן קפיצות ויזואליות, pops אודיו, וכתוביות חסויות — לפני שמציג תצוגה מקדימה
- קיימים לפחות 3-4 כלים מתחרים נוספים ב-GitHub לעריכת וידאו עם Claude Code: buttercut, claude-code-video-toolkit (digitalsamba), ו-claude-video-vision
- רלוונטי בעיקר למי שמייצר תוכן וידאו שיווקי — ייתכן שימוש עתידי ב-taylor-played ליצירת סרטוני מוצר לפרסום

## כלים וספריות

| שם | קישור | תיאור |
|---|---|---|
| [video-use](https://github.com/browser-use/video-use) | https://github.com/browser-use/video-use | כלי עריכת וידאו אוטומטי המשתלב כ-skill ב-Claude Code / Codex — שולט קלטת לתיקייה ומקבל final.mp4 |
| [Claude Code](https://claude.ai/code) | https://claude.ai/code | סביבת קידוד אוטונומית של Anthropic — בסיס ההרצה לכלי video-use |
| [ElevenLabs Scribe](https://elevenlabs.io/scribe) | https://elevenlabs.io/scribe | מנוע תמלול אודיו עם timestamps ברמת מילה ו-speaker diarization — נדרש לתפקוד video-use |
| [Remotion](https://www.remotion.dev) | https://www.remotion.dev | ספריית יצירת וידאו פרוגרמטי ב-React — הכלי שהוזכר כנחות ב-TikTok, אך בפועל משמש בכלים אחרים בתחום |
| [ffmpeg](https://ffmpeg.org) | https://ffmpeg.org | כלי עיבוד מולטימדיה בקוד פתוח — dependency חובה של video-use |

## ריפוזיטוריז

- https://github.com/browser-use/video-use

## הערות אימות

- ⚠️ הטענה על 'color grading, filters, animations' — תיעוד ה-repo האמיתי אינו מאזכר יכולות אלו; הכלי מתמקד בחיתוך מבוסס-transcript, הסרת fillers וכתוביות. ייתכן הגזמה של היוצרת
- ⚠️ הטענה ש-video-use 'עדיף על Remotion' — השוואה לא הוגנת: Remotion הוא framework ליצירת וידאו פרוגרמטי, video-use הוא כלי לעריכת footage קיים — שני שימושים שונים
- ⚠️ 'Cloud Code' בטרנסקריפט = Claude Code (שגיאת הגייה של היוצרת)

