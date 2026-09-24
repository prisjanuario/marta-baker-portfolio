# Marta Baker — Portfolio concepts (3 directions)

Typeface: **Syne** (variable, 400–800) — bundled in each concept's `fonts/` folder and
loaded via `@font-face`. Each concept is one self-contained, responsive HTML file.
Open `index.html` in any browser (no build step, no dependencies).

---

## concept_01_bauhaus/
Flat, minimal, Bauhaus. Strictly three colours: **#000000** text, **#ffffff** background,
**#868686** for every geometric form, rule and secondary label.
- Hero: oversized Syne 800 wordmark "Marta Baker", offset second line, outlined circle,
  half-circle and tick-rhythm lines; column guides behind the content.
- A grey hairline divider separates the hero from section 02 — **About** — with the
  statement "I design human-centered interfaces…" and a 4-cell form catalogue
  (circle / axes / half-circle / line field).
- Motion: clip-reveal of the name, divider draw, scroll reveals (disabled under
  `prefers-reduced-motion`).

## concept_02_darkmode/
Same copy as concept 01, extended with **Tools and Skills**, **Where I've been** and
**Where to find me**. Deep grey (#1a1a1a) ground, white type.
Accessibility was the design constraint:
- Contrast: white on #1a1a1a = **17.4:1**, secondary #b4b4b4 = **8.4:1**, cards 15.7:1 (all AAA).
- Skip link, visible 3px focus rings, semantic landmarks/headings, `aria-label`s,
  44–56px touch targets, accessible disclosure menu (aria-expanded + Esc) on small screens,
  marquee duplicated for screen readers as plain text, full `prefers-reduced-motion` support.

## concept_03_playful/
Cartoonish kids-app direction: cream paper, dotted texture, drifting blobs, sticker UI with
hard ink outlines and 3D offset shadows, hand-drawn SVG characters (robot mascot + crayon buddy).
Nothing static or generic:
- Headline splits into per-letter bobbing glyphs that wiggle on hover.
- Mascot's pupils track the cursor; "Tickle me" (or tapping the mascot) makes it giggle, tilt
  and shoot confetti.
- "Pop!" button fires a canvas confetti burst and counts pops.
- Springy hover/press states on every button, tilting sticker cards, rotated ticker,
  floating footer doodles — all silenced under `prefers-reduced-motion`.

---

`source/` — screenshot/QA script used during the build + the original Syne variable font file.
