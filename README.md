# HANGOVR 180 — Brand Site

**Live URL:** Deployed on Vercel  
**Version:** 4.3  
**Last updated:** April 15, 2026

## Overview
Static marketing site for HANGOVR 180, a pre-alcohol supplement brand based in Austin, TX.

## Tech Stack
- Static HTML/CSS (no framework, no build tools)
- Font: Montserrat (Google Fonts)
- Hosting: Vercel (auto-deploys from this repo)
- Images: WebP with `<picture>` art direction

## Button System (v4.3)
Two CTA classes replace all previous button variants:
- `.btn-cta-light` — red CTA on light backgrounds, hovers to dark
- `.btn-cta-dark` — red CTA on dark backgrounds, hovers to yellow
- `.card__btn` — full-width red on product cards, hovers to dark

## Nav Clarifiers (v4.3)
- Desktop: hover tooltips below each nav link
- Mobile: persistent subtext below each hamburger menu link
- HOME link added as first entry in mobile menu

## v4.3 Changes
- Button color standardization (site-wide, 10 buttons remapped)
- Text size standards applied across all pages
- Tension image border removed (index.html)
- Pack section: "Simply," deleted, headline/body rewritten, button standardized
- Email body line deleted (index.html)
- Review stars doubled (2.5rem), rating numbers added, names doubled (1.75rem)
- Identity section line break after "It is THE move."
- Portrait borders removed, captions flush to images
- Bento body bolded + text standard applied
- Stock Up hero subtext max-width removed
- Products heading restyled to match section headline standard
- Nav clarifier tooltips (desktop) and subtext (mobile) added

## Deployment
Push to main branch. Vercel auto-deploys. No vercel.json.
