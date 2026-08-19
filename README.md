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
