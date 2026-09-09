# Dharshan V — Portfolio

Personal portfolio site. Single-page static website — plain HTML/CSS, no build step.

## Structure

| File | Purpose |
|------|---------|
| `index.html` | The site (entry point Vercel serves) |
| `vercel.json` | Clean URLs + security headers |
| `robots.txt`, `sitemap.xml` | SEO |
| `package.json` | Local preview script only |
| `dharshan_portfolio.html` | Original source file (kept for reference) |

## Local preview

```bash
npm run dev      # serves at http://localhost:3000
```

Or just open `index.html` in a browser.

## Deploy to Vercel

### Option A — Dashboard
1. Push this folder to a GitHub repo.
2. On [vercel.com](https://vercel.com) → **Add New → Project** → import the repo.
3. Framework preset: **Other**. Build command: *none*. Output directory: *leave blank* (root).
4. **Deploy.**

### Option B — CLI
```bash
npm i -g vercel
vercel          # preview deploy
vercel --prod   # production deploy
```

No environment variables or build configuration required.

## After deploying

Update the production URL in `index.html` (`canonical`, `og:url`), `robots.txt`, and `sitemap.xml` if your domain differs from `dharshan-portfolio.vercel.app`.
