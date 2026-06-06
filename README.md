# qdrant-db-web

Public assets and GitHub Pages site for [Qdrant DB](https://marketplace.visualstudio.com/items?itemName=harishkaparwan.qdrant-db).

Live at: **https://harishkaparwan.github.io/qdrant-db-web/**

## Structure

```
index.html          ← Landing page (served at root)
app/                ← Built React workbench (populated by deploy:web)
public/
  assets/           ← Logo and static images
  policy/
    privacy.html    ← Privacy Policy
.github/workflows/
  deploy.yml        ← GitHub Pages deploy workflow (GitHub Actions)
```

## Deploying the web workbench

From the private `qdrant-db` source repo:

```bash
npm run deploy:web
```

This builds the React app with base `/qdrant-db-web/app/` and copies the output into `qdrant-db-web/app/`. Then commit and push `qdrant-db-web`.
