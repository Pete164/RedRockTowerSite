# redrocktower.ie

Company site for Red Rock Tower Ltd (CRO 815834). One static page, no build step, no JavaScript.

- `index.html` — the page (inline CSS, light/dark via `prefers-color-scheme`).
- `_headers` — security headers applied by Cloudflare.
- `fonts/` — self-hosted Montserrat and Source Sans 3 (variable, latin subset, from Google Fonts). No third-party requests.
- `images/logo.png`, `images/logo-dark.png`, `images/mark.png` — the company logo cut onto transparency from `brand/RedRockTowerLogo.png` (the original artwork, on its paper background, not referenced by the page). `logo-dark.png` recolours the slate to light grey for dark mode.
- `images/bosca-logo.png` — copied from the BoscaWebsite repo; update it there first.
- `favicon.svg` — hand-drawn simplification of the mark (spire + rock).

## Hosting
Cloudflare Workers static assets (dashboard: Workers & Pages → redrocktowersite), connected to this GitHub repo. Every push to `main` deploys; other branches get a preview URL on `*-redrocktowersite.petersexton164.workers.dev`.
Build command: none. Output directory: `/` (repo root).
Custom domains: `redrocktower.ie` (Worker custom domain) and `www.redrocktower.ie` (proxied AAAA `100::` + Redirect Rule to the apex). Always Use HTTPS is on at zone level.

## Facts on the page
Registered office, company number and phone must match CRO and the Apple/Play developer records.
When any of those change (see the registered-office note in the project memory), change them here the same day.
