---
title_he: "TREK — מתכנן טיולים קבוצתיים self-hosted עם שיתוף פעולה בזמן אמת"
title_en: "TREK — Self-Hosted Group Trip Planner with Real-Time Collaboration"
source: "https://vt.tiktok.com/ZSHRxbBMk"
creator: "@github.awesome"
platform: "tiktok"
category: "other"
relevance: 1
date_processed: "2026-03-29"
tags: ["self-hosted", "travel", "pwa", "open-source", "real-time", "collaboration"]
---

## תקציר

TREK הוא כלי קוד פתוח לתכנון טיולים קבוצתיים, המתארח עצמאית (self-hosted) ומציע לוח זמנים בגרירה ושחרור, מפות אינטראקטיביות, מעקב אחר טיסות ותקציב, ורשימות אריזה. הכלי תומך בשיתוף פעולה בזמן אמת דרך WebSockets ומוגדר כ-PWA (Progressive Web App), כך שחברים יכולים להתקין אותו ישירות מהדפדפן ללא App Store. אינו רלוונטי לאף אחד מהפרויקטים הפעילים.

## תובנות מפתח

- הגישה של TREK לאפשר התקנת PWA ישירות מהדפדפן (ללא App Store) היא פטרן מעניין שעשוי לשמש השראה ל-taylor-played אם נרצה להנגיש את הפלטפורמה לנייד ללא פיתוח אפליקציה נפרדת
- הארכיטקטורה: Node.js 22 + Express + SQLite בצד שרת, WebSockets לסנכרון בזמן אמת — פשוטה ויעילה לפרויקטי צוות קטן
- תמיכה ב-SSO דרך OIDC (Google, Apple, Keycloak) — יכולה לשמש דוגמה ל-optiplan בנושא ניהול הרשאות ארגוניות

## כלים וספריות

| שם | קישור | תיאור |
|---|---|---|
| [TREK](https://github.com/mauriceboe/TREK) | https://github.com/mauriceboe/TREK | מתכנן טיולים קבוצתיים קוד פתוח, self-hosted, עם מפות, תקציב, רשימות אריזה ו-PWA |

## ריפוזיטוריז

- https://github.com/mauriceboe/TREK

## הערות אימות

- ⚠️ הטענה שחברים יכולים להתקין את האפליקציה ישירות לטלפון ללא App Store — מאומתת: TREK היא PWA תקנית המשתמשת ב-Service Worker דרך Workbox, ותואמת iOS ו-Android

