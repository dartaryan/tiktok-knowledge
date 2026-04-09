---
title_he: "Graphify — כלי Claude Code לבניית גרף ידע אינטראקטיבי מקוד, PDFs וצילומי מסך"
title_en: "Graphify — Claude Code Skill That Turns Any Folder Into a Queryable Knowledge Graph"
source: "https://vt.tiktok.com/ZSH9pyA58"
creator: "@github.awesome"
platform: "tiktok"
category: "optiplan"
relevance: 3
date_processed: "2026-04-09"
tags: ["knowledge-graph", "claude-code", "codebase-navigation", "ai-tooling", "developer-productivity", "local-llm"]
---

## תקציר

Graphify הוא skill עבור Claude Code (ועוד AI coding assistants) שקורא כל תוכן בתיקייה — קוד, Markdown, PDFs, תמונות — ובונה ממנו גרף ידע ויזואלי, Obsidian vault, wiki בסגנון ויקיפדיה, ו-GRAPH_REPORT.md עם 'god nodes' וחיבורים מפתיעים. הכלי רץ לוקאלית לחלוטין ללא שרת חיצוני, ומשתמש ב-Tree-sitter ו-NetworkX לחילוץ מבנה מ-19 שפות תכנות. יכול להיות שימושי במיוחד לניווט ב-NX monorepo מורכב של optiplan.

## תובנות מפתח

- הטענה על חיסכון של 71.5x ב-tokens היא מדויקת רק עבור corpus של 52+ קבצים — ב-corpus קטן, הערך הוא בהירות מבנית ולא חיסכון בטוקנים
- כל קשר בגרף מסומן EXTRACTED / INFERRED / AMBIGUOUS — כך ה-AI יודע מה נמצא לעומת מה שנוסק
- ניתן להתקין git hook (graphify hook install) שמאחזר את הגרף אוטומטית אחרי כל commit — שימושי ב-NX monorepo עם שינויים תכופים
- ה-wiki mode (--wiki) מייצר מאמרים בסגנון ויקיפדיה עם index.md — agent יכול לנווט בידע בלי לפרסר JSON
- הכלי פורסם לפני מספר ימים בלבד — עדיין מוקדם מאוד, כדאי לעקוב אחרי בשלות

## כלים וספריות

| שם | קישור | תיאור |
|---|---|---|
| [Graphify](https://github.com/safishamsi/graphify) | https://github.com/safishamsi/graphify | Claude Code skill לבניית גרף ידע מרובה-מודאלי מקוד, מסמכים ותמונות — רץ לוקאלית |
| [Graphify (PyPI)](https://graphify.net/) | https://graphify.net/ | אתר הבית של Graphify עם הוראות התקנה דרך pip install graphifyy |
| [Claude Code](https://docs.anthropic.com/en/docs/claude-code) | https://docs.anthropic.com/en/docs/claude-code | סביבת הפיתוח הראשית שבה Graphify פועל כ-skill |
| [NetworkX](https://networkx.org/) | https://networkx.org/ | ספריית Python לבניית וניתוח גרפים — בשימוש פנימי של Graphify |
| [Tree-sitter](https://tree-sitter.github.io/tree-sitter/) | https://tree-sitter.github.io/tree-sitter/ | פרסר AST (עץ תחביר) תומך 19 שפות — מאפשר ל-Graphify להבין קוד ברמה מבנית |

## ריפוזיטוריז

- https://github.com/safishamsi/graphify

## פריטי פעולה

- [ ] הרץ pip install graphifyy && graphify install ואז /graphify על תיקיית הפרויקט של optiplan כדי לזהות god nodes ו-dependencies מסובכים ב-NX monorepo
- [ ] נסה את --wiki flag לייצר wiki index שאפשר לתת ל-AI agent כנקודת כניסה לניווט בקוד
- [ ] שקול להתקין את git hook (graphify hook install) כדי שהגרף יתעדכן אוטומטית אחרי כל commit

## הערות אימות

- ⚠️ הטענה של '71.5x fewer tokens' מאומתת בקוד המקור, אך תקפה רק ב-52+ קבצים — ב-corpus קטן יותר אין חיסכון בטוקנים, רק בהירות מבנית
- ⚠️ הכלי פורסם לפני 2-3 ימים בלבד — ייתכן שיש bugs ו-edge cases לא מתועדים, לא מתאים לסביבת production עדיין

