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
  no SATYA mention until cleared (career `catalog/unreleased.md`); the Remixes rotator
  carries **released** remix credits only, and Falsa Magra is left off on purpose even
  though he's on DAM60 (Dodi, 2026-08-25 — not a name to lean on for credibility); no
  part 2 of the After Me remix comp on the page until it's out (career
  `catalog/unreleased.md`).
- The Remixes section is **not** a support/played-by list, and the header must not imply
  one: Kirill had no DJ-support data when asked (2026-04-06) and cleared the remixer
  names as the thing to credit instead. It was headed "Support" until 2026-08-25. A real
  Support section only goes up if confirmed DJ names arrive (career `catalog/released.md`,
  DAM60 entry). The fade rotator is deliberate — Dodi likes it; a flat list reads as a CV.
  In the rotator meta, DAM60 is shown by **catalogue number, not title** ("DAM60 · After
  Me"): under a header reading "Remixes", above a line reading "Remixed by X", the title
  "Dodi Remixes" was the third repetition on screen (Dodi, 2026-08-27). Releases with
  distinct titles keep theirs ("Incept EP · Tzinah Records") — the same rule the
  discography already follows for After Me's generically-titled records.
- If `assets/press.jpg` is replaced: keep the © EXIF, update the `og:image:width/height`
  meta to match, and refresh `assets/press-hires.jpg` (the press download target).
- This repo is the **single source of truth** for the EPK. Don't create copies in other
  projects (a duplicate in the career repo was removed 2026-06-10).
- Content/links come from `../dodi_artist_labels_carreer` (`assets/links.md`,
  `identity/bio.md`) — when facts conflict, the career repo wins.
- Voice: same rules as everywhere (global `~/.claude/CLAUDE.md` + career repo's voice
  section). Understated, scene-aware, no hype.
