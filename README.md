# Message On Hold — Website

Live site: **https://jamesonflex.github.io/Message-On-Hold/**

One-page site for **Message On Hold** (messageonholdphones.com): on-hold messaging, AI phone ordering and VOIP for pizza shops and quick-service restaurants. Everything runs from `index.html`, with no build step.

## What's inside

| File | Purpose |
|---|---|
| `index.html` | The site (demo player, audio mixer, 3D AI-ordering flow with voices, swipeable reviews) |
| `contact.html` | Free 60-day trial quiz funnel — every trial/contact button on the site leads here |
| `og-image.jpg` | 1200×630 link-preview image (Messenger, iMessage, WhatsApp, LinkedIn, Slack, X, SMS) |
| `favicon.ico`, `favicon.svg`, `favicon-32.png` | Browser tab icons |
| `apple-touch-icon.png`, `icon-192.png`, `icon-512.png`, `site.webmanifest` | Home-screen / app icons |
| `assets/logo.svg` | Vector logo, used if the live-site logo can't load |
| `404.html` | Sends any wrong address inside the site back to the homepage |
| `robots.txt`, `sitemap.xml`, `.nojekyll` | Search + GitHub Pages housekeeping |

## Updating the site

Upload the files to the **root** of the `Message-On-Hold` repo (replace existing), then commit. GitHub Pages republishes in about a minute.

## Link previews

All preview tags point to `https://jamesonflex.github.io/Message-On-Hold/`. The address is **case-sensitive**: keep the repo named exactly `Message-On-Hold`. If you rename the repo or add a custom domain, find and replace that address in `index.html`, `robots.txt` and `sitemap.xml`.

**After any change to the preview, refresh Facebook's copy** (Messenger caches it):

1. Open https://developers.facebook.com/tools/debug/
2. Paste `https://jamesonflex.github.io/Message-On-Hold/` and click **Debug**.
3. Click **Scrape Again** until "Link" and "Image" show the new values.

Other checkers: LinkedIn https://www.linkedin.com/post-inspector/

iMessage caches the first preview it sees, so send the link only after the new files are live.

## Trial requests (contact.html)

Every "Free 60-Day Trial" / "Contact" button opens `contact.html`, a 5-step quiz (business type → locations → services → busy-phone problem → contact details).

- Requests are emailed to **sales@messageonholdservice.com** through FormSubmit (formsubmit.co), a free form-to-email service — no server needed.
- **One-time activation:** the very first request triggers a FormSubmit email to that inbox titled "Action Required: Activate FormSubmit". Someone at Message On Hold must click **Activate Form** once. Until then, visitors get a one-tap "send by email" fallback with everything pre-filled, so no lead is lost.
- To send requests to a different inbox, change `LEAD_TO` near the top of the script in `contact.html`.
- If a visitor built a mix in the Audio Mixer, it's attached to their request automatically.
