# 💕 LipGlow — AR Lipstick Shade Finder & Shop

Try on lipstick shades in real time with your **front camera**, browse multi-brand catalogs, add to cart, and check out — all in the browser.

![License](https://img.shields.io/badge/license-MIT-pink)
![Demo](https://img.shields.io/badge/demo-GitHub%20Pages-e91e63)

## Features

- **AR try-on** — MediaPipe Face Mesh tracks your lips live
- **Front camera** — Uses `getUserMedia` with `facingMode: user`
- **70+ shades** across MAC, Charlotte Tilbury, NARS, Fenty, Maybelline, Dior, YSL, Rare Beauty, Pat McGrath, Huda, Clinique, e.l.f., Revlon
- **Prices & cart** — Add items, change qty, free shipping over $50
- **Demo checkout** — Name, email, address, card fields (no real payment)
- **Cute pink UI** — Soft gradient, hearts, rounded cards
- **Snapshot** — Save a try-on photo
- **100% client-side** — Camera feed never leaves your device

## Quick start

### Option A — Open locally with a server (required for camera)

```bash
# Clone
git clone https://github.com/jnegapatanmendieta-coder/lipglow-ar.git
cd lipglow-ar

# Python
python3 -m http.server 8080

# Or Node
npx --yes serve -p 8080
```

Open **http://localhost:8080**

### Option B — GitHub Pages

After enabling Pages (Settings → Pages → Deploy from branch `main` / root), visit:

`https://jnegapatanmendieta-coder.github.io/lipglow-ar/`

## How to use

1. Click **Start Camera** and allow access
2. Pick a brand or search a shade
3. Tap a swatch to try it on
4. Adjust **Intensity**
5. **+ Cart** → open 🛒 → checkout

## Tech

| Piece | Stack |
|--------|--------|
| Face tracking | [MediaPipe Face Mesh](https://developers.google.com/mediapipe/solutions/vision/face_landmarker) (CDN) |
| Camera | `navigator.mediaDevices.getUserMedia` |
| UI | Single-file HTML / CSS / JS |
| Shop | Client-side cart + demo checkout |

No build step. No backend. No npm install required to run the demo.

## Project structure

```
lipglow-ar/
├── index.html      # Full app (AR + catalog + cart + checkout)
├── README.md
├── LICENSE
└── .gitignore
```

## Privacy

- Camera frames are processed **only in your browser**
- Nothing is uploaded to a server
- Checkout is a **prototype** — no real payments are processed

## License

MIT — see [LICENSE](LICENSE)

---

Made as a beauty e-commerce AR prototype 💗
