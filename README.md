# Topview AI Video Hackathon

Public landing page for the AI Video Hackathon hosted by Topview AI at the AWS Office, Kuala Lumpur.

- **Date:** Sunday 6 September 2026
- **Hours:** 08:45 to 18:00
- **Prizes:** RM2,000 / RM1,000 / RM500

## Status

Public facing. Static single-file site (`index.html`), no build step.

The only external dependency is Google Fonts (Archivo, Inter, JetBrains Mono),
loaded over CDN. Everything else is inline.

Registration links are still placeholders pointing at `#register`.

## Theme

Light is the default and the system colour-scheme preference is deliberately not
consulted. The toggle in the nav switches to dark and the choice is remembered in
`localStorage` under `tv-theme`.

## Local preview

```
npx serve .
```

## Deploy

Deployed on Vercel as a static site. Root directory is the repo root, no build command.
