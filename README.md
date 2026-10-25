# redrocktower.ie

Company site for Red Rock Tower Ltd (CRO 815834). One static page, no build step, no JavaScript.

- `index.html` — the page (inline CSS, light/dark via `prefers-color-scheme`).
- `_headers` — security headers applied by Cloudflare.
- `fonts/` — self-hosted Montserrat and Source Sans 3 (variable, latin subset, from Google Fonts). No third-party requests.
- `images/logo.svg`, `images/mark.svg` — the company logo as vectors, traced from `brand/RedRockTowerLogo.png` (the original 1024 px artwork, not referenced by the page) along its anti-aliased edges, so it stays sharp at any size. `logo.svg` keeps the paper background and is used as-is in both colour schemes. `images/og.png` (1200×630) is rendered from it for link previews.
- `images/bosca-logo.png` — copied from the BoscaWebsite repo; update it there first.
- `favicon.svg` — the traced mark on a paper rounded square.

## Hosting
Cloudflare Workers static assets (dashboard: Workers & Pages → redrocktowersite), connected to this GitHub repo. Every push to `main` deploys; other branches get a preview URL on `*-redrocktowersite.petersexton164.workers.dev`.
Build command: none. Output directory: `/` (repo root).
Custom domains: `redrocktower.ie` (Worker custom domain) and `www.redrocktower.ie` (proxied AAAA `100::` + Redirect Rule to the apex). Always Use HTTPS is on at zone level.

## Facts on the page
Registered office, company number and phone must match CRO and the Apple/Play developer records.
When any of those change (see the registered-office note in the project memory), change them here the same day.
