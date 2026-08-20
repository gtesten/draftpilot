# DraftPilot 2026

GitHub-ready release based on DraftPilot version 28.

## Included
- FERDA, DRE Digital, and Shaker Dynasty presets
- Shaker-only auction budgets and live nomination workflow
- Live roster and remaining-needs tracking for all three leagues
- Corrected Next Pick % risk model and color coding
- Sticky Draft / Nominate action buttons
- Recent picks, Last Action banner, Draft Mode, Undo, and two-click Reset
- Browser auto-save, named draft sessions, and JSON import/export
- PWA manifest and service worker

## Publish the update
Upload/replace `index.html`, `manifest.webmanifest`, `sw.js`, `.nojekyll`, and the `icons` folder in the root of your existing GitHub repository, then commit to `main`.

If GitHub Pages is already set to **Deploy from a branch → main → /(root)**, the site republishes automatically.

## After publishing
Because DraftPilot uses a service worker, refresh the live site once after GitHub finishes deploying. If an installed app still shows the old version, fully close and reopen it. Existing named sessions use the same browser storage keys and should remain available on the same device.


## v30 NFL Intel + automatic board adjustments
Adds a lightweight NFL Intel view with a current Aug. 19, 2026 ESPN fantasy depth-chart snapshot, curated fantasy-impact injury news, live source links, and injury badges on affected draft-board players. The snapshot is static by design to keep DraftPilot responsive during live drafts.


### Automatic injury-value adjustments
NFL Intel now carries lightweight ranking modifiers with material injury news. When the Intel snapshot is refreshed, related downgrades, beneficiary bumps, and season-ending redraft removals can be updated in the same data block. The feature is ON by default and can be toggled from the NFL Intel page.
