---
title_he: "רשימת בדיקות לפני השקת אתר — אבטחה, תפעול וביצועים"
title_en: "Website Pre-Launch Security & Operations Checklist (10 Points)"
source: "https://www.instagram.com/reel/DWMXQJPgIrx/?igsh=MThrdmwxdnczOGJnOA=="
creator: "@Arjay McCandless"
platform: "instagram"
category: "optiplan"
relevance: 4
date_processed: "2026-03-28"
tags: ["security", "pre-launch", "saas", "devops", "authorization", "web-checklist"]
---

## תקציר

סרטון המציג 10 נקודות בדיקה קריטיות לפני השקת אפליקציית ווב לפרודקשן: אבטחה (Authorization, CORS, Rate Limiting, סינון קלטים), תפעול (Logging, Alerts, Rollback בגישת Blue-Green) וביצועים (אינדקסים ב-DB). הנקודות פרקטיות ומכסות את מרבית הסיכונים הנפוצים בהשקת SaaS. רלוונטי במיוחד לפני כל Release משמעותי של OptiPlan.

## תובנות מפתח

- Authorization — ודא שכל משתמש ניגש רק למשאבים שלו; ב-OptiPlan זה כולל בדיקת RBAC ו-multi-tenancy דרך Clerk כדי למנוע דליפה בין Organizations
- Rate Limiting — חיוני למניעת חיובים בלתי צפויים; ניתן להגדיר ב-Convex functions או ב-Vercel Edge Middleware
- Blue-Green Deployment — Vercel תומכת ב-instant rollback מובנה, כך שאין צורך בתשתית blue-green נפרדת; מספיק לוודא שה-Deployments הקודמים נשמרים
- Database Indexing — הוסף אינדקסים רק לשדות הנשאלים בתדירות גבוהה; ב-Convex מוגדרים אינדקסים ב-schema.ts ומשפיעים על write overhead
- Frontend Error Handling — השתמש ב-React Error Boundaries למניעת חשיפת Stack Traces גולמיים למשתמשי קצה
- Logging ממוקד — Convex מספקת Dashboard logs מובנה שמפחית את הצורך בכלי חיצוני יקר; ייעד logging לנתיבים קריטיים בלבד

## פריטי פעולה

- [ ] בנה Checklist פנימי ל-OptiPlan לפני כל Release: Authorization, Input Validation, CORS, Rate Limiting, Error Screens, DB Indexing, Logging, Alerts, Rollback
- [ ] בדוק שמדיניות Clerk RBAC מונעת גישה בין Organizations שונות ב-OptiPlan — בדיקת multi-tenant authorization
- [ ] הוסף Rate Limiting ל-Convex HTTP actions ו-public functions כדי למנוע ניצול לרעה
- [ ] ודא ש-React Error Boundaries מוגדרים ברמת ה-Router ו-feature boundaries ולא חושפים Stack Traces בפרודקשן
- [ ] עבור על אינדקסים ב-schema.ts של Convex וודא כיסוי מלא לשאילתות הנפוצות
- [ ] הגדר Alerts דרך Vercel או שירות כגון Sentry שיודיעו מיידית על שגיאות 5xx בפרודקשן

## הערות אימות

- ⚠️ הסרטון לא מציין כלים ספציפיים — כל ההמלצות עקרוניות ויש להתאים לכל Stack
- ⚠️ טיפ ה-Blue-Green Deployment רלוונטי יותר לשרתים עצמאיים; ב-Vercel ה-rollback מובנה ואינו דורש תשתית נפרדת

