# PC Lab 3D

Interactive 3D computer assembly & exploration simulator that runs entirely in
the browser (three.js r160 from CDN, no build step).

Pick a difficulty level and build a computer piece by piece:

- 🧒 **Elementary** — 10 main parts in everyday words
- 🎒 **High School** — 14 parts with real technical terms
- 🎓 **College** — 24-part full build incl. peripherals and cabling
- 🔧 **Tinkerer** — 21 motherboard-level components (VRM, chipset, POST)

Build, disassemble or explore mode, guided next-step hints, exploded view,
X-ray, part labels, undo/reset, and a boot console when everything is
installed. Progress per level is saved in localStorage.

## Run locally

Any static file server works:

```bash
cd public
python -m http.server 8080
```

## Deploy

Assets-only Cloudflare Worker, custom domain `comlab-3d.skiddph.com`:

```bash
npx wrangler deploy
```
