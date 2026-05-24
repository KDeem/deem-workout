# DEEM // PROTOCOL

Personal workout app. Single HTML file. No build step. Deploys to GitHub Pages in 2 minutes.

## What it does

- **Today view** — interactive workout for Day 1/2/3 + Day 4 long walk
  - Tap sets to mark complete
  - Auto-starts rest timer when you mark a set done
  - Interval timer for finishers (work/rest rounds)
  - Audio beep + phone vibration on transitions
- **Stealth view** — 3-tier CDW desk workout protocol
- **Progress view** — session count, weekly streak, weight log, quick notes
- **Reference view** — weekly schedule, daily targets, protein sources, progression rules

All data saved locally on the device (localStorage). Nothing leaves the phone.

## Deploy to GitHub Pages (5 steps)

1. Create a new GitHub repo (e.g. `deem-workout`) — public
2. Upload `index.html`, `README.md`, `.nojekyll` to the repo
3. Repo → **Settings** → **Pages** (left sidebar)
4. **Source:** Deploy from a branch → Branch: `main` → Folder: `/ (root)` → Save
5. Wait ~1 min, then open `https://<your-username>.github.io/deem-workout/`

Done. Bookmark on phone home screen for app-like access (iOS: tap Share → Add to Home Screen).

## Adding to iPhone home screen

1. Open the URL in Safari
2. Tap the Share button (bottom center)
3. Scroll down → **Add to Home Screen**
4. Name it "Protocol" or whatever — looks/acts like a real app

## Customizing

Open `index.html` in any text editor. Workout data is in the `WORKOUTS` object near the bottom (JavaScript section). Edit reps, sets, rest times, exercises. Save and re-upload.

## Files

- `index.html` — the entire app
- `README.md` — this file
- `.nojekyll` — tells GitHub Pages not to process this as Jekyll (faster, fewer surprises)

## Tech notes

- Vanilla JS + CSS — no React, no build, no dependencies except Google Fonts
- Mobile-first
- Dark theme · tactical/performance aesthetic
- Data persistence via `localStorage`
- Web Audio API for timer beeps
- Vibration API for haptics (Android — iOS Safari ignores)

## License

Personal use. Edit freely.
