# Lian Lahat Cosmetic — demo

Original single-page skincare demo (placeholder brand, lorem copy, CSS-rendered visuals).

## Run locally
It's a single static file — just open `index.html` in a browser, or serve it:

```bash
npx serve .
# or
python3 -m http.server 8000
```

## Deploy (free)

### Option A — GitHub Pages (static, uses GitHub Actions)
1. Put the workflow at `.github/workflows/deploy.yml` (file included in this folder as `deploy.yml`).
2. Push to the `main` branch.
3. Repo → **Settings → Pages → Build and deployment → Source: GitHub Actions**.
4. Every push to `main` builds and publishes. URL: `https://<user>.github.io/<repo>/`.

### Option B — Vercel (recommended once this becomes a Next.js app)
1. Push the repo to GitHub.
2. vercel.com → **Add New → Project → Import** your repo.
3. Zero config for static; for Next.js it's auto-detected.
4. You get a production URL **plus a preview URL on every push/PR** — ideal for testing.

Netlify and Cloudflare Pages work the same way (connect repo → auto-deploy).

## Files
- `index.html` — the site
- `.gitignore`
- `deploy.yml` — move to `.github/workflows/deploy.yml`
