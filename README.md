# אריאל גולן מוביס

אפליקציית RTL ניידת לקטלוג ZOVEX, עם חיפוש, קטגוריות, סדרות/עונות/פרקים, דפי פרטים, נגן פנימי וממשק ניהול מאובטח בצד השרת.

## פריסה ב-Render

- Build command: ריק
- Start command: `npm start`
- Environment:
  - `ADMIN_PASSWORD` - סיסמת המנהל
  - `SESSION_SECRET` - מחרוזת אקראית ארוכה
  - `GITHUB_TOKEN` - Fine-grained token עם Contents read/write ל-repo
  - `GITHUB_REPO` - `boherbatov/zovex-flow`
  - `CATALOG_URL` - אופציונלי, ברירת מחדל `https://zovex.duckdns.org/movies.json`

הקטלוג נטען ישירות מ-ZOVEX בזמן עליית השרת ואינו חייב להישמר ב-repo. עריכות נשמרות כ-overlay קטן ב-`data/overrides.json` דרך GitHub API. סיסמת האדמין קיימת רק ב-Render environment ולא בקוד הדפדפן.
