# Ebury Design System

A design system distilled from the **Ebury Brand Deck** (Figma). Ebury is a global fintech offering cross‑border payments, FX and working‑capital solutions — the deck template is the visual language used for pitch, investor and product presentations.

## Source Materials

- **Figma file:** *Brand Deck.fig* (mounted as VFS during authoring). 1 page, 1 top‑level frame, ~32 slide masters.
- **Scope:** 1920×1080 landscape presentation template. No product/app UI; no marketing web surfaces were provided.
- Type: **KMR Apparat** (display) + **Inter** (body). KMR Apparat is a commercial Kometa Studio face; we substitute a close Google Font — see Caveats.
- Image assets are mostly lifestyle/stock photography placeholders (`image/jpeg`) embedded inside the Figma file.

## Brand Snapshot

Ebury positions itself as a **next‑gen financial platform** for global growth — cross‑border payments, FX risk management, trade finance. The deck reads as **calm, institutional, confident** — editorial more than marketing. Lots of whitespace, big numbers, big typography, restrained palette (charcoal / cream / dusty blue). No emoji, no gradients beyond a single blue fade used on diagrams, no cute illustrations.

## Products Represented

This file represents **one surface**: the corporate slide deck template. No app, no web, no email. Anything outside of slides is an extension and should be flagged.

## CONTENT FUNDAMENTALS

How copy is written in Ebury materials, based on the deck template and ebury.com voice:

- **Voice:** Third‑person authoritative for headlines; second person (you / your) when addressing the customer directly. *"Open your account with Ebury and unleash your global growth potential."*
- **Tone:** Confident, expert, unhyped. Avoids adjectives like "amazing" / "revolutionary"; prefers **concrete nouns** (account, platform, payments, FX, liquidity, risk).
- **Casing:** Sentence case for titles — *"Experience the next‑gen financial platform"*. Never title‑case or ALL CAPS in body. Numeric labels use uppercase (01, 02) as a layout device.
- **Sentence length:** Short and declarative. Marketing claims are 4–8 words.
- **Numbers:** Hero stats are a core device — big KMR Apparat number + short label (e.g. *"$30Bn Traded annually"*, *"24 Offices worldwide"*).
- **Emoji:** Never.
- **Punctuation:** Minimal. Periods optional on short display lines. Pipe separators for contact info: *"info@ebury.com | ebury.com"*.
- **Naming:** The product wordmark is **lowercase** (`ebury`). The company name in body copy is capitalised (*Ebury*).
- **Legal / boilerplate:** Quiet, small, bottom‑left or back‑cover. No exclamation marks anywhere.

## VISUAL FOUNDATIONS

- **Palette:** Four functional families.
  1. *Charcoal* `#231F20` — default text, dark backgrounds, bar‑chart anchors.
  2. *Cream / off‑white* `#F5F5F5`, `#F7F7F7` — default slide background (NOT pure white).
  3. *Ebury blue* `#74B0CA` — hero accent, chart primary, cover slides. Tints `#B4D4E2`, `#ACD0DF`, `#BAD7E5` used on diagrams.
  4. *Deep navy* `#234862` — secondary chart colour paired with Ebury blue.
  5. *Mint accent* `#9FF6F3` — sparingly for highlight blocks/tracker states.
