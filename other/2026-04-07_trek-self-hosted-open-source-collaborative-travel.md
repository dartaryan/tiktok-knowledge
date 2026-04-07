---
title_he: "TREK — פלטפורמת תכנון טיולים קולאבורטיבית ופתוחה לאחסון עצמי"
title_en: "TREK — Self-Hosted Open Source Collaborative Travel Planner"
source: "https://vt.tiktok.com/ZSH5bndRB"
creator: "@howtowebdev"
platform: "tiktok"
category: "other"
relevance: 2
date_processed: "2026-04-07"
tags: ["self-hosted", "open-source", "travel-planning", "mcp", "docker", "real-time-collaboration"]
---

## תקציר

TREK הוא כלי קוד פתוח (AGPL-3.0) לתכנון טיולים קבוצתיים, המאפשר שיתוף פעולה בזמן אמת, מפות אינטראקטיביות, ניהול תקציב ורשימות אריזה — הכל על שרת פרטי. הכלי נפרס דרך Docker ותומך ב-SSO, 2FA ו-PWA להתקנה ישירה מהדפדפן. נקודת עניין: יש לו אינטגרציית MCP המאפשרת לחבר אליו Claude Desktop ולנהל טיולים שלמים בשפה טבעית.

## תובנות מפתח

- TREK תומך באינטגרציית MCP (Model Context Protocol) — ניתן לחבר אליו Claude Desktop ולהורות לו בשפה טבעית ליצור טיולים, הוסיף מקומות, תקציב ורשימות אריזה ישירות בתוך הפלטפורמה
- הפרויקט מדגים דפוס ה-self-hosted SaaS עם Docker + SQLite + WebSocket לסינכרון בזמן אמת — דפוס ארכיטקטוני שרלוונטי לעיצוב optiplan או taylor-played
- 3,300+ כוכבים ב-GitHub תוך שבוע — פרויקט חם מאוד, רלוונטי להדגמה בהדרכות shalhevet בנושא MCP ואינטגרציות AI עם כלים חיצוניים

## כלים וספריות

| שם | קישור | תיאור |
|---|---|---|
| [TREK](https://github.com/mauriceboe/TREK) | https://github.com/mauriceboe/TREK | פלטפורמת תכנון טיולים קולאבורטיבית, self-hosted, עם מפות, תקציב, PWA ו-MCP |
| [Leaflet](https://leafletjs.com) | https://leafletjs.com | ספריית מפות אינטראקטיביות קוד פתוח — בשימוש ב-TREK לויזואליזציה של מסלולים |
| [Open-Meteo](https://open-meteo.com) | https://open-meteo.com | API תחזיות מזג אוויר חינמי (ללא מפתח API) — מספק תחזית 16 יום ב-TREK |

## ריפוזיטוריז

- https://github.com/mauriceboe/TREK

## פריטי פעולה

- [ ] אם רוצים להדגים אינטגרציית MCP עם Claude בהדרכות shalhevet — TREK הוא דוגמה חיה ומרשימה: להגדיר instance ל-demo ולהראות יצירת טיול שלם בשפה טבעית
- [ ] לשמור כהפניה לדפוס Docker + SQLite + WebSocket לפרויקטים עתידיים הדורשים self-hosting מהיר

## הערות אימות

- ⚠️ הסרטון מציין תכונות בסיסיות בלבד — בפועל הכלי עשיר הרבה יותר (MCP, SSO, 2FA, PDF export) שלא הוזכרו כלל

