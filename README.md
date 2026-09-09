# Leo Hub

One page that links to every Leo notebook and app. Live at
**https://leojai23.github.io/leo-hub/**

| App | Link |
| --- | --- |
| MBA Study Notebook | https://leojai23.github.io/mba-notebook-pwa/ |
| Leo Interview Notebook | https://leojai23.github.io/leo-interview-notebook-pwa/ |
| Leo-Health — Satvic Reference | https://leojai23.github.io/leo-health/ |
| Leo Healing Study Companion | https://leojai23.github.io/leo-healing-study-companion/ |
| Leo-Finance | https://leojai23.github.io/leo-finance-pwa/ |

## Files

- `index.html` — the whole hub (inline CSS + JS, no dependencies).
- `manifest.json`, `sw.js`, `icon-*.png` — make it an installable, offline PWA.
- `build.py` — regenerates the icons and rewrites `sw.js` with a fresh
  content hash in `CACHE`.

## Updating

1. Edit `index.html` (add/rename a card).
2. `python build.py` — refreshes `sw.js` so browsers pick up the change.
3. `git add -A && git commit && git push` — GitHub Pages redeploys in ~1–3 min.
