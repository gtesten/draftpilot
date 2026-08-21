# DraftPilot 2026 — v37

## Shaker Dynasty
Shaker alone uses the dynasty model. It combines KeepTradeCut, DynastyProcess, and a cached FantasyCalc 1QB market snapshot, then blends that dynasty consensus 80/20 with the 2026 production model. Auction target/max guidance is calculated from the dynasty-ranked available pool and the actual remaining Shaker budgets.

FantasyCalc refresh endpoint for Shaker:
`https://api.fantasycalc.com/values/current?isDynasty=true&numQbs=1&numTeams=10&ppr=0.5`

## FERDA + DRE Digital
FERDA and DRE Digital remain full-PPR redraft leagues. Loading either preset resets every player back to the redraft ranking/value model; KTC, DynastyProcess, and FantasyCalc dynasty data do not influence those recommendations.

## v37 changes
- Adds FantasyCalc as the third Shaker dynasty consensus source.
- Keeps the dynasty model isolated to the Shaker preset.
- Preserves full-PPR redraft rankings for FERDA and DRE Digital.
- Preserves NFL Intel, injury badges, depth charts, draft sessions, Shaker auction tools, compact mode, tier breaks, mobile controls, and PWA support.
- Service-worker cache bumped to v37.

### FantasyCalc snapshot note
The direct FantasyCalc endpoint was not readable by the build environment's web cache during this refresh. The embedded FantasyCalc cache uses the current Aug. 21 1QB FantasyCalc market mirrored by DraftADynasty for the top 199 players. The exact 10-team/0.5-PPR endpoint above remains the canonical URL for future refreshes. Players missing from a source are averaged across the dynasty sources available for that player.
