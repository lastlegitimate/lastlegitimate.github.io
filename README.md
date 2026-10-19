# lastlegitimate.com

Static personal site. One page, no build step, no backend, no JavaScript, no analytics.
The only external request is the display typeface (Google Fonts, `font-display: swap`,
so first paint never waits on it).

## Files
- `index.html` — the whole site. Edit this.
- `404.html` — not-found page.
- `robots.txt` — points researchers at `security.txt`.
- `.well-known/security.txt` — RFC 9116 contact + disclosure policy. Bump `Expires` yearly.
- `index-terminal-backup.html` — old draft. Not served as the homepage; safe to delete.

## Deploy (GitHub Pages)
1. Push to a repo (e.g. `lastlegitimate.github.io`, or any repo with Pages enabled).
2. Settings → Pages → deploy from `main` / root.
3. Custom domain: add a `CNAME` file containing `lastlegitimate.com` and point DNS at
   GitHub Pages. (Not committed here so the default `*.github.io` URL keeps working until
   DNS is ready.)

## Adding a disclosure to the Record
Newest first. Copy one `<details class="rec">` block in `index.html` and edit it.
Status ladder classes: `done` (filled), `now` (current, accent), none (pending/hollow).
Keep it honest — no CVE, report link, or vendor named before a fix ships.
