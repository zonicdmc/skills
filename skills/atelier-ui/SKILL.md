---
name: atelier-ui
description: >
  Art direction for pages that should feel edited, not assembled. Use when
  building or restyling a landing page, marketing site, portfolio, product
  page, or a screen that should read like print. Triggers on taste, art
  direction, editorial, magazine, atelier, less generic, less AI, or make it
  look designed.
---

# Atelier

Give the page a point of view before you give it components.

Do not invent a second brand. Use the name, offer, proof, and pictures the user actually has.

## 1. Brief, four lines, before CSS

Write these in a stylesheet comment and then build only that:

1. **Who is in the room.** One reader, not "everyone".
2. **The job of the page.** One action.
3. **The material.** Pick one: paper, ink, metal, cloth, timber, glass.
4. **The voice.** Either short stamped lines, or long measured sentences. Not both.

## 2. Deal one family and commit

Pick one. Do not mix.

| Family | When | What it looks like |
| --- | --- | --- |
| **Ledger** | Tools, pricing, numbers, status | Ruled rows, small type, one ink, figures that can be checked |
| **Folio** | Story, studio, product with a photograph | Wide margins, a display serif, one full-bleed picture, long quiet sections |
| **Bench** | Craft, hardware, making | Things in a row, labels like stamps, photos of hands and materials |

Say the family name in the comment from section 1. A later section may not switch families.

## 3. Type

- Two families maximum. A display face for the promise, a text face for the argument.
- Body measure 60–75 characters. Line-height 1.45–1.6 for text, about 1.05–1.15 for display.
- A headline may be two lines only when the line break is a phrase break.
- No all-caps paragraphs. One running label (the section name) may be small and tracked out. Buttons are sentence case.

## 4. Color is a material

Three roles only:

- `--paper` ground
- `--ink` text and rules
- `--stain` the single accent

The stain appears at most three times above the fold: the action, one rule or mark, one detail. Do not paint sections with it.

Neutral paper and ink do the rest. If the brand already has a color, that color is the stain, not a fourth role.

Put the three roles in the project's token layer. Do not sprinkle raw hex through components.

## 5. Pictures and empty space

- One photograph that could only be this subject, cropped tight, or no photograph.
- No gradient blobs, no fake device frames, no gray placeholder boxes, no emoji as icons.
- If there is no photo, use type and one diagram. Do not substitute stock.
- Sections separate by space, not by cards nested in cards.

## 6. Grid

- Pick 4, 6, or 12 columns and keep them.
- One element may break the grid. It has to be the thing the page is about.
- Rhythm on an 8px baseline.
- Order of a marketing page: claim, proof, how it works, offer. Do not open on a feature grid.
- First screen is the claim plus one piece of proof. A navbar is not the hero.

## 7. Motion, one idea

The whole page gets one motion, matched to the family:

- **Ledger:** a figure counts once on enter. Rows do not bounce.
- **Folio:** the photograph drifts at most 8px while scrolling. Nothing else moves.
- **Bench:** a control lifts 2px on hover.

Animate `transform` and `opacity` only. 150–250ms, ease-out. Gate the drift and the count behind `prefers-reduced-motion: no-preference`. Hover feedback may stay.

## 8. Words

Specific nouns and a number the reader can check. Buttons name the action ("Open the ledger", "Read the folio") when a truer verb than "Get started" exists.

Do not write: elevate, seamless, unleash, next-gen, unlock, game-changer, delve.

## 9. Read it back

Before you call the page done, answer:

- Can you name the material in one word?
- Is there exactly one stain?
- Is the first screen a claim plus proof?
- Would it still make sense printed in one ink?

Any "no" means change the design. Do not add another section to hide it.
