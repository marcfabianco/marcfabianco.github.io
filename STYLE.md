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

- **Sans (everything):** the system UI stack — `-apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", "Lucida Grande", Arial, sans-serif`. No webfont is loaded. The site renders in the reader's native interface font.
- **Serif (optional accent):** Georgia, Times, serif. Available for pull quotes and long-form editorial pages. Not used on the main site.

Weights in use: 400 for body, 600 for headings and labels.

### Scale

| Token      | Size    | Weight | Use                                              |
|------------|---------|--------|--------------------------------------------------|
| Brand      | 18px    | 600    | Masthead name, 0.6px letter-spacing              |
| H2         | 20px    | 600    | Section headings                                 |
| Item title | 17px    | 600    | Paper and publication titles                     |
| Body       | 16px    | 400    | Paragraphs                                       |
| Meta       | 14px    | 400    | Authors, captions, secondary text                |
| Venue      | 13px    | 400    | Venue and status lines, light gray               |
| Label      | 11-12px | 600    | Uppercase section labels and nav, 2-2.5px letter-spacing |

### Rules

- **One family.** Size, weight, and letter-spacing carry the hierarchy. No display face.
- **Letter-spacing:** uppercase labels 2-2.5px, brand mark 0.6px. Body text uses default tracking.
- **Line height:** body 1.6, titles 1.35.
- **Uppercase letter-spaced labels** are the main structural signal, replacing the old serif section headings.
- **Italics:** sparing. Meta text and the occasional note.

## 3. Layout

- **Max content width:** 900px, centered in the zone left of the pink band, 40px side padding.
- **Right band:** 130px fixed soft-pink column, full height, vertical Substack link. Becomes a horizontal strip at the breakpoint.
- **Masthead:** name on the left, uppercase nav on the right, 20px vertical padding, 1px bottom border.
- **Section vertical padding:** 40px top and bottom. Keep it tight. Whitespace comes from line height, not from padding.
- **Section divider:** 1px top border `rgba(153,153,153,0.25)`. First section has no top border.
- **No decorative heading rules.** The terracotta bar under H2 is retired.
- **Lists are unnumbered.** No counters, no leading-zero indices.
- **Item metadata is a single line**, middle-dot separated. No definition lists, no bordered metadata blocks.
- **Cards:** white surface, 4px colored top border (one of terracotta / gold / sage), 28px x 24px padding, 4px corner radius, subtle shadow `0 2px 10px rgba(51,51,51,0.05)`. On hover: lift 3px and shadow deepens.
- **Breakpoint:** single column at <= 860px. Portrait centers above the text, grids collapse.

---

## 4. Imagery

- **Portrait:** circular crop, transparent background PNG, white 4px ring, soft shadow `0 6px 24px rgba(51,51,51,0.12)`. Default size 280px in the intro block; 200px at the mobile breakpoint.
- **Source photo:** `MFC2.jpg` (in use); `MFC.jpg` is the original. Always center-cropped to square, then circular-masked. Never stretched.
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
