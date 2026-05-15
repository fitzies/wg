# Wishing Garden — Handoff

Snapshot for the next chat session. Read this first, then `IDENTITY.md` (brand truths) and `CONCEPTS.md` (decision log). The active concept lives at `brand/concepts/i-merged.html` + `brand/concepts/i-workshop.html`.

---

## Client & project

- **Client:** Jamie. IG `@wishingarden`. Singapore. Handcrafted gemstone trinkets — crystal charms on brass, deckle-edge paper cards, jute, sun/star sigil.
- **Phase:** Concept exploration. No backend, no build step, no framework. Static HTML with embedded CSS, served as files.
- **Stakeholder loop:** Oli (dev) builds → shares `brand/index.html` with Jamie → Jamie sends feedback → Oli iterates.

---

## Current state — round 2 (revised)

**One merged concept**, two pages:

1. `brand/concepts/i-merged.html` — homepage. Sections: hero/workshop teaser → Lily of The Valley new arrivals → secondary collection (silver / bookmarks / keychains) → pop-ups → "a letter from the garden" philosophy block → bench (our small practice) → footer.
2. `brand/concepts/i-workshop.html` — workshop detail page. Reached via "wander in" CTA on the homepage hero. Sections: page title → hero image → two gardens (Core / Statement) → booking form → what to expect → footer.

The `brand/index.html` gallery points to `i-merged.html` as the only round-two entry. Round-one concepts A–E still on disk but de-emphasized in the index. Round-two earlier attempts (F/G/H) were deleted — they didn't follow feedback strictly enough.

---

## Hard-won rules (do not violate)

### Typography — 5 styles only, applied via classes

```css
.display   — Cormorant Garamond regular, clamp(40px, 5.4vw, 76px). Hero h1, section displays. Italics ONLY via .display em — used sparingly.
.display.small-display — same family, 28-42px. For sub-displays.
.kicker    — Cormorant 11px, letter-spacing 0.36em, uppercase. EVERY label, nav item, button, section title.
.body      — Cormorant 17px regular, line-height 1.7. Every paragraph.
.small     — Cormorant 13px. Footer links + fine print.
.wordmark  — Cormorant small-caps 17px, letter-spacing 0.28em.
```

No other sizes. No mixed letter-spacings. No italic body copy. Body font is Cormorant throughout — Inter was dropped because mixing two families produced visual chaos. The whole page reads as one type system.

### Palette — strict, from Jamie's docx

| Role | Hex |
|------|-----|
| Body background | `#F7F4D5` (beige) |
| Section variation | `#F1ECC6` (beige-soft), `#E8E2B0` (beige-deep) |
| Body text | `#0A3323` (dark green) |
| Scrolling banner background | `#105666` (midnight — reads as deep teal/blue) |
| Scrolling banner text | `#F7F4D5` (beige) |
| Moss / rosy brown | `#839958` / `#D3968C` — use only as faint photographic accents. Not as type colors. |

No inverted dark sections in the body. Stay in the cream family. SSFW does this and Jamie's palette reads best this way.

### Wordmark — single g, "all small caps"

- The brand is written `wishingarden` (one word, single g, lowercase) and styled with `font-variant: small-caps`.
- The wordmark sits BELOW a small flower-and-star sigil in the nav. Centered.
- Per docx feedback referencing concept 03 — Jamie explicitly preferred this layout.

### Header / nav structure

```
[ banner — scrolling midnight ]
[ utility row — right-aligned: whatsapp · contact · search · account · basket ]
[ main nav — 4 items LEFT · sigil+wordmark CENTER · 4 items RIGHT ]
```

Nav sequence (locked by Jamie): `new arrivals · workshops · trinkets ▾ · gemstones ▾ ⟪logo⟫ bookmarks · suncatchers · gifting ▾ · our philosophy`. Carets indicate dropdowns (WIP).

### Workshop page — SEPARATE page, not inline

- "Wander in" CTA goes to `i-workshop.html`, never inlines workshop detail on the homepage.
- Form lives on the workshop page only.
- Lesson: when client says "everything on one page, sectioned" about the workshop page, they mean *the workshop page itself is one cohesive sectioned page* — they do NOT mean merge homepage + workshop.

### Hero CTAs — OFF the image

- Hero image is just photography. Tiny corner caption only.
- Title + CTA live on a solid beige strip BELOW the image.
- The "wander in" CTA is a proper dark green button — visible at a glance.
- Lesson: text overlaid on photography is hard to read and looks cheap. SSFW does the same — image is the image, CTAs sit on solid backgrounds.

### Booking form — editorial inline rows

- Each field is one row with a hairline border bottom. Label left (`.kicker`), input/choices right.
- Choice fields are inline TEXT options separated by `·`. Active option is italicized + underlined; inactive is dimmed text. Click to switch (JS).
- No pill buttons. No deposit box. No slab submit button.
- Deposit notice is one italic body line above the submit.
- Submit is a tracked-caps text link with arrow `reserve a seat →`.

### Section-head pattern (SSFW-derived)

```
— [crumb kicker] —
[title kicker]
[ thin 56px horizontal rule ]
[ optional arrow link →]
```

Every section head uses this. Centered for full-width sections, left-aligned in editorial split layouts.

---

## File map

