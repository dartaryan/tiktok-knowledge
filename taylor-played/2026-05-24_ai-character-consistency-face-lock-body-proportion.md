---
title_he: "עקביות דמויות ב-AI: נעילת פנים, פרופורציות ו-Continuity Pipelines"
title_en: "AI Character Consistency: Face Lock, Body Proportions, and Continuity Pipelines for Multi-Scene Generation"
source: "https://www.instagram.com/reel/DYTelGfyWaO/?igsh=MXRuMmQ5cjN4enVrdA=="
creator: "@Jamie Heinrich"
platform: "instagram"
category: "taylor-played"
relevance: 3
date_processed: "2026-05-24"
tags: ["ai-image-generation", "character-consistency", "face-lock", "lora", "board-game-art", "continuity-pipeline"]
---

## תקציר

סרטון פרסומי קומי של Jamie Heinrich המקדם קורס בנושא יצירת סרטים ב-AI ($5/חודש). הנקודה המרכזית: כלי AI מייצרים פנים שונות בכל רנדר ונדרשת שיטת 'נעילה' מראש — בניית master character sheet עם זוויות פרונטל ופרופיל, נעילת Face ID, פרופורציות גוף ו-Outfit IDs, ולאחר מכן שימוש חוזר באותה דמות בכל סצנה. הטכניקות רלוונטיות גם ליצירת artwork עקבי לרכיבי משחקי לוח (קלפים, קופסא, חוברת כללים) ב-taylor-played.

## תובנות מפתח

- הבעיה: כלי AI 'ממציאים מחדש' את פני הדמות בכל ג'נרציה במקום לשמור על זהות קבועה — כל רנדר מייצר אדם אחר
- הפתרון המרכזי: בנה master character sheet עם זוויות front, 3/4 ו-side לפני ההפקה, ונעל Face ID, פרופורציות גוף ו-Outfit IDs
- לפי מחקר: LoRA training על 15-30 תמונות רפרנס משיג 85-95% שמירת פיצ'רים; reference image conditioning (IP-Adapter) מתאים לפרויקטים קצרים של 5-10 תמונות לפני שיש drift
- לטיילור פלייד: ישירות ישים לייצור artwork עקבי לקלפים, חוברות כללים ואריזה — אותה דמות על עשרות רכיבי משחק דורשת continuity pipeline מסודר
- Midjourney תומך ב-parameter --cref להוספת reference image לשמירת עקביות פנים; Ideogram Character מאפשר נעילה מתמונה בודדת

## כלים וספריות

| שם | קישור | תיאור |
|---|---|---|
| [Jamie Heinrich AI Filmmaking Course (Skool)](https://www.skool.com/@jamie-heinrich) | https://www.skool.com/@jamie-heinrich | קורס $5/חודש על יצירת סרטים ב-AI עם דגש על עקביות דמויות — הכלי שמפורסם בסרטון |
| [Ideogram Character](https://ideogram.ai/features/character/) | https://ideogram.ai/features/character/ | כלי לנעילת פנים דמות מתמונת רפרנס אחת — שומר על identity אחיד גם בשינוי תנוחה, תלבושת ותאורה |
| [IP-Adapter](https://huggingface.co/h94/IP-Adapter) | https://huggingface.co/h94/IP-Adapter | אדפטר ל-Stable Diffusion שמזריק תמונת רפרנס לתהליך הג'נרציה לשמירת עקביות פנים ללא אימון |
| [OpenArt](https://openart.ai) | https://openart.ai | פלטפורמת AI image generation עם Character Profiles — שומר פרופיל דמות וממחיל אותו על כל ג'נרציה עתידית |

## פריטי פעולה

- [ ] לפני יצירת artwork לדמויות משחקי לוח ב-taylor-played: בנה master character sheet עם תמונות front, 3/4 ו-side view בתאורה ניטרלית
- [ ] נסה Ideogram Character (ideogram.ai) לנעילת פנים מתמונת רפרנס אחת — ישים לדמויות על קלפים וחוברות כללים
- [ ] לעקביות לטווח ארוך בין עשרות רכיבי משחק: שקול LoRA training על 15-25 תמונות רפרנס של כל דמות
- [ ] אם משתמשים ב-Midjourney: הוסף --cref [URL לתמונת רפרנס] לכל פרומפט לשמירת עקביות פנים בין סצנות

## הערות אימות

- ⚠️ הסרטון הוא תוכן פרסומי קומי — לא מציג הדגמה טכנית ולא מזכיר כלי ספציפי בשמו; כל הטכניקות הן בגדר 'כותרות' בלבד
- ⚠️ האתר של הקורס מזהיר שהמחיר עשוי לעלות מ-$5 ל-$50/חודש בקרוב — המחיר הנוכחי לא מובטח

