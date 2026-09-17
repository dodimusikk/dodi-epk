# dodi-epk

Static one-page EPK for Dodi (minimal / microhouse DJ & producer), live at
**[dodi.fm](https://dodi.fm)**.

- Plain HTML, no build step. The page is `index.html`; press shot at
  `assets/press.jpg` (web, 1400px) with downloadable hi-res at
  `assets/press-hires.jpg` (both © Albin Händig). `assets/press-kit.zip` is the
  downloadable press kit (3 photos in web + print sizes, bios EN/SV, links, README);
  it is built from the career repo's `identity/bio.md` plus the photos folder, so it
  gets replaced wholesale rather than edited in place.
- Hosted on GitHub Pages from `main`: **a push deploys immediately**.
  `CNAME` and `.nojekyll` must stay.
- Catalog facts, links and bio are maintained in a separate private repo;
  this page is the public rendering of them.
- `.github/workflows/link-check.yml` checks all external links weekly and
  opens an issue if any have died.
