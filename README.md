# Marrolo — Contemporary Fashion Design

Portfolio and brand website for **Marrolo**, a contemporary fashion label built around original garments, expressive visuals, and modern editorial culture. Designed and developed by the founder.

---

## Overview

Marrolo is a static, no-framework website — pure HTML, CSS, and vanilla JavaScript. No build step, no dependencies, no bundler. Open `index.html` in a browser and it works.

The site is fully bilingual (English / Spanish), supports light and dark mode, and is optimized for desktop and mobile.

---

## Pages

| File | Description |
|---|---|
| `index.html` | Main brand page — hero, collections, designer story, lookbook, merch, contact |
| `portfolio.html` | Portfolio page — fashion runway projects with sidebar navigation |

---

## Features

- **Dark / Light mode** — respects `prefers-color-scheme` on first visit; persisted in `localStorage`
- **Bilingual (EN / ES)** — full translation of all UI strings; language persisted in `localStorage`
- **Designer Story image stack** — 3-photo fan display with 3D CSS transforms, autoplay, and prev/next navigation
- **Collection carousel** — per-card image slideshow for the No Time 4 Love collection
- **Merch carousel** — paginated two-up grid with prev/next controls and slide counter
- **Marrolo Lovers carousel** — single-image portrait carousel
- **SVG follower** — interactive paint-trail cursor effect on the about, lookbook, and merch sections
- **Bouncing balls canvas** — animated particle background on the intro band and contact sections
- **Custom cursor** — red dot + ring with lag and hover scale; dark-mode flashlight spotlight overlay
- **Scroll reveal** — `IntersectionObserver`-based fade-in for all major content blocks
- **Portfolio scrollspy** — sidebar links highlight the active section on scroll
- **Responsive** — breakpoints at 860px and 560px; mobile navigation via full-screen overlay menu

---

## Project Structure

```
Marrolo/
├── index.html
├── portfolio.html
├── styles.css
├── script.js
└── assets/
    ├── marrolo-hero.JPG
    ├── marroloLogoBlack.png
    ├── marroloLogoWhite.png
    ├── happyMarrolo.png
    ├── designer-studio.svg
    ├── collection-*.svg
    ├── lookbook-*.svg
    ├── designerStory/          # Designer story section photos
    │   ├── IMG_0686.JPG
    │   ├── IMG_6328.JPG
    │   └── IMG_8418.jpg
    ├── noTimeForLoveCollection/
    ├── marroloLovers/
    ├── merch/
    └── portfolio/
        ├── imOkFashionRunway/
        └── readyToLoveFashionRunway/
```

---

## Typography & Colors

| Token | Value | Usage |
|---|---|---|
| `--ink` | `#0a0a0a` / `#f0f0f0` dark | Primary text |
| `--paper` | `#ffffff` / `#0c0c0c` dark | Background |
| `--red` | `#8c1828` | Brand accent, eyebrows, cursor |
| `--blue` | `#1e3a8a` | Store callout, collection index |
| `--yellow` | `#f5c800` | Ticker, principle numbers, hover highlights |
| `--pink` | `#e8729e` | Contact eyebrow |

**Fonts:** Cormorant Garamond (headings, italic) · Space Grotesk (body, UI) — loaded via Google Fonts.

---

## How to Run

No build step required.

```bash
# Option 1 — open directly
open index.html

# Option 2 — local server (avoids any file:// restrictions)
npx serve .
# or
python -m http.server 8080
```

---

## Browser Support

Modern evergreen browsers (Chrome, Firefox, Safari, Edge). The custom cursor is automatically disabled on touch devices (`pointer: coarse`).

---

## Brand

**Marrolo** — Vancouver, BC  
Contemporary fashion design · Made on demand · Moving between Mexico and Canada  
Contact: marrolo.can@gmail.com
