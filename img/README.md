# Images for the store listings

Anything dropped in here is served at `https://pixelfishing.io/img/<filename>`
the moment it is pushed. Lower-case names, hyphens, no spaces — a space in a
filename becomes `%20` in the URL and breaks about half the places you paste it.

## What the listings need

Discord's App Directory takes screenshot uploads directly in the developer
portal, so it does **not** need these. Top.gg does: its long description is
markdown, so every image in it has to be a URL.

| File | What it is | Size |
| --- | --- | --- |
| `icon.png` | The app icon. Also the site favicon. | 512 × 512 |
| `og.png` | The link preview when the site is shared. | 1200 × 630 |
| `01-cast.png` | The waiting panel: float on the swell, Reel button. | 16:9 |
| `02-bite.png` | The alarm frame — red border, REEL! | 16:9 |
| `03-catch.png` | A catch reveal with a good field note. | 16:9 |
| `04-dex.png` | The record book, about two-thirds filled. | 16:9 |
| `05-map.png` | The map cross-section with a locked zone showing its price. | 16:9 |
| `06-trophy.png` | A trophy card from `/show`. The one people share. | 16:9 |
| `07-shop.png` | `/gear` in the North Atlantic, so the pounds show. | 16:9 |
| `08-board.png` | `/top` heaviest, with names on it. | 16:9 |

Take the screenshots on the live bot in a real server, dark theme, cropped to
the message but with enough Discord chrome that it reads as Discord.

## Keeping them small

A PNG straight out of a screenshot is often 2–3 MB. Anything over about 400 KB
is worth squashing — the listing pages load slowly otherwise, and GitHub Pages
has a 1 GB repository limit. macOS can do it without installing anything:

    sips -Z 1920 08-board.png --out 08-board.png
