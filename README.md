# Warren — GitHub Pages Site

This directory contains the public-facing website for **Warren**, an AI-powered financial assistant. It is intended for Plaid compliance review and serves as the app's public website URL.

---

## ✅ This Repository Is Safe to Make Public

The files in this directory contain **no secrets, credentials, or private information**. Specifically:

- No `PLAID_CLIENT_ID` or `PLAID_SECRET`
- No API keys or access tokens
- No database URLs or Supabase keys
- No backend server URLs
- No `.env` files
- No personal banking information

---

## 🔒 Secrets Must Never Be Committed

Before pushing **any** code to a public repository, verify that secrets are excluded.

Add the following to your root `.gitignore` (and confirm it is in place):

```
# Environment variables — never commit these
.env
.env.*
*.env

# Secrets
secrets.json
credentials.json
```

Run `git status` and `git diff --cached` before every commit to confirm no sensitive files are staged.

---

## 🚀 Deploying to GitHub Pages

### 1. Create a GitHub repository

Go to [github.com/new](https://github.com/new) and create a **public** repository (e.g., `warren-site`).

### 2. Push the files

From the root of your project:

```bash
git init
git add docs/
git commit -m "Add Warren public website"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/warren-site.git
git push -u origin main
```

### 3. Enable GitHub Pages

1. Open the repository on GitHub.
2. Go to **Settings → Pages**.
3. Under **Source**, select:
   - Branch: `main`
   - Folder: `/docs`
4. Click **Save**.

GitHub will build and publish the site. It typically goes live within 1–2 minutes.

### 4. Get your URL

Your site will be available at:

```
https://YOUR_USERNAME.github.io/warren-site/
```

Use this URL as the **Website URL** in the Plaid Developer Dashboard when submitting your app for review.

---

## Files

| File | Purpose |
|------|---------|
| `index.html` | Main one-page website |
| `style.css` | Styles (no external dependencies) |
| `README.md` | This file |

---

## Notes

- The site uses no external libraries, fonts, analytics, or tracking scripts.
- No cookies are set by this site.
- The site is fully static — no server-side code required.
