# Unity Medical Transportation — GitHub Pages (Ready-to-Deploy)

This repo is pre-configured to publish with **GitHub Pages** and a custom domain: **www.unitymt.com**.

## 1) Create the repo
1. Sign in to GitHub → click **New repository**.
2. Name it: `unitymt-website` (Public).
3. Create the repo **empty** (don’t add template files).

## 2) Upload these files
- Click **Add file → Upload files** and drag everything from this folder:
  - `index.html` (your site)
  - `CNAME` (locks domain to `www.unitymt.com`)
  - `.nojekyll` (prevents Jekyll processing)
  - `404.html` (fallback page)
  - `assets/.keep` (placeholder for images/files)
  - `.gitattributes` and `.gitignore`

Commit to the **main** branch.

## 3) Enable Pages
- Repo → **Settings → Pages**.
- **Build and deployment → Source**: `Deploy from a branch`.
- **Branch**: `main`, **Folder**: `/root`. Save.
- Wait up to 60 seconds. You’ll see a green check + URL.

## 4) Point the domain (if not already set)
- In **Settings → Pages → Custom domain**, enter: `www.unitymt.com` and **Save**.
  - GitHub auto-creates/validates the `CNAME` file.
- In your DNS (registrar):
  - Add **CNAME** record → **Host/Name**: `www` → **Target**: `USERNAME.github.io` (replace `USERNAME`).
- Turn on **Enforce HTTPS** once the certificate is ready (toggle appears under Pages).

> Tip: Set your registrar to **forward** apex `unitymt.com` → `https://www.unitymt.com` for now. This avoids apex A‑record setup.

## 5) Easy editing
- Quick edit on GitHub: press `.` in the repo to open the web editor, tweak `index.html`, and **Commit**.
- Or use **GitHub Desktop** to drag-drop updates and **Push**.
- Or open a **Codespace** for a full IDE in the browser.

---
Generated: 2025-10-01 22:37:42
