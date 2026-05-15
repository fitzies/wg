# Wishing Garden — Concept Log

Living record of design exploration. Append-only — each round captures the brief, what we tried, and Jamie's response, so future sessions can read why we landed where we did. Pair with `IDENTITY.md` (stable brand truths).

---

## Round 1 — Initial five (A–E)

Five homepage concepts shared with Jamie via `brand/index.html`:

- **A — Editorial Soft** — `concepts/a-editorial-soft.html`
- **B — Garden Romantic** — `concepts/b-garden-romantic.html`
- **C — Modern Apothecary** — `concepts/c-apothecary-modern.html`
- **D — Talisman** — `concepts/d-talisman.html`
- **E — Heritage** — `concepts/e-heritage.html`

### Jamie's feedback
Full notes in `brand/initial-feedback.md` and `brand/feedback-attached.docx`. Headlines:

- Cherry-picked across **A, B, C** — copy style from A, taglines from B, nav layout from C.
- **D and E got no comments** → treated as silently rejected. Kept in repo, not iterated on.
- **Scope cut:** only the *wishingarden dome workshop* section needs to be fully functional. Everything else is a placeholder card ("Awakening. Soon." / "A space unfolds. Stay curious.").
- **Experimental palette** proposed — framed as experiment, not lock-in:
  - Beige `#F7F4D5` (main bg)
  - Dark Green `#0A3323` (contrasting body type)
  - Moss `#839958`
  - Rosy Brown `#D3968C`
  - Midnight Green `#105666` (top scroll banner, with beige type)
- **Wordmark:** `wishingarden` — single g, stylized "all small caps". Small logo sits **above** the wordmark in the nav.
- **Section order:** scroll banner → nav → workshop hero → new arrivals (Lily of The Valley) → secondary collection (silver / bookmarks / keychains, 3 horizontal images, more whitespace) → pop-ups → bench / philosophy → footer. Contact moves to top-right of header.
- **Workshop flow:** Core Garden / Statement Garden → form (name, notify via WhatsApp or email, which garden, date picker, time slot) → `$20 deposit` notice. Pricing: Core `$75 / $97`, Statement `$127 / $158`.

### Pending from Jamie
- Lily of The Valley product photos.
- Pop-ups section reference screenshots & notes.
- Copy suggestions she invited: workshop SEO, 2nd-section tagline, bench-section tagline.

---

## Round 2 — Three drastic directions *(abandoned)*

**Original brief:** Three philosophically distinct concepts (F — Editorial Periodical, G — Botanical Apothecary, H — Modern Handcraft) exploring different layout systems, palette philosophies, and type pairings. Files were built (`f-editorial-periodical.html`, `g-botanical-apothecary.html`, `h-modern-handcraft.html` + matching workshop pages).

**Why abandoned:** Three concepts diluted the feedback signal — they didn't follow Jamie's notes literally enough, and the workshop detail pages were over-designed. Decision (with Oli): consolidate to a **single combined concept** that follows the docx point-by-point, with workshop as a clean on-page section rather than a separate page.

**Files removed:** `concepts/f-*.html`, `concepts/g-*.html`, `concepts/h-*.html`. Not preserved — the notes here capture the attempt.

---

## Round 2 (revised) — One combined concept

File: `concepts/i-merged.html` — single page, all sections, workshop functional.

**Palette (strict, per docx):**
- Body bg: Beige `#F7F4D5`
- Type: Dark Green `#0A3323`
- Top scrolling banner: Midnight `#105666` bg + beige text
- Moss `#839958` / Rosy Brown `#D3968C` used only as subtle plate accents

**Typography:** Cormorant Garamond (display, with italics + small caps) + Inter (body / UI). Single serif, single sans — per IDENTITY's "hold the line" principle.

**Wordmark:** `wishingarden` — single g, small caps. Small sigil sits **above** the wordmark in the nav (per Jamie's preference for concept 03's nav layout).

**Section order, copy per docx:**
1. Scrolling banner — "complimentary post over $80", "letters from the garden, every new moon", "workshops opening · june 2026".
2. Utility row — "whatsapp · soon", "contact us" pinned to top-right corner.
3. Nav — `new arrivals · workshops · trinkets · gemstones · [sigil + wishingarden] · bookmarks · suncatchers · gifting · our philosophy`. Dropdown carets on trinkets / gemstones / gifting (WIP indicators).
4. **Section 01 — workshop hero** — "wishingarden dome workshop" + "A hands-on workshop to craft your own wishingarden. Therapeutic, gentle, and yours to shape." + "wander in →". Includes small sigil ornament above the headline and an ssfw-style scroll cue below.
5. **Workshop detail** (anchored from "wander in") — Core Garden ($75 / $97) + Statement Garden ($127 / $158). Minimal booking form: name, notify-by (whatsapp / email), garden, date, time slot. $20 deposit notice. Reserve a seat CTA.
6. **Section 02 — Lily of The Valley** — "Wearable blooms from our garden." + placeholder plate + "awakening · soon" pill.
7. **Section 03 — the collection** — 3 horizontal items (925 silver jewellery, metal bookmarks, keychains) with placeholder pricing + generous whitespace.
8. **Section 04 — pop-ups** — placeholder, awaiting Jamie's reference screenshots and notes.
9. **A letter from the garden** — quiet philosophy block. "Some things, we believe, are best made slowly & intentionally." + handcrafted gemstone charm description (on brass, deckle-edge cards, flower-and-star mark).
10. **Our small practice / bench** — "Made by hand, in small batches, with chosen stones." + "Each trinket handcrafted at our bench in Singapore. (wishingarden domes, too.)"
11. **Footer** — four columns (brand block / visit / the garden / more) + colophon strip.

**Placeholders:** image plates use CSS gradient placeholders with subtle "image · placeholder" labels — ready to swap in real product photography once Jamie sends Lily of The Valley shots.

### Open items for next round
- Lily of The Valley photos (pending from Jamie).
- Pop-ups section screenshots & notes (pending).
- Copy suggestions Jamie invited (workshop SEO, alternate taglines).
- Decide whether to wire up the form (Calendly / custom backend / Typeform) once direction is approved.
