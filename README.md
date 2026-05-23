# shoes-lander

One-page lander for **Shoes** — AI-driven custom orthotic insoles, scanned by iPhone LiDAR, shipped quarterly. Lives at `shoes.makeacompany.ai`.

Visual language borrowed from `donsgarage.makeacompany.ai` (Three.js exploded-view + glassmorphic panels) but re-skinned white/black/minimal and re-modeled as a stacked insole (top cover / foam / arch shell / midsole / base) that separates at peak scroll.

## Layout

- `index.html` — the whole site, single file, no framework. Google Fonts (Inter / Instrument Serif) via CDN, Three.js via importmap from unpkg.
- `Dockerfile` — `nginx:1.27-alpine` serving `index.html`.

## Local preview

```sh
# direct
open index.html

# or container
docker build -t shoes-lander . && docker run --rm -p 8080:80 shoes-lander
```

## Posture

Wellness program. Not a medical device. No FDA claims (Phase 1).
