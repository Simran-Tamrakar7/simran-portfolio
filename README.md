# Simran Tamrakar — Portfolio

Static site for **simrantamrakar.com.np**.

## Local preview

```bash
python3 -m http.server 5173
```

Open http://localhost:5173

## Deploy

Point the domain (or a subdomain) at this folder via GitHub Pages, Netlify, Cloudflare Pages, or any static host.

Suggested Cloudflare / DNS:

1. Push this repo to GitHub.
2. Connect the host to the repo.
3. Add `simrantamrakar.com.np` as a custom domain.
4. Update the contact email in `index.html` once mail is set up.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | Portfolio |
| `cv.html` | Rough printable CV (Print → Save as PDF) |
| `styles.css` / `script.js` | Site styles & motion |
| `manifest.webmanifest` / `sw.js` | PWA install + offline shell |
| `assets/icons/` | App icons (192 / 512) |

## PWA

Install from the browser (Add to Home Screen / Install app). The service worker is **network-first**, so deploys show up while online; offline uses the last cached copy. After a publish, returning visitors get an **Update ready → Reload** prompt (or auto-refresh once the new worker activates).

When you change `sw.js` or precached paths, bump the `CACHE` string in `sw.js` so old caches are cleared.

## Notes

Portfolio and `cv.html` skills/experience are aligned with `simran-tamrakar-cv.md` (QA Associate at Infocom Solutions; full testing toolkit).
