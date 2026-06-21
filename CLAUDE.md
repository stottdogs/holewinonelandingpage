# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

A single-file static landing page for **HoleWinOne** — a hole-in-one jackpot game played on real golf courses. The entire site is `index.html`: no framework, no build step, no dependencies beyond Google Fonts.

## Deployment

The repo is connected to Vercel (`stottdogs/holewinonelandingpage`). Any push to `main` auto-deploys. There is no build command or output directory — Vercel serves `index.html` directly.

To push changes:
```bash
git add index.html
git commit -m "your message"
git push
```

## Site structure

All content lives in `index.html` in this order: Nav → Hero → How it works → Why it's legit → The Jackpot → FAQ → For Courses CTA → Footer.

**To change copy:** edit the visible text in the relevant HTML section. FAQ questions/answers are plain HTML in `.faq-item` divs — no JS data array to update separately.

**To change jackpot values:** the three constants at the top of the `<script>` block control the odometer:
```js
const TARGET = 3460;  // where the odometer animates to on load
const FLOOR  = 2500;  // displayed minimum ($2,500)
const CAP    = 5000;  // displayed maximum ($5,000)
```

**To add/remove FAQ items:** duplicate or delete a `.faq-item` div in the FAQ section. The accordion JS uses `querySelectorAll('.faq-btn')` so it picks up changes automatically.

## Brand

- **Colors:** Deep Emerald `#0C3A2C`, Jackpot Gold `#ECB22B`, Pitch Ink `#0A130F`, Warm Cream `#FBF8F0`
- **Fonts:** Archivo (headlines/wordmark, 800–900 weight), Space Grotesk (body/UI), Space Mono (labels/captions)
- **Logo:** SVG concentric circles (target/coin mark) + wordmark with `WIN` in a gold box (`.win-box`)
- The `/for-courses` route is linked throughout but doesn't exist yet — it's a placeholder for a future page

## Design source

Original designs are in `project/` as `.dc.html` files (Claude Design Component format — not standard HTML). `project/HoleWinOne Landing.dc.html` is the source for `index.html`. `project/HoleWinOne Brand Sheet.dc.html` contains the full brand system reference.