- **Type:** KMR Apparat for display (46 / 75 / 120 / 180 px). Inter Medium 22/28 for subtitles + bullets. Inter Regular 14/16/20 for body and captions. Line‑height tight on display (0.9), comfortable on body (1.2).
- **Background treatments:** Solid flat fills — cream, charcoal, or Ebury blue. Occasional full‑bleed lifestyle photography (warm, natural light, global scenes — never AI‑looking). No gradients on backgrounds; one subtle blue→transparent fade is used on progress bars and ring diagrams only.
- **Spacing:** 1920×1080 canvas, **96 px** gutters left/right, **96 px** from top for title. Card inset is typically **16–24 px**; inter‑card gaps **24–48 px**.
- **Corner radii:** `10 px` for content cards/chart frames. `0 px` (square) for photos. Large image blocks occasionally use `10 px` as well.
- **Borders:** Hairline `1 px` dividers at 1/3 and 5/6 of the canvas on cover slides (vertical rules). Table rows separated with `1 px rgba(116,116,116,0.5)`.
- **Shadows:** Slide shadow for preview only — `0 5px 20px rgba(0,0,0,.1), 0 0 3px rgba(0,0,0,.3)`. Content cards generally FLAT (no shadow) on the cream background.
- **Inner shadows / gradients:** Diagrams use a subtle linear gradient from Ebury blue → lighter tint, sometimes with a soft inner glow. Not used elsewhere.
- **Transparency / blur:** Almost absent. Header chips sometimes layer a 15 % white over charcoal.
- **Cards:** `rgb(224,224,224)` light‑gray panel, 10 px radius, flat. Inside, a clean figure/chart + caption.
- **Imagery vibe:** Warm, natural daylight. Global / urban / travel / portrait. Shot feel, not rendered. No duotone, no grain filter.
- **Animation:** Print‑first; no motion language specified in the Figma. We add minimal fades (120 ms ease‑out) on prototype demos and flag.
- **Hover / press:** Not defined in a deck. For HTML prototypes we use `opacity .85` on hover, `scale(.98)` on press — flagged.
- **Layout rules:** Title TOP‑LEFT at (96, 96). Subtitle right‑side at same baseline. Content block starts y ≈ 248 px. Page furniture (page #, wordmark) lives along the bottom.
- **Fixed elements:** Wordmark `ebury` bottom‑right on cover slides. Hairline vertical rule at 1214 px separates content from wordmark.
- **Iconography vibe:** Light‑weight line icons drawn in a square 80×80 tile, charcoal stroke ~4 px, no fill. Always inside a 80×80 or 144×144 light‑gray card.

## ICONOGRAPHY

The deck ships a small icon set (≈9 glyphs) used on stat cards: `building`, `person`, `currency pound`, `currency dollar`, `globe`, `headphones/support`, `adjust/controls`, `fast/speed/ray`, `umbrella/hedge`, `EU flag`. All are **SVG, line style, uniform stroke**, sit inside a `144×144` light‑gray tile with `10 px` radius.

Because the Figma glyphs are proprietary recreations, we **substitute with Lucide** (line, 2 px stroke, square corners) as the working icon set — the nearest visual match on a CDN. Substitution is flagged; swap back to the Figma SVGs by copying them into `assets/icons/` and updating `ui_kits/*` imports.

- **Emoji:** Never.
- **Unicode arrows:** A long right arrow (`→`) is used as the bullet marker in body copy. This is allowed.
- **Flags:** The EU flag is a real colored SVG; treat country flags as illustrations, not icons.

## Index

Root files:
- `README.md` — this file
- `SKILL.md` — agent‑compatible skill manifest
- `colors_and_type.css` — raw tokens + semantic CSS vars

Folders:
- `fonts/` — **KMR Apparat** (7 weights, 300–900) self-hosted `.ttf`
- `assets/logo/ebury-logo.svg` — official black wordmark (invert for dark bg)
- `assets/icons/` — line-style SVG icon set (building, person, globe, currency-dollar, currency-pound, umbrella)
- `preview/` — one card per design-system concept. `logo`, `colors-primary`, `colors-blue-scale`, `colors-neutrals`, `type-display`, `type-body`, `type-hero-number`, `iconography`, `chips`, `stat-cards`, `bullet-list`, `spacing`, `radii-shadow`, `chart-swatch`
- `slides/` — 1920×1080 templates: `01-title`, `02-bullets-chart`, `03-stats-grid`, `04-big-quote`, `05-section-divider`, `06-agenda`, `07-closing`. All share `slide.css`.

No UI kit folders exist — the source file is a slide template, not a product UI. If you need a web/app kit, ask for those Figma files or codebase.

## Caveats / Open Questions

- **KMR Apparat** — full weight family (Light 300 → Black 900) loaded from `fonts/KMR-Apparat-*.ttf`. Display headings default to 300 Light to match Figma renderings.
- **Ebury wordmark** — real SVG at `assets/logo/ebury-logo.svg`. Use `<img>` + `filter:invert(1)` on dark backgrounds. A white-on-dark variant from Frontify would remove the need for the invert filter.
- **Icon set** — currently line-style SVGs in `assets/icons/` (building, person, globe, currency, umbrella). The real Figma deck uses them inside `86×86` rounded-square tiles (light blue `#74B0CA` for "soft", navy `#234862` for "strong") at `11 px` radius. Pattern captured in the stats grid / flow slides.
- **Brand portal (Frontify)** — `brand.ebury.com` is blocked from the authoring sandbox's allow-list. Any additional brand assets (white logo variants, official color/type specs, imagery) must be uploaded via the Import menu.
- **Platform design system (Storybook)** — `design-system.web.ebury.rocks` is a client-side SPA; the HTTP fetch returns only the shell. Component styles must be mirrored by hand from specific story URLs or pasted devtools output.
- **Imagery** — no production imagery shipped. Full-bleed photo slides use placeholder blocks.
- **Motion spec** — none in Figma. Any prototype animation is ours and should be reviewed.

## Known fixes applied during authoring

- Scaler bug — `.scaler` now uses negative margins instead of `translate(-50%, -50%) scale()`, so slides no longer clip on narrow viewports ("only a corner loading").
- Type-wordmark → real SVG logo across every slide and preview card.
- Stats grid rebuilt to match the real Figma design (3×3 white-bordered cells on `#231F20`, KMR Apparat 120px in `#74B0CA`, white labels).
