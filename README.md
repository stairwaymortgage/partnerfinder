# NEXA Pathfinder

Static website: homepage with the compass navigator and one-question-at-a-time evaluation, plus ten interview-style articles.

## Structure
- `index.html` — homepage (survey + provisional calendar, client-side only)
- `articles/` — ten articles sharing `styles.css` and `article-enhancements.js`
- `vercel.json` — Vercel config (clean URLs, no build step)

## Deploy (Vercel)
No build step. In Vercel: **Add New → Project → import this repo**, Framework Preset **Other**, leave Build Command and Output Directory empty. Every push to `main` deploys automatically.

## Before launch
- Audio players expect `audio/<article-name>.mp3` — files not yet supplied.
- Survey and calendar have no backend. The completion screen says info was "recorded" and a meeting "reserved" — change that copy or add a backend before launch.
- Custom domain / DNS to be configured in Vercel.
