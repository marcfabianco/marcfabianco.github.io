# Visual Style Guide

This document defines the stylistic system for all public-facing materials (website, profile README, CV accents, slides, figures). It is about **look and feel** — not content.

---

## 1. Color palette

### Main colors

| Role          | Name           | Hex       | Use                                                                 |
|---------------|----------------|-----------|----------------------------------------------------------------------|
| Background    | Warm white     | `#F0F0EB` | Primary page background. Replaces pure white everywhere.            |
| Body text     | Dark text      | `#333333` | Headings and primary text. Never pure black.                        |
| Secondary     | Warm gray      | `#666663` | Subheadings, meta text, captions.                                   |
| Primary accent| Terracotta red | `#BF4D43` | Links, primary accents, eyebrow labels, section underlines.         |
| Secondary accent | Muted gold  | `#C9A84C` | Second accent — card tops, chart series, pull quotes.               |
| Tertiary accent | Sage green  | `#6B8F71` | Third accent — card tops, chart series, success states.             |

### Supporting colors

| Role         | Name       | Hex       | Use                                                              |
|--------------|------------|-----------|-------------------------------------------------------------------|
| Card surface | White      | `#FFFFFF` | Cards, tables, elevated surfaces against warm-white background.  |
| Muted line   | Light gray | `#999999` | Dividers, borders, footer text. Used at 20–40% opacity typically.|
| Soft accent  | Soft pink  | `#F5D0CC` | Subtle highlights, hover backgrounds, callout tints.             |

### Usage rules

- **Never use pure white (`#FFFFFF`) as page background** — always warm white.
- **Never use pure black (`#000000`) for text** — always dark text `#333333`.
- **One primary accent per component.** Terracotta is the default; gold and sage are for differentiation (e.g., a set of three cards).
- **Soft pink is for subtle emphasis only.** Never use as a primary surface.
- **Light gray dividers** should be `#999999` at ~25% opacity: `rgba(153,153,153,0.25)`.

---

## 2. Typography

### Families

- **Serif (display):** Cormorant Garamond — weights 500, 600, 700. Fallback: Georgia, "Times New Roman", serif.
- **Sans (body/UI):** Inter — weights 400, 500, 600. Fallback: -apple-system, BlinkMacSystemFont, "Helvetica Neue", Arial, sans-serif.

### Scale

| Token     | Size  | Family | Weight | Use                                |
|-----------|-------|--------|--------|-------------------------------------|
| Hero H1   | 56px  | Serif  | 600    | Name / primary hero title          |
| H2        | 32px  | Serif  | 600    | Section headings                   |
| H3        | 21px  | Serif  | 600    | Card / item titles                 |
| Body      | 17px  | Sans   | 400    | Paragraphs                         |
| Body lg   | 18px  | Sans   | 400    | About paragraph, lead text         |
| Meta      | 14–15px | Sans | 400    | Captions, metadata, secondary text |
| Eyebrow   | 13px  | Sans   | 600    | Uppercase label above title, 3px letter-spacing |
| Tagline   | 20px  | Serif italic | 500 | Subtitle under hero name        |

### Rules

- **Serif for anything that reads as a title.** Sans for anything that reads as UI or running prose.
- **Letter-spacing:** eyebrow labels 3px, nav links 0.5px, brand mark 2px. Body text uses default tracking.
- **Line height:** body 1.6, headings 1.05–1.3 (tighter for larger sizes).
- **Italics:** reserved for taglines, meta text, and the "note" paragraph at section ends.

---

## 3. Layout

- **Max content width:** 960px. Centered, 32px side padding.
- **Section vertical padding:** 64px top/bottom.
- **Section divider:** 1px top border `rgba(153,153,153,0.25)`. First section has no top border.
- **H2 underline:** 44px × 3px terracotta bar, 12px below the heading text.
- **Cards:** white surface, 4px colored top border (one of terracotta / gold / sage), 28px × 24px padding, 4px corner radius, subtle shadow `0 2px 10px rgba(51,51,51,0.05)`. On hover: lift 3px and shadow deepens.
- **Breakpoint:** single-column layout at ≤ 760px. Hero photo centers, grid collapses to one column.

---

## 4. Imagery

- **Portrait:** circular crop, transparent background PNG, white 4px ring, soft shadow `0 6px 24px rgba(51,51,51,0.12)`. Default size 220px in hero; 170px in compact contexts.
- **Source photo:** `MFC.jpg` (original). Always center-cropped to square, then circular-masked. Never stretched.
- **Icons:** none currently. If added later, use stroke-based SVG in `#666663`, 1.5px stroke.
- **No stock imagery.** No decorative photos. No emoji in prose.

---

## 5. Data visualization

When producing figures (ggplot, Datawrapper, etc.) that may appear on this site or adjacent materials:

- **Primary series:** terracotta `#BF4D43`.
- **Second series:** sage `#6B8F71`.
- **Third series:** muted gold `#C9A84C`.
- **Neutral / reference lines:** warm gray `#666663`.
- **Background:** warm white `#F0F0EB` or transparent.
- **Grid lines:** light gray `#999999` at ~20% opacity.
- **Axis text:** dark text `#333333`, sans-serif.
- **No default ggplot gray background.** No default matplotlib blue.

---

## 6. Voice in stylistic elements

(Content-level voice lives elsewhere; these are the few stylistic decisions that touch copy.)

- **Bullets:** sentence case, no trailing period on single-fragment bullets, period on full sentences.
- **Dashes:** em dash (—) for asides, no spaces; en dash (–) for ranges. Never use "--" or hyphens in place of em dashes.
- **Middle dot (·)** as separator in hero taglines, card metadata, link labels.
- **Section labels and eyebrows:** uppercase, letter-spaced, terracotta or warm gray.

---

## 7. What this guide is *not*

- It does not specify copy, research framing, skills descriptions, or publication content. For those, see `JOBS/CLAUDE.md`.
- It does not cover academic paper formatting (LaTeX). The CV has its own typographic conventions based on `mathptmx` and stock article geometry.
