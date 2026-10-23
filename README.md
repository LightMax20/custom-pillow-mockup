# LightNest Pillow Studio

Vite + Three.js static starter for custom-shaped pillow concept previews from transparent PNGs.

## Run locally
Requires Node.js 20.19+ or 22.12+ for current Vite versions.

```bash
npm install
npm run dev
```

Build for deployment with `npm run build`; preview using `npm run preview`.

## Netlify
Build command: `npm run build`. Publish directory: `dist`. Both are configured in `netlify.toml`.

## Features
- PNG-only upload; trims transparent padding and approximates the outer alpha silhouette.
- 3D pillow preview with drag rotation, scroll zoom, front/back/360 controls.
- Puffiness, thickness, artwork scale, optional white border (off by default).
- Artwork PNG preview and 3D screenshot export.
- Responsive UI. No image upload API/server configured.

## Limitations
Starter prototype, not a manufacturing pipeline or physically simulated sewn textile. Uses a sampled outer contour and bevelled extrusion. Complex inner holes or very intricate outlines may not reproduce perfectly. The same artwork texture is applied to both sides without intentional mirroring, but the back-side material/orientation should be validated in-browser. Exports are previews, not guaranteed production-ready artwork. Validate against your supplier's actual print template before production.
