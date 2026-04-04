---
title_he: "Lenis — ספריית Smooth Scroll קלילה עם אינטגרציה ל-GSAP"
title_en: "Lenis — Lightweight Smooth Scroll Library with GSAP Integration"
source: "https://vt.tiktok.com/ZSHBdEyCx"
creator: "@howtowebdev"
platform: "tiktok"
category: "taylor-played"
relevance: 2
date_processed: "2026-04-04"
tags: ["smooth-scroll", "lenis", "gsap", "animation", "frontend", "parallax"]
---

## תקציר

הסרטון מציג את Lenis (שגוי כ-'Linus' בתמלול), ספריית smooth scrolling קלילה ובעלת ביצועים גבוהים המיועדת לפרונט-אנד מודרני. היא תומכת באפקטי parallax, שומרת על נגישות ומסתנכרנת עם ScrollTrigger של GSAP לאנימציות גלילה חלקות. רלוונטית לממשקי משתמש consumer-facing כמו TaylorPlayed שדורשים חוויה ויזואלית פרימיום.

## תובנות מפתח

- Lenis היא ספריית ה-smooth scroll המובילה לווב — קלילה, ביצועיסטית ונגישה, בשימוש סוכנויות מובילות ברחבי העולם
- האינטגרציה עם GSAP ScrollTrigger מתבצעת על ידי חיבור lenis.on('scroll', ScrollTrigger.update) והוספת lenis.raf לתוך gsap.ticker
- בניגוד ל-GSAP ScrollSmoother (שדורש רישיון מסחרי), Lenis היא open source — יתרון משמעותי לפרויקטים עצמאיים
- ספריות מתחרות כוללות GSAP ScrollSmoother ו-Locomotive Scroll; Lenis נחשבת הקלילה והנגישה ביותר מבין השלוש
- רלוונטי גם ל-optiplan אם נוספות אנימציות scroll לדשבורד הפרויקטים בעתיד

## כלים וספריות

| שם | קישור | תיאור |
|---|---|---|
| [Lenis](https://lenis.dev) | https://lenis.dev | ספריית smooth scroll קלילה ונגישה, תומכת ב-GSAP ScrollTrigger ו-parallax |
| [GSAP](https://gsap.com) | https://gsap.com | ספריית אנימציית JavaScript מובילה, כוללת ScrollTrigger ו-ScrollSmoother |

## ריפוזיטוריז

- https://github.com/darkroomengineering/lenis

## פריטי פעולה

- [ ] שקול להוסיף Lenis לממשק ה-consumer של TaylorPlayed לחוויית גלילה חלקה ופרימיום בדפי המוצר
- [ ] בדוק את תיעוד האינטגרציה של Lenis עם GSAP ScrollTrigger ב-https://github.com/darkroomengineering/lenis לפני שילוב בפרויקט

## הערות אימות

- ⚠️ בתמלול נכתב 'Linus' — ככל הנראה שגיאת תמלול אוטומטי; הכוונה ל-'Lenis' (מאושר על ידי חיפוש)
- ⚠️ הטענה 'plays perfectly with GSAP animations' — האינטגרציה מצריכה הגדרה ידנית של ticker ו-ScrollTrigger, לא plug-and-play אוטומטי

