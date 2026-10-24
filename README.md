# redrocktower.ie

Company site for Red Rock Tower Ltd (CRO 815834). One static page, no build step, no JavaScript.

- `index.html` — the page (inline CSS, light/dark via `prefers-color-scheme`).
- `_headers` — security headers applied by Cloudflare Pages.
- `images/bosca-logo.png` — copied from the BoscaWebsite repo; update it there first.

## Hosting
Cloudflare Pages, connected to this GitHub repo. Every push to `main` deploys.
Build command: none. Output directory: `/` (repo root).
Custom domains: `redrocktower.ie` and `www.redrocktower.ie` (DNS is already on Cloudflare).

## Facts on the page
Registered office, company number and phone must match CRO and the Apple/Play developer records.
When any of those change (see the registered-office note in the project memory), change them here the same day.
