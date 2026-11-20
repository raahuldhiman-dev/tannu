# Taranpreet Kaur — Digital Marketing Portfolio

Redesigned, interactive single-page portfolio for **Taranpreet Kaur** (Digital Marketing Specialist — SEO, PPC, AEO, GEO, analytics).

Built with plain HTML / CSS / vanilla JavaScript — no frameworks, fully deployable to GitHub Pages.

## Run locally

Just open `index.html` in a browser, or serve the folder:

```bash
npx serve .
# or
python -m http.server 8080
```

## Features

- **Interactive case studies** — tabbed switcher with animated panels
- **Animated counters** — scroll-triggered stats
- **Typing rotator** — animated role highlights in the hero
- **Scroll reveal** animations, scroll progress bar, back-to-top
- **Scrollspy** nav with active section highlighting + mobile menu
- **Light / dark theme** toggle (persisted, respects system preference)
- **Contact form** that composes a `mailto:` link
- Fully responsive + print-friendly + `prefers-reduced-motion` support

## Deploy to GitHub Pages

The folder is ready to be served as a GitHub Pages site.

### Option 1 — New repository (recommended)

```bash
cd tannu-portfolio
git init
git add .
git commit -m "Initial Taranpreet Kaur portfolio"
git branch -M main
gh repo create raahuldhiman-dev/tannu --public --clone=false
git push -u origin main
gh repo edit raahuldhiman-dev/tannu --source . --homepage https://raahuldhiman-dev.github.io/tannu/
gh api repos/raahuldhiman-dev/tannu/pages -method POST -field "source[branch]=main" -field "source[path]=/"
```

### Option 2 — Inside an existing GitHub repository

Copy the contents of `tannu-portfolio/` into the repo root or the `/docs` folder of your GitHub repository, then set **Settings → Pages → Source → Deploy from a branch → `main` → `/ (root)`** (or `/docs`).

## Before going live

- Replace `PORTFOLIO_EMAIL` in `assets/js/main.js` with the real professional email.
- Replace the LinkedIn placeholder in the contact section with the real profile URL.
- Confirm client permissions and anonymise figures before publishing case studies.
