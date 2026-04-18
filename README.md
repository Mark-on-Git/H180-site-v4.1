# HANGOVR 180 — Brand Site

**Live URL:** Deployed on Vercel  
**Version:** 4.4  
**Last updated:** April 16, 2026

## Overview
Static marketing site for HANGOVR 180, a pre-alcohol supplement brand based in Austin, TX.

## Button System (v4.4)
- `.btn-cta-light` — Red CTA on light backgrounds → dark hover
- `.btn-cta-dark` — Red CTA on dark backgrounds → yellow hover  
- `.btn-signup` — Dark/yellow default → red hover (signup + cart actions)
- `.card__btn` — Dark/yellow full-width → red hover (product cards)

## v4.4 Changes (Master Build v5)

### Site-wide
- Hero scaling: center-left anchor (`object-position:center left`) adopted as default
- Mobile typography: increased clamp minimums, bottom padding with `env(safe-area-inset-bottom)`
- btn-signup class added for "I'M IN" and cart buttons (dark/yellow default)
- Nav tooltips: 0.5s hover delay + fade animation, white bg/black text
- Footer logo: 2× height (3.5rem → 7rem)

### Home
- Tension: border removed, unified scaling
- Pack: "Simply," deleted, headline/body rewritten
- Email: body line removed, button → btn-signup

### Do A 180
- Hero: "WHO'S IN" CTA button removed entirely
- Reviews: star overflow fixed (flex-shrink:0), 3→2→1 column at 1200/768
- Reviews: mouse drag + arrow key navigation added
- Reviews: getPerPage() uses 1200/768 thresholds

### Tomorrow People
- Identity: headline reduced at max width (3.5rem max vs 4.5rem), full empty line break
- Portraits: breakpoints at 1400px (4-col) and 850px (2-col), no borders, flush captions
- Bento: "STAY" bolded only, rest at weight 400

### What's Inside
- Patent section: "Real Science. Three ingredients. Nothing else." as hook
- "Patent Pending" on own line in red
- Clinical cards: square aspect ratio locked
- Product/Protocol: breakpoint moved to 1400px, headline overflow protection

### Find Us
- Wild gallery: stays 2×2 at 768px+
- Events button: btn-signup

### Stock Up
- Hero sub: max-width removed
- Products title: section headline standard
- Card buttons: card__btn (dark/yellow)

## Deployment
Push to main. Vercel auto-deploys. No vercel.json.
