# HANGOVR 180 — Brand Site

**Live URL:** Deployed on Vercel  
**Version:** 4.2  
**Last updated:** April 15, 2026

## Overview

Static marketing site for HANGOVR 180, a pre-alcohol supplement brand based in Austin, TX.

## Tech Stack

- Static HTML/CSS (no framework, no build tools)
- Font: Montserrat (Google Fonts)
- Hosting: Vercel (auto-deploys from this repo)
- Images: WebP with `<picture>` art direction (portrait/landscape/desktop)

## Structure

```
/
├── index.html          Home
├── doa180.html         Do A 180
├── whos-in.html        Tomorrow People
├── inside.html         What's Inside
├── find-us.html        Find Us
├── stock-up.html       Stock Up
├── global.css          Shared styles (nav, buttons, footer, resets)
└── images/             All site images (44 WebP + 2 SVG)
```

## Brand Colors

| Name   | Hex       |
|--------|-----------|
| Yellow | `#FFD800` |
| Black  | `#303633` |
| Red    | `#C7084F` |
| White  | `#FFFFFF` |

## Deployment

Push to main branch. Vercel auto-deploys.

## Breakpoint System (v4.2)

Three tiers:
- **768px** — 2-column content layouts (text+image, text+text), form rows, simple horizontal arrangements
- **768–1023px** — Intermediate 2-col grids for portraits, gallery, products (landscape phone gets a reasonable middle ground)
- **1024px** — Nav links, footer row, 3/4-col grids, generous padding, headline size bumps

Principle: if you're holding a phone (any orientation), max 2 columns. 3+ columns only on tablets and desktops.

## v4.2 Changes (Breakpoint Fix)

Every `@media(min-width:768px)` rule audited and split:

**Moved to 1024px:** All 3-col and 4-col grids, all 6rem+ padding, hero headline size bumps, footer horizontal layout, review 3-up cards, steps 3-col, clinical 3-col, product min-heights

**Kept at 768px:** All 2-col content pairs (text+image, text+text), form row layouts, reassurance row, review header row, biology 2-col, bento 2-col, product side-by-side frame

**Added at 768–1023px:** Intermediate 2-col grids for portraits, wild gallery, product cards

**JS fix:** Reviews carousel `getPerPage()` now uses 1024px threshold to match CSS

## Notes

- Material Symbols font loaded only on whos-in.html (rocket icon)
- Images folder ships empty — client adds 44 WebP + 2 SVG files
- Email signup forms are placeholder only
- Cart buttons link to stock-up.html (Shopify pending)
