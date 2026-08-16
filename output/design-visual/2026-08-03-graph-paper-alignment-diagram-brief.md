# Design Brief: Graph-Paper Alignment Plotting Diagram (Dark/Grid Style)

**For:** Claude Design (`/design`)
**Prepared by:** design-visual-specialist
**Date:** 2026-08-03
**Route:** Marketing layout / visual asset — hand to `/design` with this brief as-is.
**Design-sync status:** DONE (2026-08-03) — Claude Design project "ALINE
Manufacturing" created and the brand color palette synced
(`colors/palette.html`). Safe to run `/design` referencing this brief now.

---

## FLAGS — read before building (not resolved by this brief, don't guess)

1. **Address — RESOLVED 2026-08-03.** Jason confirmed directly: Liberty
   Hill, TX (270 Cole Drive) is the old, pre-move address — ALINE relocated
   to Johnson City, TX approximately 4 years ago. Johnson City is current
   (matches company-brief.md). The PDF's phone number (512-778-5454) is
   unconfirmed as still current — still don't carry it forward without
   asking. Per the original design intent below, **no address is planned
   for this diagram anyway** (it's a technical plotting reference, not a
   branded contact asset), so this is now a non-issue either way.

2. **Distance A/B/C — RESOLVED 2026-08-03.** Jason confirmed: the page 2
   worked examples use the **same distances as page 1: A=10", B=5", C=11"**.
   They aren't printed as numbers on the original page 2 plots because
   they're shown graphically — small black dots on the original plot mark
   these distances, meant to be read by counting grid squares between plot
   markers rather than by a printed label. **The new diagram should label
   A/B/C = 10"/5"/11" explicitly** (this is a place the new diagram can
   improve on the original by printing the values instead of requiring the
   viewer to count squares) — this is confirmed content, not a guess.

3. **Non-uniform grid axes — this is the single most important technical
   detail to get right.** The plotting grid is *not* a uniform square
   grid in real-world terms even though it's drawn as square boxes:
   - Vertical axis (indicator/shim amount): **each square = .001"**
   - Horizontal axis (indicator/feet spacing): **each square = 1.0"**
   If Design (or any automated grid-generation step) treats this as a
   uniformly-scaled grid, or auto-labels both axes the same way, the
   diagram becomes technically wrong. This must be preserved exactly as
   two different scales sharing one visual grid.

