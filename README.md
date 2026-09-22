# smarticlab-track

Customer order-tracking page and ops panel for Smarticlab.

| Page | URL |
|---|---|
| Customer — My Orders / Track / Return / Exchange | https://track.smarticlab.in/ |
| Ops panel (noindex, robots-blocked) | https://track.smarticlab.in/ops.html |

## Deployment

Hosted on **Hostinger**, not GitHub Pages.

Auto-deployment is enabled: every push to `main` deploys into the site's
document root at `/home/u298839160/domains/smarticlab.in/public_html/track`.
Edit `index.html` or `ops.html` here and push — no manual upload needed.

DNS: `track` is an ALIAS to `track.smarticlab.in.cdn.hstgr.net` in the
`smarticlab.in` zone.

## Backend

All calls go to n8n at `https://auto.rohitvision.com/webhook/...`, which is
configured to allow CORS from `https://track.smarticlab.in`. The backend
lives outside this repo; nothing here holds credentials.