```
brand/
├── IDENTITY.md           — brand truths (palette, voice, references) — STABLE
├── CONCEPTS.md           — round-based decision log — append-only
├── HANDOFF.md            — THIS FILE — snapshot for next session
├── initial-feedback.md   — Jamie's first feedback (chat messages)
├── feedback-attached.docx — Jamie's per-section feedback document
├── index.html            — concept gallery, shared with Jamie
├── refs/
│   ├── ssfw/             — 6 SSFW screenshots, the visual reference
│   ├── jilsander/        — restraint reference (not the palette)
│   └── instagram/        — Jamie's IG product shots
└── concepts/
    ├── a-editorial-soft.html       — round 1
    ├── b-garden-romantic.html      — round 1
    ├── c-apothecary-modern.html    — round 1 (the nav layout Jamie liked)
    ├── d-talisman.html             — round 1 (rejected, kept as archive)
    ├── e-heritage.html             — round 1 (rejected, kept as archive)
    ├── i-merged.html               — round 2 (revised) — CURRENT HOMEPAGE
    └── i-workshop.html             — round 2 (revised) — CURRENT WORKSHOP PAGE
```

Plus the root `CLAUDE.md` — minimal pointer file. Doesn't need to grow much; deeper context lives in the brand/ docs.

---

## Pending from Jamie

These are still owed by Jamie before round 3:

- **Lily of The Valley product photos** — for the section-02 hero plate. She said "will send photo tmr or thurs" (around 2026-05-09).
- **Pop-ups section reference & notes** — she said she liked content from a link she'd send screenshots of.
- **Copy suggestions she invited:**
  - Workshop SEO copy (1st section)
  - 2nd section tagline alternative ("Wearable blooms from our garden" is current)
  - Bench section tagline (open to alts on "Made by hand, in small batches…")
- **Form action target** — once Jamie approves the design, decide where the booking form posts (Calendly? Typeform? a simple email-to-Jamie webhook? WhatsApp pre-filled message?).

---

## Reference sites (research subagent, vetted URLs)

Use these for the next visual direction round if needed. Tightest matches to palette + vibe:

| Site | Why |
|------|-----|
| [cultivateapothecary.com](https://cultivateapothecary.com/) | Hudson Valley botanical skincare. Cream + forest green + warm beige — closest to Jamie's palette in the wild. |
| [yamaceramicsstudio.com](https://yamaceramicsstudio.com/) | California pottery. Nearly all five Wishing Garden hues appear. |
| [mimosahandcrafted.com](https://mimosahandcrafted.com/) | Louisiana handcraft jewelry. Direct analog as a *handcraft jewelry* site with green/beige/bronze. |
| [maisonbalzac.com](https://www.maisonbalzac.com/) | Sydney candles. Moss + dusty rose accents on cream. |
| [saipua.com](https://www.saipua.com/) | Brooklyn soap + flower farm. Slowest editorial commerce on the list — vibe twin. |
| [buly1803.com](https://buly1803.com/en-us) | Officine Buly — the apothecary editorial reference, restrained typography. |
| [notaryceramics.com](https://www.notaryceramics.com/) | Portland ceramics. Closest structural cousin to SSFW. |

Plus the original reference: **`ssfw.com.sg`** (screenshots in `brand/refs/ssfw/`) — Jamie's anchor for the visual restraint, even though SSFW uses cream/grey not green.

---

## What NOT to do (lessons from prior rounds)

1. **Don't merge homepage + workshop into one page.** I did this in an early round 2 attempt and the client was furious. Workshop is its own page.
2. **Don't propose 3 "drastic directions" when the client already picked elements from existing concepts.** Round 2's first attempt built F/G/H as separate philosophies — they got deleted. Client wanted ONE concrete merged direction.
3. **Don't overlay big display headlines on hero photography.** They become unreadable. CTAs go on solid backgrounds.
4. **Don't build a heavy form with pill buttons and a boxed deposit notice.** Three iterations failed before the editorial inline-row pattern landed. If a future round of feedback says "the form looks bad," try removing visible structure entirely — make it look like a sentence, not a form.
5. **Don't introduce a third typeface.** Body in Cormorant. Inter was tried and removed — it created visual noise alongside the display serif.
6. **Don't use moss/rosy brown as text colors.** They're for photographic accents only. Type is always `#0A3323` on `#F7F4D5`.
7. **Don't write project / activity recap docs unless asked.** This HANDOFF.md exists because Oli asked — otherwise concept work doesn't need a parallel paper trail beyond CONCEPTS.md.

---

## Open design questions for next round

- Does Jamie respond to the new SSFW-restrained direction, or does she want the brand to feel warmer / more botanical (closer to Cultivate Apothecary)?
- Should the hero on the homepage be the workshop, or pivot to the new Lily of The Valley collection once photos arrive? Hero placement is currently workshop-led; arguably new arrivals should lead.
- Wordmark — is the current sigil (sun + circle of dashes) the final mark, or does Jamie have one she'd like used? The kraft card in her IG flat-lays has a flower-and-star embossed mark — that might be the brand mark, but we don't have a clean vector of it yet.
- The "letter from the garden" newsletter — should the subscribe form do anything (Mailchimp / Buttondown / ConvertKit) or stay a placeholder?

---

## How to pick this up

1. Read this file.
2. Read `IDENTITY.md`.
3. Read `CONCEPTS.md` for the decision log.
4. Open `brand/concepts/i-merged.html` and `brand/concepts/i-workshop.html` in a browser to see the current state.
5. Ask the user what they want to change. Don't refactor proactively.
