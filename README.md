# GrokTech LLC — Landing Page

Static site for GrokTech LLC IT services. Deployed on GitHub Pages.

**Live:** https://groktech.github.io/groktech-landing/

---

## File Structure

```
groktech/
├── index.html   # Single-page site (HTML5, semantic)
├── styles.css   # Dark theme styles (responsive, no frameworks)
└── README.md    # This file
```

---

## Deployment

### Option A — GitHub Pages (recommended)

1. Create a new repo under the TezCapital org (e.g. `groktech-landing`)
2. Push these files to `main`
3. Go to **Settings → Pages → Source** → select `main` branch, `/ (root)`
4. Wait ~2 min — site goes live at `https://tezcapital.github.io/groktech-landing/`

### Option B — Custom Domain (groktech.xyz)

Once GitHub Pages is live, update your DNS at groktech.xyz:

- **CNAME** record: `groktech` → `tezcapital.github.io`
- Or **A records** pointing to GitHub's IPs

Then add a `CNAME` file to the repo root:
```
groktech.xyz
```

---

## Local Preview

```bash
cd groktech
python3 -m http.server 8080
# open http://localhost:8080
```

---

## Notes

- No JavaScript dependencies — pure HTML/CSS
- Fonts: system font stack (SF Mono on macOS, Fira Code elsewhere)
- No analytics, no tracking, no external scripts
- Calendly link opens in new tab — no embed needed
