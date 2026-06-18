# PropHaunt — Design System

Generated with the `ui-ux-pro-max` skill (gaming / horror / immersive) and tuned to
the game's real brand. Use this as the source of truth when adding pages or sections.

## Direction
- **Pattern:** Scroll-triggered storytelling — sections build intensity, CTA repeats at the end.
- **Style:** Dark, cinematic, immersive "carnival horror" (atmosphere via CSS gradients,
  fog, grain, glow — no heavy WebGL, kept zero-build & performant).
- **Mood:** dark, eerie, a little playful-creepy.

## Color tokens (CSS variables in `index.html`)
| Token | Hex | Use |
|-------|-----|-----|
| `--bg` | `#0A0810` | page background (near-black) |
| `--surface` | `#150F20` | cards |
| `--surface-2` | `#1C1430` | raised cards |
| `--border` | `#2C2240` | borders/dividers |
| `--text` | `#ECE6F2` | body text |
| `--text-muted` | `#9C93AE` | secondary text |
| `--red` / `--red-2` | `#E11D2E` / `#FF3B4E` | **killer, danger, primary CTA** |
| `--amber` / `--amber-2` | `#FFC23D` / `#FFD86B` | **carnival gold, highlights, "hope"** |
| `--purple` | `#8B5CF6` | eerie atmospheric glow only |

> The skill's raw suggestion was neon-purple + rose. It was re-weighted toward the game's
> existing identity: blood-red (the in-game killer color) + carnival gold (the in-game
> yellow accent), with purple kept as background atmosphere.

## Typography (Google Fonts)
- **Headings / display:** `Russo One` — bold, geometric, "game logo" energy.
- **Body / UI:** `Chakra Petch` — techy, slightly squared, readable.
- Import: `https://fonts.googleapis.com/css2?family=Chakra+Petch:wght@400;500;600;700&family=Russo+One&display=swap`

## Section layout (one page)
1. **Hero** — logo, title, tagline "Hide. Repair. Escape.", premise, 2 CTAs.
2. **How to Play** — 3 steps: Disguise / Repair / Escape.
3. **The Butcher** — killer feature + abilities (Bear Trap, Sense Pulse).
4. **Survivors** — 4 character cards with real in-game ability names.
5. **Features** — multiplayer, proximity voice, prop physics, the Carnival.
6. **Finale CTA** — repeat Request Access + Wishlist.
7. **Footer**.

## Rules to keep (from the skill's checklist)
- SVG icons only — no emoji as icons.
- `cursor-pointer` + visible focus rings on all interactive elements.
- Hover transitions 150–300ms.
- Respect `prefers-reduced-motion`.
- Body text contrast ≥ 4.5:1.
- Responsive at 375 / 768 / 1024 / 1440 px.
- Avoid: minimalist/flat look, static-only assets (keep depth + motion).
