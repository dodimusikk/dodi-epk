---
description: Sync the EPK page against the career repo's catalog/links (review before push)
---

# /sync-site — keep dodi.fm honest against the CRM

The career repo (`../dodi_artist_labels_carreer`) is the source of truth for catalog
facts and links; this page is the public rendering. This command reconciles them.

## Steps

1. **Read the truth**: `../dodi_artist_labels_carreer/catalog/released.md`,
   `catalog/unreleased.md`, `assets/links.md` (mixes/playlists), `identity/bio.md`.
2. **Diff against `index.html`**:
   - Discography rows (`<section class="disco">`): every released item present, with
     catalog numbers, correct Bandcamp links, `· various artists` styling for VA
     appearances. Forthcoming rows (`class="ttl fc"`) only for **confirmed, placed**
     releases from `unreleased.md` — nothing tentative goes public.
   - Mixes tabs (`#mixTabs`): URLs still match the canonical mix/playlist links.
   - Support rotator: names/quotes still accurate and confirmed (anti-claims rule:
     nothing unverified).
   - Bio/meta text drift vs `identity/bio.md`.
3. **Apply the edits to `index.html`** — match the existing row markup exactly; the
   page is hand-crafted, no build step.
4. **Verify locally**: `open index.html` for the user to eyeball.
5. **Commit locally. NEVER push without explicit confirmation** — a push publishes to
   dodi.fm immediately. Say what changed and wait.

## Rules
- Voice + anti-claims per global rules and the career repo. Understated; show, don't tell.
- When the catalog and the page disagree, the catalog wins — but if the catalog
  itself looks stale (e.g. a release the user mentioned isn't there), flag it for the
  career repo instead of inventing page content.
