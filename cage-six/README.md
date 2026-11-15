# Cage Six

20,000 graded 6×6 KenKen-style cage puzzles (5,000 each: Easy, Mild, Hard, Super hard) in a single installable web app. Works offline once loaded.

**Play:** https://therealgitguy.github.io/eye-suite-dashboard/cage-six/

## Install on Android
1. Open the link above in Chrome.
2. Tap **⋮ → Install app** (or **Add to home screen → Install**).
3. Launch Cage Six from the home screen — it runs full-screen and offline.

## How puzzles are made
Each puzzle is rebuilt from its name (e.g. *Hard #0042*) by a seeded random generator: a random Latin square is made, cages are grown and given operations, then a human-style logic solver grades it. Only puzzles whose grade matches the level (and that have exactly one solution) are kept. Full detail is in the app's *How it's made* tab.

## Files
- `index.html` — the whole app (engine + UI)
- `manifest.webmanifest`, `icons/` — install metadata
- `sw.js` — offline cache. **Bump `VERSION` in `sw.js` with every release.**

Stats are stored in cookies on the device (localStorage mirror as backup).
