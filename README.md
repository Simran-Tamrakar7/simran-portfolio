# Simran Tamrakar — Portfolio

Static site for **[simrantamrakar.com.np](https://simrantamrakar.com.np)** — QA Associate portfolio, printable CV, and PWA shell.

## About

- **Role:** QA Associate at Infocom Solutions Pvt. Ltd. (Kathmandu)
- **Focus:** Manual QA, API testing (Postman), regression / UAT, automation practice (Playwright, Cypress, Selenium)
- **Domains:** Bizlevate HRMS, PrimeSales360, SalesMania
- **Contact:** [simrantamrakar77@gmail.com](mailto:simrantamrakar77@gmail.com) · [LinkedIn](https://www.linkedin.com/in/simran-tamrakar-1aa84b349/) · [GitHub](https://github.com/Simran-Tamrakar7)

## Local preview

```bash
python3 -m http.server 5173
```

- Portfolio: http://localhost:5173/
- CV: http://localhost:5173/cv.html

## Content source of truth

Skills, experience, education, and contact details live in **`simran-tamrakar-cv.md`**. Keep `index.html` and `cv.html` in sync with that file. See [`docs/content-source.md`](docs/content-source.md).

## Skills (summary)

| Area | Highlights |
| --- | --- |
| Testing | Manual, functional, regression, smoke/sanity, API, UI/UX, cross-browser, mobile, UAT, test design & planning |
| Tools | Postman, ClickUp, Jira, Chrome DevTools, JMeter, Selenium, Cypress, Playwright, Git/GitHub, Figma, Notion |
| Languages & data | Python, Java, JavaScript, SQL, HTML/CSS, MySQL, PostgreSQL |
| Soft skills | Module ownership, communication, documentation, attention to detail |

## Files

| File | Purpose |
| --- | --- |
| `index.html` | Portfolio (about, work, experience, skills, contact) |
| `cv.html` | Printable CV (Print → Save as PDF) |
| `simran-tamrakar-cv.md` | Canonical CV / skills source |
| `styles.css` / `script.js` | Site styles & motion |
| `manifest.webmanifest` / `sw.js` | PWA install + offline shell |
| `assets/` | Avatar and app icons (192 / 512) |
| `docs/content-source.md` | How content stays aligned |
| `CNAME` | Custom domain for GitHub Pages |

## Deploy

Point the domain at this folder via GitHub Pages, Netlify, Cloudflare Pages, or any static host.

1. Push this repo to GitHub.
2. Connect the host to the repo (or enable GitHub Pages from `master`).
3. Keep `simrantamrakar.com.np` as the custom domain (`CNAME`).

## PWA

Install from the browser (Add to Home Screen / Install app). The service worker is **network-first**, so deploys show up while online; offline uses the last cached copy. After a publish, returning visitors get an **Update ready → Reload** prompt (or auto-refresh once the new worker activates).

When you change `sw.js` or precached paths, bump the `CACHE` string in `sw.js` so old caches are cleared.
