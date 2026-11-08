# NOTES

Handoff for FocacciaFriday. Future jobs: read this file first and keep it current. Notes stay on `dev`. Update `main` only after explicit approval from Marc.

## Purpose

FocacciaFriday is a focaccia calculator progressive web app. The repo is a static single-page app with no build script: baker's percentages, automatic yeast scaling, a pan calculator, and a step-by-step method with timers and notifications.

Published on GitHub Pages at `https://darcmuff.github.io/FocacciaFriday/`. `manifest.json` sets `start_url` and `scope` to `/FocacciaFriday/` and `display` to `standalone`. `privacy.html` (last updated 30 March 2026) says settings and session state stay on the device in `localStorage`, and the app does not collect or transmit personal data.

## Current state (2026-11-08)

- Default branch is `main`. Before this notes commit, `origin` had only `main`, at `3210f983e52a95e62c1d1701ac1d79ba1b6f5e0f` (2026-06-08, "Increase cold ferment final proof from 2.5hrs to 4hrs"). No root README and no earlier NOTES file.
- Tree checked this date: `index.html` (UI and calculator), `sw.js` (cache name `focacciafriday-v3`, timer notifications), `manifest.json`, `privacy.html`, root `icon-192.png` and `icon-512.png`, `assets/focc.jpg`, `og-image-v2.png`, `.well-known/assetlinks.json`. No `icons/` directory.
- Newest `main` history, from commit subjects only: cold-ferment final proof raised from 2.5 hours to 4 hours (2026-06-08); status bar, nav pill spacing, and dark mode in settings (2026-05-17 and 2026-05-18); time slider base changed from 8 to 12 for a 4–48 hour range (2026-05-15); `viewport-fit=cover` and `user-scalable=no` (2026-05-14); eat-time, timeline totals, and yeast effective-time fixes, plus session restore of hours, hydration, and temperature (2026-05-06 through 2026-05-13).
- No `TODO`, `FIXME`, or `WIP` markers in `index.html`, `sw.js`, `manifest.json`, or `privacy.html`.
- Path mismatch recorded from the files, not scheduled as work: `sw.js` precaches `/FocacciaFriday/icons/icon-192.png` and `icon-512.png`, and notification icons use `icons/icon-192.png`. The files on disk, and the paths in `manifest.json`, are `icon-192.png` and `icon-512.png` at the repo root.

## Verified next steps

No product roadmap is stated in the tree. Do not add one here.

1. Read `NOTES.md` before changing this repo, and update it in the same change when the facts above move.
2. Keep notes on `dev`. Leave `main` untouched until Marc explicitly approves that update.
3. Do not record secrets, tokens, or private data in this file.
4. The icon path mismatch above is the only inconsistency found in this pass. It is noted so it is not rediscovered. It is not an approved task.
