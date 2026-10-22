# Message On Hold — Website

One-page site for **Message On Hold** (messageonholdphones.com): on-hold messaging, AI phone ordering and VOIP for pizza shops and quick-service restaurants.

Everything runs from `index.html`. No build step, no dependencies.

## What's inside

| File | Purpose |
|---|---|
| `index.html` | The site (demo player, 3D AI-ordering flow with voices, swipeable reviews) |
| `og-image.jpg` | 1200×630 link-preview image (iMessage, WhatsApp, Facebook, LinkedIn, Slack, X, SMS) |
| `favicon.ico`, `favicon.svg`, `favicon-32.png` | Browser tab icons |
| `apple-touch-icon.png`, `icon-192.png`, `icon-512.png`, `site.webmanifest` | Home-screen / app icons |
| `assets/logo.svg` | Vector logo, used if the live-site logo can't load |
| `404.html` | Branded "page not found" that returns home |
| `robots.txt`, `sitemap.xml`, `.nojekyll` | Search + GitHub Pages housekeeping |

## Publish on GitHub Pages (about 3 minutes)

1. On GitHub, create a **public** repo named exactly **`messageonhold`**.
2. Upload **all files in this folder** to the repo root, including `.nojekyll`, then commit.
3. Go to **Settings → Pages**. Under **Build and deployment**, set **Source = Deploy from a branch**, **Branch = `main`**, **Folder = `/ (root)`**, then **Save**.
4. After about a minute the site is live at **https://jamesonflex.github.io/messageonhold/**

## Link previews

The preview tags point to `https://jamesonflex.github.io/messageonhold/`.

**If you use a different repo name or a custom domain**, find and replace that URL in `index.html` (it appears in `canonical`, `og:url`, `og:image` and `twitter:image`), and in `robots.txt` and `sitemap.xml`. Previews need full absolute URLs to work.

**Testing and refreshing previews:**

- Facebook / Messenger / WhatsApp: https://developers.facebook.com/tools/debug/ → paste the URL → **Scrape Again**.
- LinkedIn: https://www.linkedin.com/post-inspector/
- iMessage caches the first preview it sees. Send the link once the site is live, not before.
