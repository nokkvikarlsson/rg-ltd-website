# rg-ltd.com website — design

## Purpose
A single-page company site for Renown Global Limited, aimed at business partners
(e.g. Safaricom) evaluating whether the company is a legitimate, real entity —
not a consumer marketing site.

## Content & structure
Single scrolling page, no multi-page nav:
- **Hero** — Renown Global name/mark + one-line tagline
- **About** — short company blurb: mobile games company, based in Nairobi, Kenya
- **Product** — Matatu Madness callout: icon, one-line description, "closed beta"
  badge (swap to a Play Store link once public)
- **Contact** — nokkvi@rg-ltd.com
- **Footer** — "Renown Global Limited · Nairobi, Kenya" + link to privacy.rg-ltd.com

## Visual style
Hybrid direction: simplified circular monogram (not the full cartoon globe logo
used in-game), clean sans-serif type, generous whitespace. Brand colors (blue
#4A9FE8, green #5CB85C, gold #F5C518) used only as accents (underline, button,
small details) — credible first, "on-brand" second.

## Tech & hosting
Plain static HTML/CSS, no build step or framework — same pattern as the existing
`matatu-madness-privacy` repo. New GitHub repo `rg-ltd-website`, deployed via
GitHub Pages with a `CNAME` file for `rg-ltd.com`. DNS cutover: update the apex
`A` records and `www` CNAME in Squarespace's DNS panel to point at GitHub Pages,
same as `privacy.rg-ltd.com` already does. No Squarespace website subscription
needed — domain stays registered there, only DNS is touched.

## Out of scope
Multi-page site, CMS/build tooling, analytics, contact form (plain mailto link
instead), Play Store link (added later once public).
