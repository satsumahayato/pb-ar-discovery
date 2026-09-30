# AR Discovery Mode: Paris Baguette Concept Demo

> **Concept demo only. Not affiliated with, endorsed by, or sponsored by Paris Baguette.**
> This is a design prototype. It is not an official Paris Baguette app or service. Menu items, prices, calorie counts, allergen information, and "PB Rewards" points shown here are illustrative and may not reflect what is sold in stores. For official allergen and nutrition information, see Paris Baguette's [2026 Spring Nutrition Chart (US, PDF)](https://parisbaguette.com/wp-content/uploads/2026/03/2026-Spring-Nutrition-Chart-US.pdf), and always confirm allergens with bakery staff.

Mobile web demo that explores how AR could help newcomers choose pastries at the display case. Point the rear camera at a pastry, tap inside the reticle, and get the pastry card, allergen info, insider collectibles, and mock rewards points.

## Run locally

Camera access requires HTTPS or `localhost`.

```bash
npx serve .
# or
python3 -m http.server 8000
```

Open `http://localhost:8000` on your phone or laptop.

## Deploy

- **GitHub Pages:** Settings → Pages → Deploy from branch → `main` / root. Open the `https://<user>.github.io/<repo>/` URL on a phone.
- **Netlify / Vercel:** import the repo, no build step, publish directory `.`

## Features

- Rear-camera AR mode; falls back to grid mode if camera is denied
- Color-signature recognition (13 pastries) on tap inside the reticle
- Pastry card with flavor/texture meters → flip to allergen shield
- Insider collectibles (after 3rd tap or 1st tray add, then every 5th tap)
- Digital tray with mock points and a mock QR checkout (not connected to any real rewards or payment system)
- Gom-i mascot celebrations

## Files

- `index.html`: the full app, self-contained (no dependencies, no build)

## Next steps

- Real-café testing for golden-brown lookalikes
- Optional neural classifier (Teachable Machine / TensorFlow Lite)
- Production React/Vite build with backend (pastry DB, rewards sync, checkout)

## Trademarks and images

Paris Baguette, PB Rewards, and related names and product photos are the property of their respective owners and appear here only to illustrate the design concept in an educational context. No commercial use is intended.
