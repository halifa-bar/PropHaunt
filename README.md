# PropHaunt — Marketing Site

A single-page, **zero-build** landing site for the PropHaunt game. Pure HTML + CSS
(hand-written, no framework, no build step). Only external dependency is Google Fonts.

## View it

Just open `index.html` in any browser — double-click it, or:

```powershell
start index.html
```

## Files

```
PropHaunt/
├── index.html              ← the whole site (HTML + CSS + a little JS)
├── assets/
│   ├── logo.png            ← PropHaunt app icon (favicon / header)
│   ├── hero-banner.png     ← MAIN green wordmark artwork (you add this — see below)
│   └── characters/         ← character portraits (from the game)
│       ├── chris.png  amanda.png  david.png  nikki.png  butcher.png
├── DESIGN.md               ← design system reference (palette, fonts, layout)
└── README.md
```

## Add the hero artwork

The hero uses the green "PropHaunt" wordmark image. Save that artwork as:

```
assets/hero-banner.png
```

It then appears as the main banner. Until the file exists, the page falls back to
the square logo + text title automatically (no broken image).

## Before you publish — fill these in

Search `index.html` for `TODO` (two spots) and replace `href="#"` with your real URLs:

1. **Request Playtest Access** → your Steam playtest "Request Access" link.
2. **Wishlist on Steam** → your Steam store page URL.

(The header "Get Access" button and the hero buttons jump to the `#playtest` section,
which holds these two real links — update them once and the page is done.)

## Hosting (free options, no domain needed)

The site is fully static, so you can drop the folder onto any of these:

- **GitHub Pages** — push the folder to a repo, enable Pages on the `main` branch.
- **Netlify / Vercel / Cloudflare Pages** — drag-and-drop the folder, get a free `*.netlify.app` URL.
- **itch.io** — zip the folder and upload as an HTML project.

When you get a domain later, point it at whichever host you picked.

## Notes

- Colors / fonts were generated with the `ui-ux-pro-max` skill and tuned to the game's
  real brand (blood-red killer, carnival gold, eerie purple). See `DESIGN.md`.
- Respects `prefers-reduced-motion`, uses semantic HTML, SVG icons (no emoji), and
  AA-contrast text.
- Survivor/killer ability names match the in-game loadouts.
