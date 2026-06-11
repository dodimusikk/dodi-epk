# dodi-epk

Static one-page EPK for Dodi (minimal / microhouse DJ & producer), live at
**[dodi.fm](https://dodi.fm)**.

- Plain HTML, no build step. The page is `index.html`; press shot at
  `assets/press.jpg` (photo © Albin Händig).
- Hosted on GitHub Pages from `main`: **a push deploys immediately**.
  `CNAME` and `.nojekyll` must stay.
- Catalog facts, links and bio are maintained in a separate private repo;
  this page is the public rendering of them.
- `.github/workflows/link-check.yml` checks all external links weekly and
  opens an issue if any have died.
