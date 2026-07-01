# dodi-epk

Static one-page EPK for Dodi, live at **https://dodi.fm** (GitHub Pages, deploys from
`main` — a push publishes immediately, so confirm before pushing).

- Page content lives in `index.html` (single file, no build step); press shot at
  `assets/press.jpg` (web, 1400px) + `assets/press-hires.jpg` (downloadable hi-res,
  both © Albin Händig); favicon at `assets/favicon.svg`; `CNAME` + `.nojekyll` must stay.
- Weekly link-check workflow (`.github/workflows/link-check.yml`) opens an issue when
  an external link dies (ra.co + instagram excluded — they bot-block; rationale for
  every skip is commented in the workflow).
- Git identity here: author as `Dodi <hello@dodi.fm>` (repo-local config; public repo,
  personal addresses stay out of history). No Claude trailers, as everywhere.
- **Deliberate absences — don't "fix" by adding:** no dates/gigs section (held back
  2026-06; rationale, re-add trigger and ready markup in career `catalog/gigs.md`);
  no SATYA mention until cleared (career `catalog/unreleased.md`); support rotator
  names four of six remixers on purpose (career `catalog/unreleased.md`, After Me
  remix-comp entry).
- If `assets/press.jpg` is replaced: keep the © EXIF, update the `og:image:width/height`
  meta to match, and refresh `assets/press-hires.jpg` (the press download target).
- This repo is the **single source of truth** for the EPK. Don't create copies in other
  projects (a duplicate in the career repo was removed 2026-06-10).
- Content/links come from `../dodi_artist_labels_carreer` (`assets/links.md`,
  `identity/bio.md`) — when facts conflict, the career repo wins.
- Voice: same rules as everywhere (global `~/.claude/CLAUDE.md` + career repo's voice
  section). Understated, scene-aware, no hype.
