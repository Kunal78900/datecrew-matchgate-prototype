# MatchGate, preference-first profile screening (demo)

Single-file static prototype built for a product assessment. No build step, no dependencies, no backend. All data is mocked and lives inside `index.html`.

## Run locally

Open `index.html` in any browser.

## Deployment

Live at https://datecrew-matchgate-prototype.vercel.app/

This repo is deployed on Vercel as a generic static site: no framework preset, no build command, output is the repository root, and `index.html` serves at the site root. The project owner redeploys from Vercel after changes land on `main` (a Git-connected Vercel project redeploys automatically on push; otherwise redeploy from the Vercel dashboard).

## What the demo shows

1. **Client preference record** - stated preferences plus explicit deal-breakers.
2. **Pre-send profile check** - BLOCKED / REVIEW / CLEAR verdicts with plain-language reasons. Deal-breaker conflicts block; soft preference mismatches flag for review; missing or unrecognized information must be confirmed before sending. Checks are advisory: the demo sends nothing and persists no overrides.
3. **Rejection feedback structurer** - local keyword rules in this demo; the production version would use an AI call for free text.
4. **30-day rejection dashboard** - the category split is illustrative demo data; only the brief's own figures (1,000 shared, 690 rejected, about 35% preventable) are real.
