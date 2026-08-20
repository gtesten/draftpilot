# DraftPilot 2026 — v32

GitHub Pages / PWA release matching the latest DraftPilot build.

## Included
- FERDA, DRE Digital, and Shaker Dynasty league presets
- Shaker-only auction budgets, nominations, live bids, and winner recording
- Live roster and remaining-needs tracking for every league
- Corrected and color-coded Next Pick % model
- Sticky On the Clock bar, sticky action column, sticky player-table header
- Quick search-to-Draft / Nominate workflow
- Top available QB/RB/WR/TE cards and obvious YOUR PICK state
- My Guys / Avoid controls, recent picks, league roster tracker, Draft Mode, Undo, and two-click Reset
- Automatic early-round K/DST hiding in redraft leagues
- NFL Intel tab with fantasy injury watch and 32-team depth charts
- Depth charts show QB1, RB1/RB2, WR1/WR2/WR3, and TE1/TE2 for every team
- Lightweight injury-driven draft-value adjustments for material news
- Browser auto-save, named draft sessions, and JSON import/export
- Installable PWA files for GitHub Pages

## Publish
Upload/replace everything in this ZIP at the root of the existing `draftpilot` GitHub repository, then commit to `main`.

If GitHub Pages is already configured as **Deploy from a branch → main → /(root)**, publishing happens automatically.

## After publishing
Wait for GitHub Pages to finish, then refresh DraftPilot once. If the installed PWA still shows an older version, fully close and reopen it. The service-worker cache name is updated for v32, while named browser sessions retain the same storage keys.

## NFL Intel freshness
The NFL Intel area is an embedded Aug. 20, 2026 snapshot so the draft interface remains responsive. Refresh the depth charts, injury news, and associated value adjustments before important drafts when material NFL news changes.
