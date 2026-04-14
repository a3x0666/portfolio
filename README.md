# Abhay Aneesh — Cybersecurity Portfolio

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![JetBrains Mono](https://img.shields.io/badge/Font-JetBrains_Mono-00ff9d?style=flat)
![Static](https://img.shields.io/badge/Deploy-Static_HTML-020b08?style=flat)

Personal cybersecurity portfolio — single-page static site with a SOC/terminal aesthetic. No build tools, no frameworks, no dependencies beyond Google Fonts.

## Overview

Single-page portfolio for Abhay P Aneesh, cybersecurity student at Lovely Professional University (B.Tech CSE, Cybersecurity minor, graduating June 2026). Covers experience at COROAT Trust and BEL, projects (MetaScan Platform, AutoBlocker), research (96.32% malware triage accuracy), certifications, and contact.

## Features

- **Zero dependencies** — pure HTML5, CSS3, vanilla JS; no npm, no build step
- **Terminal aesthetic** — scanline background, blinking cursor, `>_` section prefixes, `#00ff9d` accent
- **Responsive** — mobile nav collapses; layout adapts via CSS grid/flexbox
- **Interactive** — pulsing availability dot, left accent bar on card hover, smooth scroll
- **Stat chips** — inline research metrics (96.32% accuracy, 1.00 precision, 0 false positives)

## Tech Stack

| Layer   | Technology |
|---------|------------|
| Markup  | HTML5 (semantic) |
| Styling | CSS3 — custom properties (`--bg: #020b08`, `--accent: #00ff9d`, `--text: #d4ffe8`), scanline via `repeating-linear-gradient` |
| Script  | Vanilla JS (ES6+) |
| Fonts   | JetBrains Mono (headings), Inter (body) — Google Fonts CDN |
| Assets  | Static `.png` badges, `.jpg` profile photo |

## File Structure

```
portfolio/
├── index.html              # Full site — markup, styles, and JS all inline
├── cv-image.jpg            # Profile photo (replace with your own)
├── secplus-badge.png       # CompTIA Security+ (SY0-701)
├── netplus-badge.png       # CompTIA Network+ (N10-009)
├── azure-badge.png         # Azure Administrator (AZ-104)
├── google-cyber-badge.png  # Google Cybersecurity Professional
└── README.md
```

## Getting Started

### Local preview

No server required, but to avoid asset loading issues:

```bash
python -m http.server 8080   # Python 3
# or
npx serve .                  # Node
```

Open `http://localhost:8080`.

### Deploy

The site is a flat folder of static files — no build command needed.

| Platform | Method |
|----------|--------|
| **GitHub Pages** | Push repo → Settings → Pages → branch `main`, root `/` |
| **Netlify** | Drag folder onto [app.netlify.com](https://app.netlify.com) |
| **Vercel** | `vercel deploy` or import repo via dashboard |
| **Cloudflare Pages** | Connect repo or upload folder |

Entry point is root `index.html`.

## Customization

All content is in `index.html` — edit it directly, no compilation step.

**Swap profile photo** — replace `cv-image.jpg` with your own image (keep the filename), or update the `src` on the `<img>` tag in the hero section.

**Update text** — open `index.html` and locate sections by `id`: `#about`, `#experience`, `#projects`, `#research`, `#certifications`, `#skills`, `#education`, `#contact`.

**Swap badge images** — replace the `.png` files; filenames map directly to the four certifications listed above.

**Change accent color** — find the `:root` block near the top of the `<style>` tag in `index.html`:

```css
:root {
  --green: #00ff9d;
}
```

## License

Personal portfolio — free to use as a reference or template. Attribution appreciated but not required.

## Author

**Abhay P Aneesh** · Kerala, India  
B.Tech CSE (Cybersecurity minor) · LPU · June 2026

[abhay.aneesh2906@outlook.com](mailto:abhay.aneesh2906@outlook.com) · [GitHub @a3x0666](https://github.com/a3x0666) · [LinkedIn](https://linkedin.com/in/abhayaneesh) · +91 7559 144 918
