# HANGOVR 180 — Brand Site

**Live URL:** Deployed on Vercel  
**Version:** 4.4  
**Last updated:** April 18, 2026

## Overview
Static marketing site for HANGOVR 180, a pre-alcohol supplement brand based in Austin, TX.

## Tech Stack
- Static HTML/CSS (no framework, no build tools)
- Font: Montserrat (Google Fonts)
- Hosting: Vercel (auto-deploys from this repo)
- Images: WebP with `<picture>` art direction

## Deployment
Push to main branch. Vercel auto-deploys. No vercel.json.

## v4.4 Changes (from v4.3 baseline)

1. **Home hero text size + position** — Headline minimum raised from 3.5rem to 4.5rem with 12vw scale. Added 768-1023px mid-range boost (5rem min). Bottom padding increased to 5rem + safe-area-inset.
2. **Home S2 tension scaling** — Removed fixed max-width:24rem from image frame. Image now fills its grid column at 768px+. Mobile gets centered 24rem max. Added align-self:center on image wrap.
3. **Home S3 pack zoom fix** — Removed min-height:100vh from pack grid. Added max-height:80vh on image at 768px+ so it scales down rather than cropping tight.
4. **Home S4 aboard hierarchy** — Boosted headline to clamp(3rem,8vw,4.5rem) below 1024px so it dominates the CTA button.
5. **DoA180 review stars overflow** — Reduced letter-spacing to 0 and gap to 0.1rem. Added overflow:hidden, flex-wrap:nowrap, max-width:100% on star row.
6. **Tomorrow People identity balance** — Reduced headline from clamp(2.5rem,6vw,4.5rem) to clamp(1.75rem,3.5vw,2.75rem) so headline and body text are balanced at all widths.
7. **Tomorrow People portrait order** — Verified: order:1/2 on img-wrap/caption in base styles, order:unset only at 1024px+. Sarah and Dr. Fumi render image-first at all sub-1024 widths. No change needed.
8. **Inside ingredient cards** — Added max-width:72rem on clinical grid at 1024px. Added mobile card constraints (min-height:20rem, max-width:32rem, centered).
9. **Inside Protocol headline clip** — Added overflow:hidden on headline. Added sub-1400px override reducing font to clamp(2rem,4vw,3rem).
10. **Stock Up hero subtext** — Widened hero content container from 64rem to 72rem to prevent "up yet." orphan.
