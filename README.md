# Made By Maddox

The portfolio of Tiffany Maddox, built as an early-00s desktop computer. Everything on the desktop opens: case studies, the My_Space profile, the showreel player, the playlist, and two games.

## How it's built

It's a static site with no build step.

- `index.html` holds the whole desktop: markup, styles and logic.
- `vendor/petite-vue.iife.js` is the small library that makes the windows interactive. It's served from this repo rather than a CDN.
- `images/` holds the wallpaper, portrait, share image and one hero image per case study, all as WebP.
- `_redirects` sends the old Squarespace URLs (like `/bodyform`) to the matching window on the new desktop.
- `favicon.svg` is the browser tab icon.

## Links into the desktop

Add a window's name after `#` to open it on load, for example:

- `madebymaddox.com/#bodyform` opens a case study (any case study slug works)
- `#cases`, `#ms`, `#services`, `#cmo`, `#reel`, `#games`, `#quiz`, `#sweeper`, `#brandagotchi`, `#contact`

## Hosting

Hosted on Cloudflare Pages, connected to this repo. Every push to `main` goes live, and other branches get their own preview link.

Settings when connecting the project: no framework preset, no build command, and `/` as the output directory.

## Updating

Ask Claude for the change ("add a new case study", "swap my photo", "update the 5× stat") and it edits the files here and pushes.
