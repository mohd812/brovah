# Brovah Design System

Source of truth: `brand/Brovah_BRAND_GUIDELINES_2024.pdf` and `brand/BROVAH Company Profile (2026).pdf`.
Implemented as CSS custom properties in [`assets/brovah.css`](assets/brovah.css).

Brand personality: **"More than a studio."** Confident, structured, creative. Big bold
headlines, generous dark space, gold used as the voice — never as decoration everywhere.

---

## 1. Logo

Horizontal lockup (wordmark + equalizer symbol). Files in `assets/`:

| File | Fill | Use on |
|---|---|---|
| `logo-gold.svg` | Old Gold `#CCAF2D` | Dark Purple backgrounds (primary use) |
| `logo-white.svg` | `#FFFFFF` | Dark backgrounds / photography |
| `logo-dark.svg` | Dark Purple `#18162A` | Light / gold backgrounds |

Rules (from guidelines):
- Minimum clear space around the logo ≈ the width of one symbol bar ("x") on all sides.
- Never recolor outside the four approved fills (gold, white, dark purple, black), never
  stretch, never add effects.
- The standalone equalizer symbol may be used alone (favicon, avatars, pattern).

## 2. Color

| Token | Hex | Name | Role |
|---|---|---|---|
| `--brovah-gold` | `#CCAF2D` | Old Gold | Primary accent: headlines, CTAs, links, highlights |
| `--brovah-purple` | `#18162A` | Dark Purple | Primary background / text-on-light |
| `--brovah-gold-50` | `#E6D796` | Old Gold 50% | Subtle tints, hover states, borders on light |
| `--brovah-purple-50` | `#8C8B95` | Dark Purple 50% | Muted text on dark, secondary UI |
| `--brovah-white` | `#FFFFFF` | White | Body text on dark, light surfaces |

Usage ratio (mirrors the brand guidelines): dark purple dominates as ground, gold is the
accent voice, white carries body copy. Gold-on-purple and purple-on-gold are the two
signature pairings — both pass WCAG AA for text.

Gradient (pattern accent only, not for text): `linear-gradient(90deg, transparent, #CCAF2D)`
— the "gold ribbon" from the brand pattern pages.

## 3. Typography

**Rubik** (Google Fonts) for both English and Arabic — the corporate typeface for all
brand communication.

Weights: **Bold 700**, SemiBold 600, Medium 500, Regular 400. (Use all four for hierarchy;
nothing lighter than 400.)

| Style | Size (rem, clamp on web) | Weight | Case |
|---|---|---|---|
| Display / hero | clamp(2.75rem – 5.5rem) | 700 | UPPERCASE, tight leading (1.0–1.1) |
| H2 section | clamp(2rem – 3rem) | 700 | UPPERCASE |
| H3 card title | 1.25rem | 600 | Title case |
| Body | 1rem–1.125rem | 400 | Sentence case, line-height 1.6 |
| Label / eyebrow | 0.8125rem | 600 | UPPERCASE, letter-spacing 0.1em, gold |
| Stat number | clamp(2.5rem – 3.5rem) | 700 | Prefixed with `+` (e.g. `+250`) |

Headline pattern from the profile: oversized uppercase display type, sometimes with the
section label as a small gold eyebrow above.

## 4. Spacing & Layout

- Base unit: **8px**. Scale: 8 / 16 / 24 / 32 / 48 / 64 / 96 / 128.
- Content max-width: **1100px**, side padding 24px (mobile) / 48px (desktop).
- Sections separated by 96–128px vertical rhythm on desktop, 64px mobile.
- Corner radius: **8px** cards, **999px** pills/buttons. The brand is mostly rectilinear —
  keep radii small.

## 5. Components

- **Button (primary)**: gold background, dark-purple text, 600 weight, pill radius,
  darkens slightly on hover.
- **Button (ghost)**: 1px `--brovah-purple-50` border on dark, white text, gold border on hover.
- **Card**: slightly lighter purple surface (`#211E38`), 1px border `#2E2B47`, 8px radius.
- **Stat**: `+NUMBER` in gold 700 with an uppercase white label beneath.
- **Eyebrow label**: small uppercase gold text above section headings.
- **Client chip**: bordered pill with client name, muted → white on hover.

## 6. Pattern & Motifs

- **Equalizer bars**: the symbol may repeat as a decorative pattern (see guidelines
  "Pattern" pages) in gold on white/purple.
- **Gold gradient ribbons**: horizontal bars fading transparent → gold, staggered;
  used as section dividers or hero backdrop, always behind content, low quantity.
- **Timeline dots**: gold circles connected by a line — used for the 7-step process.

## 7. Voice & Content

- Tagline: **"More than a studio!"** · Social line: **"Where Creativity Resonates"**
- Positioning: forward-thinking music & audio production studio, Riyadh (Diplomatic
  Quarter, al-Mashtal Creative Space), serving Saudi Arabia, MENA and beyond.
- Values: authenticity, creativity, excellence, respect, long-term impact.
  "Creativity meets discipline" — every project is both art and business.
- Bilingual-ready: Rubik supports Arabic; keep layouts mirrorable for future RTL.

## 8. Contact block (canonical data)

- Email: `info@brovah.com` · Phone: `+966 55 632 2154`
- Instagram/TikTok/X: `@brovahstudio` · Web: `brovah.com`
- Location: Diplomatic Quarter, Riyadh, Saudi Arabia — al-Mashtal Creative Space
