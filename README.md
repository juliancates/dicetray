# Dice Tray

A single-page dice roller for tabletop games. Pick any mix of dice, hit **ROLL**, and watch them tumble on a felt tray before settling on their results — individually and as a combined total.

No build step, no dependencies, no backend. It's one HTML file you can open locally or drop on any static host.

## Features

- Supports d4, d6, d8, d10, d12, d20, and d100
- Add any number of each die type and re-roll the same set as often as you like
- Each die type has its own shape and color (d6s show real pip dots) so the tray is easy to read at a glance
- Animated tumble-and-settle roll, with results shown per die and grouped by type
- Running total displayed prominently after each roll
- Respects `prefers-reduced-motion` and is keyboard/focus accessible

## Usage

Open `index.html` directly in a browser — that's it.

To host it as a static site (GitHub Pages, Netlify, Vercel, S3, etc.), just publish `dice-tray.html` as-is. It has no server-side requirements.

### GitHub Pages

1. Push this repo to GitHub.
2. In **Settings → Pages**, set the source to your default branch.
3. If `dice-tray.html` isn't already named `index.html`, either rename it or point Pages at it directly — GitHub Pages serves whatever file you specify.

## How it works

- Pure HTML, CSS, and vanilla JavaScript — no frameworks or build tools.
- Die faces are drawn with CSS shapes (`clip-path`, `border-radius`) rather than images.
- The only external resource is a Google Fonts stylesheet (Roboto Slab + Inter); everything else is self-contained in the file.

## License

MIT — use, modify, and share freely.
