# Athletic Gym Companion

Single-page workout companion for the final accepted 6-day gym plan.

## Open Locally

Open `index.html` directly in your browser.

No build step is required. This version is dependency-free because this machine does not currently have `node` or `npm` available.

## Features

- Monday to Saturday workout selector, with Sunday rest day.
- Warm-up templates, exercises, wrist notes, alternatives, supersets, time budget, and progression rules.
- Exercise completion checkboxes saved in `localStorage`.
- Per-exercise notes saved in `localStorage`.
- Per-exercise rest timers.
- Reset button for the selected day.
- YouTube search links for each exercise form video.
- Verified remote exercise images, with generated local SVG fallbacks if a remote image fails.

## Editing The Workout

All workout data is inside `index.html` in these objects:

- `warmups`
- `days`
- `progression`
- `exerciseImages`

Exercise images are mapped in `exerciseImages`. If a remote image fails to load, the card automatically falls back to a locally generated SVG from the exercise's `visual` type.
