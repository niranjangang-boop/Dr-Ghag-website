# Live Site Patch — How to Apply

Drop-in fixes for your CURRENT GitHub Pages repo (the one with `index-BOZMa-ei.js`).
Deployable today, no build step needed.

## Steps

1. Copy everything in this folder into the root of your GitHub repo,
   **replacing** existing files (`index.html`, the `assets/` images).
2. The old repo has duplicate images at the repo root (outside `assets/`) —
   they are unused and can be deleted.
3. Commit and push. GitHub Pages redeploys automatically.

## What this changes

- `index.html` — correct title ("Dr. Niranjan Ghag | Orthopedic Surgeon"),
  meta description, canonical, Open Graph tags, favicon links, hero preload,
  and full Physician + Joshi's Neurotrauma Centre JSON-LD schema.
- `404.html` — copy of index.html so deep links (e.g. /about) work on GitHub Pages.
- `favicon.ico`, `favicon-16/32.png`, `icon-192/512.png`, `apple-touch-icon.png` — NG logo favicons.
- `sitemap.xml` + `robots.txt` — submit the sitemap in Google Search Console.
- `assets/` — same filenames, recompressed: 9.5 MB → 3.0 MB.

## After deploying

- Google Search Console → Sitemaps → submit `https://www.drniranjanghag.com/sitemap.xml`
- Test schema at https://search.google.com/test/rich-results
