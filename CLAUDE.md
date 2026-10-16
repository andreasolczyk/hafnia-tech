# Hafnia Technologies — hafnia.tech

Static website for Hafnia Technologies, hosted on GitHub Pages.

## How the site works

- Pushing to `main` publishes the site within a minute or two. Treat every push to `main` as going live.
- Keep all site files in the repository root. Do not move or delete `CNAME` (it holds the custom domain `hafnia.tech`).
- No build step, no frameworks and no outside requests: the font is embedded in `index.html` as base64, and the logo animation is plain JavaScript and SVG. Keep it that way unless asked.
- Respect `prefers-reduced-motion`: with reduced motion, show the finished logo without animation.
- When changing visible text, also update the matching `<meta name="description">` and `<meta property="og:description">` in `<head>`.

## Brand essentials

The full brand guide is the "Hafnia Technologies" design system on claude.ai. These are the rules that matter most here.

**Voice:** calm and precise, Scandinavian. Short plain sentences, concrete details over adjectives, sentence case, no emoji or hype words, at most one exclamation mark per page.

**Colours** (dark is the primary theme):

| Role | Dark | Light |
| --- | --- | --- |
| Page ground (`surface`) | `#1E2023` | `#F1ECE8` |
| Raised panels (`surface-raised`) | `#25282B` | `#FAF7F4` |
| Main text (`text`) | `#EFE8E3` | `#2A2D30` |
| Secondary text (`text-muted`) | `#B9B0AA` | `#5A5650` |
| Labels, footers (`text-faint`) | `#99918B` | `#6B655F` |
| Links, buttons, focus (`accent`) | `#E05C72` | `#9B1B30` |
| Text on accent fills (`on-accent`) | `#1E2023` | `#EFE8E3` |

- The logo's H is always ruby `#9B1B30`, with a `#EFE8E3` drop above the centre (`#CFC8C2` on light grounds) and a `#3A3E42` drop below.
- Never use the bright ruby `#E05C72` in the logo, and never use `#9B1B30` as small text on dark grounds.
- Keep ruby to about 5–10% of a page.

**Type:** Plus Jakarta Sans only, weights 300/400/600/700. "Hafnia" in 700 and "Technologies" in 300. Body text 17px with 1.6 line height, lines near 65 characters.

**Backgrounds:** dark grounds get a fine grain overlay (about 0.22 opacity, overlay blend) and one or two soft ruby glows from opposite corners. No other gradients, no stock photos, no drop shadows.

**Motion:** the liquid-node logo animation once per page. Connected drops always share one colour. Interface transitions stay at 150–250 ms.
