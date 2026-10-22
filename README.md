# Fitness Incremental — offline workout PWA

## Publish to GitHub Pages
1. Extract the ZIP.
2. Create a new public GitHub repository (or use an existing one).
3. Upload **all seven website files plus this README** to the repository root (not the outer folder).
4. Open repository **Settings → Pages → Build and deployment → Deploy from a branch**.
5. Select branch `main`, folder `/ (root)`, then **Save**.
6. Visit the GitHub Pages URL GitHub displays after deployment.
7. On iPhone, open the URL in Safari and select **Share → Add to Home Screen**. Open once while online to cache the site for offline use.

## Features
- Opens on today's date; calendar picker for previous or future dates.
- One scrollable workout screen with per-set autosaving, suggested totals and actual reps.
- Exact compounding per exercise: baseline × (1 + percentage / 100) ^ number of earlier completed workouts involving that exercise. Only displayed targets are rounded.
- Growth continues even if actual reps are lower; the rate is adjustable per exercise.
- Split suggested total across any number of sets.
- Finish Workout button, history feed, monthly calendar, individual and overall progress graphs.
- Add, reorder, hide, and edit exercises; descriptions behind ⓘ.
- Local IndexedDB storage, offline service worker, JSON backup and restore.

## Important
GitHub hosts only the **app code**. Workout data is saved in the browser on the device, not on GitHub. Back up regularly with **Settings → Export JSON**, and save that file to iCloud Drive or another safe location. A different device or browser won't automatically share the data. Clearing browser storage may delete it.

The included 2024 workout numbers are example starting values taken from an older routine, not a prescription. Review them in Settings. Prone reverse flies start at 10 total reps, one set, 0% growth; stop any movement that causes tingling or pain.

## Version 1 limitation
One workout per date. Already-created workout targets remain snapshots; editing earlier dates doesn't automatically rewrite them. Baselines and rates in Settings affect workouts created afterward. 
