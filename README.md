# KINETIC ALCHEMIST

> A unified, hyper-realistic, futuristic file-transmutation and generative intelligence laboratory.

## Live Demo
Deploy via Vercel or GitHub Pages using this single static site.

---

## 🚀 Deploy on Vercel (Recommended)

### Option 1 – Vercel CLI
```bash
npm i -g vercel
vercel --prod
```

### Option 2 – Vercel Dashboard
1. Go to [vercel.com](https://vercel.com) → **New Project**
2. Import this repository
3. Vercel auto-detects `vercel.json` → no extra config needed
4. Click **Deploy** ✓

---

## 🐙 Deploy on GitHub Pages

### Option 1 – Manual
1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Set source to `main` branch, root `/`
4. GitHub Pages will serve `index.html` directly ✓

### Option 2 – GitHub Actions (auto-deploy on push)
Create `.github/workflows/deploy.yml` in your repo:
```yaml
name: Deploy to GitHub Pages
on:
  push:
    branches: [main]
jobs:
  deploy:
    runs-on: ubuntu-latest
    permissions:
      contents: write
    steps:
      - uses: actions/checkout@v3
      - name: Deploy
        uses: peaceiris/actions-gh-pages@v3
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          publish_dir: ./
```

---

## 📁 Project Structure
```
kinetic-alchemist/
├── index.html          # Main SPA entry point (entire app)
├── vercel.json         # Vercel deployment config
├── .nojekyll           # GitHub Pages — disables Jekyll processing
├── README.md           # This file
└── 404.html            # SPA fallback for GitHub Pages routing
```

---

## ✨ Features
- **Hub** — "Reforge Reality" landing with 3 animated glass pods
- **Image Alchemist** — AI-powered prompt-to-image synthesis with layer-by-layer canvas animation
- **Document Forge** — PDF/file conversion with drag-and-drop, live queue & progress
- **PNG Edge-Detection** — Interactive draggable detection beam with real-time alpha masking

## 🎨 Tech Highlights
- Pure vanilla HTML/CSS/JS — zero build step, instant deploy
- Custom WebGL-style canvas animations (orb, laser grid, edge beam)
- Animated particle constellation background
- Spring physics transitions between modules
- `Orbitron` + `Rajdhani` + `Share Tech Mono` typography system
- Full custom cursor, glass morphism panels, gold iridescent borders
