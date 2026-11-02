# Yards After Combustion

A 3D rocket-startup game from **Kittle Aerospace** (est. #85). You run a scrappy desert launch company: design rockets, win contracts, and catch your boosters with a 96-meter tower nicknamed *The Hands*.

**Play:** https://georgekittle85.github.io/SPACE/

## Controls

- **Base:** use the HQ / Hangar / R&D / Pad tabs to take contracts, build, research and launch.
- **Flight:** set throttle (100 / 70 / 50), `4×` time warp, and **SEPARATE** when the booster is spent.
- **The Catch:** steer with **WASD / arrow keys** (or the on-screen grid-fin stick), then **Space** to close the hands.

Progress saves to your browser's `localStorage`, so you can pick a season back up on the same device.

## How it's built

It's a single file, `index.html`, with no build step. [Three.js](https://threejs.org/) (r160) loads from jsDelivr and the fonts from Google Fonts.

Run it locally with any static server:

```bash
python3 -m http.server 8085
```

Then open http://localhost:8085.

## Deployment

`.github/workflows/deploy-pages.yml` publishes the site to GitHub Pages on every push to `main`. You can also run it by hand from the **Actions** tab ("Deploy to GitHub Pages" → *Run workflow*).

One-time setup: in **Settings → Pages → Build and deployment**, set **Source** to **GitHub Actions**.
