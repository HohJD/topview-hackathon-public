# AI Video Hackathon KL

Public landing page for AI Video Hackathon KL, hosted by Topview at the AWS Office, Kuala Lumpur.

- **Date:** Sunday 6 September 2026
- **Hours:** 08:45 to 18:00
- **Prizes:** RM2,000 / RM1,000 / RM500

## Status

Public facing. Static single-file site (`index.html`), no build step.

The only external dependency is Google Fonts (Inter, Roboto Mono), loaded over
CDN. Everything else is inline.

Registration goes to Luma: https://luma.com/9z2e5zfv (nav button, hero
announcement pill, hero CTA and closing CTA all point there).

## Design

The page follows the design language of [Cruip's Simple Light landing page
template](https://github.com/cruip/tailwind-landing-page-template), ported from
Tailwind to plain CSS because there is no build step here. What was carried over:

- hairline rules that fade out at both ends, framing the eyebrow, headline and button row
- a floating pill header with a gradient border drawn by a masked pseudo element
- large, heavily blurred colour orbs behind the hero
- vertical stripes, masked so they fade downward
- dark console panels sitting inside a crosshair rule frame
- Inter throughout at tight tracking, Roboto Mono for micro labels

The template's blue becomes the Topview brand violet, `#731DFB`. Because violet
is far more saturated than that blue, the orb and stripe opacities are dialled
back from the template's values.

## Theme

Dark is the default and the system colour-scheme preference is deliberately not
consulted. The toggle in the header switches to light and the choice is remembered
in `localStorage` under `tv-theme`.

## Local preview

```
npx serve .
```

## Deploy

Deployed on Vercel as a static site. Root directory is the repo root, no build command.
