# Raven Sisters — image assets

## ⚠️ Logo: action needed

`logo-placeholder.svg` is a **temporary text wordmark**, not the real mark. It exists only to
hold the correct 160×146 header slot. No raven was drawn — the real logo could not be read
from chat, only saved by hand.

**To install the real logo:**

1. Save the watercolour raven logo into this folder as **`logo-raven.png`**
   (full path: `D:\HaliteStudio\projects\ws_9bd393b88567\public\images\logo-raven.png`)
2. In `../../site.json`, change:
   ```json
   "nav": { "logo": "images/logo-placeholder.svg" }
   ```
   to:
   ```json
   "nav": { "logo": "images/logo-raven.png" }
   ```
3. Rebuild: `npm run build:site -- ws_9bd393b88567`

The header band is pure `#FFFFFF`, so a logo with a non-transparent white-ish background
blends without a visible seam. Transparency is optional.

## Photos

The `.jpg` files are **royalty-free stock photos** (Pexels / Unsplash), used until Raven
Sisters photography is supplied. Filenames are unchanged so `site.json` paths stay stable:

| File | Slot | Ratio used |
|---|---|---|
| `hero.jpg` | Full-bleed hero band | cover, 550px tall |
| `card-order.jpg` | Card 1 — "Order this week's drop" | 3:4 |
| `card-menu.jpg` | Card 2 — "What we bake" | 3:4 |
| `card-contact.jpg` | Card 3 — "Say hello" | 3:4 |
| `featured.jpg` | Full-width photo band | 1205:803 |
| `story.jpg` | Our Story two-column image | free |
| `favicon.png` | Favicon | square |

Keep the same filenames and the site needs no config change.
