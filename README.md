# APT Intel — Cyber War Threat Intelligence

Interactive global map of nation-state APT attacks, economic impacts, and threat actor profiles.

## Deploy to GitHub Pages

### Option A — Upload via GitHub UI (Simplest)

1. Create a new repository on GitHub (e.g. `apt-intel`)
2. Go to the repository → **Add file → Upload files**
3. Drag and drop **all files from this folder** (including the hidden `.nojekyll` file)
4. Commit to `main` branch
5. Go to **Settings → Pages**
6. Under **Source**, select **Deploy from a branch**
7. Branch: `main`, Folder: `/ (root)` → click **Save**
8. Your site will be live at: `https://<your-username>.github.io/apt-intel/`

> ⚠️ Make sure `.nojekyll` is included — it prevents GitHub from breaking the asset paths.

---

### Option B — Git CLI

```bash
git init
git add .
git commit -m "Deploy APT Intel dashboard"
git branch -M main
git remote add origin https://github.com/<your-username>/apt-intel.git
git push -u origin main
```

Then enable GitHub Pages in Settings → Pages → Source: `main` / `/ (root)`.

---

## Files

| File | Purpose |
|------|---------|
| `index.html` | App entry point |
| `404.html` | Fallback for direct URL access |
| `.nojekyll` | Disables Jekyll processing (required) |
| `assets/` | Compiled JS + CSS bundles |

## Data Sources

- [Mandiant / Google Cloud APT Registry](https://cloud.google.com/security/resources/insights/apt-groups)
- [ESET APT Activity Reports](https://www.eset.com/business/resource-center/reports/)
- [TeamT5 APAC Threat Landscape 2025](https://teamt5.org/en/posts/apt-threat-landscape-in-apac-2025-industrialization-of-intrusions/)
- [CloudSEK Top APT Groups 2026](https://www.cloudsek.com/knowledge-base/top-apt-groups-dominated)
- [MITRE ATT&CK Framework](https://attack.mitre.org/)