4. **Tolerance band — do not invent a number.** The website's existing
   "Tolerance Window" diagram shows a ±.004" dashed tolerance band as an
   example for a *different* topic (reading tolerances generally, with an
   8.0" coupling span). The Vertical/Horizontal Move worked examples in
   this brief have no stated tolerance value. Do not add a ±.004" band or
   any other tolerance figure to the new diagrams — only plot what's
   sourced below. If Jason wants a tolerance band added, that's a
   separate decision he needs to make explicitly.

5. If any technical detail below still looks ambiguous once you're
   actually laying this out, stop and flag it back to the Manager rather
   than approximating it — precision is the entire point of this asset.

---

## 1. Goal

Produce a diagram (or small set of 2-3 companion diagrams) that teaches
ALINE's graphical reverse-indicator alignment plotting method end-to-end,
using the **real worked-example numbers** from ALINE's original "Back to
Basics" instructional graph-plotting handout — but rendered in the site's
**current dark/grid visual language** (as seen live on
`alinemfg.com/horizontal-move` and `alinemfg.com/vertical-move`), not the
old cyan-grid-on-white-paper scanned-worksheet look.

This is meant to function as a real, citable reference diagram — usable on
the website (most likely replacing or supplementing the existing
Horizontal Move / Vertical Move page diagrams) and/or in future sales
material. It needs to be precise enough that a millwright could actually
plot points and reproduce the recommended shim/shift corrections from it —
not just an illustrative mockup.

Two worked examples must both be represented (Vertical Move and Horizontal
Move) since Jason wants the full worked-example content that exists in the
PDF but is not currently on the website, presented in the site's current
visual system.

## 2. Layout

Follow the existing site pattern exactly — this is not a new layout
system, it's an extension of one already live:

- **Label → Heading → Diagram** stacking pattern used throughout the site:
  a small-caps, letter-spaced, muted-gray label line above a plain-language
  heading (e.g. label "PLOTTING EXAMPLE" above heading "VERTICAL MOVE,
  WORKED EXAMPLE" — exact wording is Design's to set within this pattern,
  not invented technical content).
- Two panels, one per worked example (Vertical Move, Horizontal Move),
  either stacked or side-by-side depending on what reads best at the
  target placement (website page vs. sales sheet) — Design's call, but
  each example needs to remain a self-contained, fully-readable unit; don't
  compress them into a single combined plot.
- Each panel reuses the **existing diagram anatomy** already established on
  the live Horizontal/Vertical Move pages as the visual template to extend:
  - Dark navy/near-black background with a subtle, fine grid-paper texture
    (understated, not bright white — this is the core style deviation from
    the old PDF).
  - Blue circular marker with a "+" symbol and red circular marker with a
    "−" symbol, each connected to thin vertical guide lines in matching
    blue/red.
  - Small cross-tick marks along the guide lines marking measurement
    points.
  - Labeled centerlines using the same "FIXED C/L" (solid blue) / "MOVEABLE
    C/L" (solid red) labeling convention seen on the Tolerance Window
    diagram.
  - Measurement callouts (arrows + values) pointing to the plotted result
    points, matching the site's existing callout style.
- A "BEFORE YOU START" style checklist box may be included above or beside
  the diagrams, reusing the site's two-column checklist box pattern — see
  Content section below for the real checklist copy to use if included.
- Do not introduce a new visual motif (new marker shapes, new color for
  centerlines, a different grid treatment, etc.) — the goal is consistency
  with what's already live, not a redesign.

## 3. Content

**Do not paraphrase or round these numbers — plot and label exactly as
given.**

### Vertical Move — worked example
- Indicators are zeroed at the top of shaft rotation and read at the
  bottom.
- To compensate for sag, always start the reading with a plus (+) value.
- Pump indicator reads **-12**
- Motor indicator reads **+8**
- These are Total Indicator Readings (T.I.R.). The shaft positions at the
  point of measurement are **one-half the T.I.R.**: half of -12 = -6, half
  of +8 = +4. Mark these two half-value points on the plot to represent
  the distance/position at the feet of the motor.
- Using square grid paper, when these two points are marked and the line
  is extended to be collinear with the pump shaft centerline, the result
  is: **add 0.003" shim to the front foot** and **add 0.001" shim to the
  back foot** of the motor.
- On the original plot, the resulting line is annotated directly at each
  foot position: **".003 up"** at the front foot, **".001 up"** at the back
  foot.

### Horizontal Move — worked example
- Machine is viewed from the pump end. Indicator on the left is zeroed;
  rotate and read on the right.
- Pump indicator reads **-8**
- Motor indicator reads **+10**
- Half T.I.R. values: half of -8 = **.004"** out at the point on the pump
  shaft where the indicator is mounted; half of +10 = **.005"** out at the
  point on the motor shaft where the indicator is mounted.
- When this line is projected back (extended past the foot locations), the
  result is: **front feet of the motor shift .006" to the left**, and
  **back feet shift .007" to the left**.
- On the original plot, the resulting line is annotated: **".006 left"**
  at the front foot, **".007 left"** at the back foot.

### Supporting reference content (include if space allows / if useful as a
checklist box per the site's existing "BEFORE YOU START" pattern)

**Preliminary checklist** (verbatim from source):
1. Visual check of coupling, pipehangers, base bolts, coupling spacing,
   etc.
2. Check for coupling & shaft run out.
3. Clean under feet, remove all rust, nicks, burrs and paint.
4. Reduce to a minimum the number of shims.
5. Check for soft foot.
6. Check for sag.

**Bracket installation steps** (verbatim from source):
1. Clean mounting surface, file off all nicks and burrs.
2. Check indicators for sticking or loose needle.
3. Aim indicator stem directly toward center line of shaft.

**Sag check example** (verbatim from source): When allowing for sag on a
vertical move, always start the indicator with a plus (+) reading. Example:
.002" sag → position the indicator to read +2.

**Grid legend note** (verbatim intent from source, reword for
small-caps/letter-spaced site convention if needed, but preserve the
instruction): to eliminate confusion, plus and minus signs should be
marked directly on the graph next to each reading.

**Axis scale, must appear on every diagram** (see Flag #3 above — do not
omit or simplify):
- Vertical axis: each grid square = .001"
- Horizontal axis: each grid square = 1.0"

### Do not include
- The blank "Alignment Report" fillable template from PDF page 3 (Company /
  Date / Equipment / Mechanic / Distance A/B/C fields, 4-step instructions
  to extend the moveable centerline). This is a distinct, separate asset
  from the two worked-example diagrams and is out of scope for this brief.
  If Jason wants it built as a matching dark/grid fillable template later,
  that should be a separate brief so it's not silently bundled in here.
- Any address, phone number, or letterhead branding from the source PDF
  (see Flag #1 — resolved, but still don't add one; this diagram isn't a
  branded contact asset).
- Any tolerance band or tolerance figure (see Flag #4).

### Confirmed addition (see Flag #2)
- **Label A/B/C = 10" / 5" / 11" explicitly on both worked-example
  diagrams** — printed as text/callouts rather than requiring the viewer to
  count grid squares, which is an improvement on the original PDF layout.

## 4. Audience

Millwrights, maintenance supervisors, and contract-firm project managers —
**not** reliability engineers (per `company-brief.md`, this persona has
drifted incorrectly in past work; don't repeat that here).

This audience needs:
- A diagram they could actually use in the field to cross-check a plot —
  clarity and correctness of the plotted lines, tick marks, and numeric
  callouts matters more than illustrative polish.
- No decorative flourishes that obscure the measurement points or make the
  grid harder to read at a glance.
- Confidence that the numbers shown are exact, reproducible values (not
  rounded or approximated) — this audience will notice and distrust a
  diagram that looks "close enough."

---

## Brand palette reference (from `output/design-visual/aline-color-palette.md`)

| Name | Hex | Use |
|---|---|---|
| `--navy-deep` | `#0a1a29` | Page background |
| `--navy` | `#10243a` | Secondary background |
| `--navy-card` | `#152b44` | Card/box backgrounds |
| `--steel` | `#7e8da0` | Muted/secondary text, section labels |
| `--steel-light` | `#c2cdd8` | Body copy on dark background |
| `--paper` | `#edf0f2` | Base text color (general use) |
| `--red` | `#bd322c` | Border/darker red accent |
| `--red-bright` | `#dd4b41` | Bright red accent (badges, bullets, highlights) |
| `#4f8fdb` | — | Blue accent, used sparingly (links/diagram highlights) |
| `#fff` | — | Pure white (headings) |

Headings: pure white. Body copy on dark backgrounds: `--steel-light`.
Section labels: `--steel`, small-caps, letter-spaced, per existing site
convention.
