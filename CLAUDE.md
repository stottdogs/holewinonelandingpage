# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

A single-file static landing page for **holeWINone** — a hole-in-one jackpot game played on real golf courses. The entire site is `index.html`: no framework, no build step, no dependencies beyond Google Fonts. `HoleWinOneVideo.mp4` is the hero video served alongside it.

## Deployment

Live at **holewinone.com**. Connected to Vercel (`stottdogs/holewinonelandingpage`) — any push to `main` auto-deploys in ~1 minute. No build command or output directory.

```bash
git add index.html   # (or other changed files)
git commit -m "your message"
git push
```

## Site structure

All content lives in `index.html` in this order: Nav → Hero (video) → How it works → Why it's legit → The Jackpot → FAQ → For Courses CTA → Footer.

**To change copy:** edit the visible text in the relevant HTML section. FAQ items are plain `.faq-item` divs — the accordion JS picks up changes automatically via `querySelectorAll('.faq-btn')`.

**To change jackpot values:** three constants at the top of the `<script>` block:
```js
const TARGET = 3460;  // odometer animates to this on load
const FLOOR  = 2500;  // displayed minimum
const CAP    = 5000;  // displayed maximum
```

**"For Courses" nav button** scrolls to `#courses` (the partner CTA section at the bottom). There is no `/for-courses` page yet — all those links point to `#courses` as a placeholder.

## Brand

- **Name:** always written `holeWINone` — lowercase h and o, WIN in caps (rendered with `.win-box` gold pill in HTML)
- **Colors:** Deep Emerald `#0C3A2C`, Jackpot Gold `#ECB22B`, Pitch Ink `#0A130F`, Warm Cream `#FBF8F0`
- **Fonts:** Archivo (headlines/wordmark, 800–900 weight), Space Grotesk (body/UI), Space Mono (labels/captions)
- **Tone:** no em dashes. Punchy, confident, golf-native. Don't mention sensors — the hardware is a camera only.
- **Contact:** `hello@holewinone.com`

## Design source

Original designs are in `project/` as `.dc.html` files (Claude Design Component format). `project/HoleWinOne Landing.dc.html` is the source for `index.html`. `project/HoleWinOne Brand Sheet.dc.html` has the full brand reference.
