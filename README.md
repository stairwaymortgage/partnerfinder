# NEXA Pathfinder

Static website: homepage with the compass navigator and one-question-at-a-time evaluation, plus ten interview-style articles.

## Structure
- `index.html` — homepage (survey + provisional calendar, client-side only)
- `articles/` — ten articles sharing `styles.css` and `article-enhancements.js`
- `vercel.json` — Vercel config (clean URLs, no build step)

## Deploy (Vercel)
No build step. In Vercel: **Add New → Project → import this repo**, Framework Preset **Other**, leave Build Command and Output Directory empty. Every push to `main` deploys automatically.

## Lead capture
The evaluation posts to the OneFocus CRM: `POST https://www.onefocuscrm.com/api/forms/pathfinder` (brand slug `pathfinder`).
The CRM stores the lead, emails an alert to the brand's notify address, and sends the visitor a confirm-your-email message.
The thank-you screen only shows after the CRM confirms the save; on failure the visitor sees an error and can retry.

**Adding a custom domain:** add `https://<domain>` (and `https://www.<domain>`) to the `pathfinder` brand's
`allowed_origins` in the CRM, or the form will be refused from that domain.

## Still to do
- Audio players expect `audio/<article-name>.mp3` — files not yet supplied.
- Meeting times are requested, not booked; the team confirms each one personally.
