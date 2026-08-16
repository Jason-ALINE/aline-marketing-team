# `/introduction`

**Title tag:** Shaft Alignment Instructions — Reverse-Indicator Method | ALINE Manufacturing
**H1:** How to Perform Reverse-Indicator Shaft Alignment
**Status:** RESTORED — core content matched consistently across multiple independent Google-cache hits of this exact URL and the retired `introduction.htm`/`procedure.htm` pages. Reworded lightly for current voice; structure matches the four live `/instructions` pages. See Restoration & Assumption Notes at the bottom before this goes to Wix.

[SITEWIDE NAV STRIP — existing template element shared by all 7 `/instructions` pages. Not drafted here; this page just needs to sit inside it.]

---

Reverse alignment is the measurement of the centerline of one shaft relative to the centerline of an opposing shaft. Taken correctly, that measurement can be projected the full length of both shafts — which is what lets you account for thermal growth later — and it shows you the position of both centerlines at the coupling flex planes, which is what you need to pick an allowable tolerance.

This page covers the first thing you do on every job: mount the brackets and measure your three reference distances — **A**, **B**, and **C**. Every other page in this sequence assumes you've already got these three numbers written down.

## BEFORE YOU START

- Bracket set and dial indicators (each ALINE set ships with a Starrett 196B1 — .001" resolution)
- Tape measure or calipers, for A/B/C
- Adjustable wrench, for the bracket clamps
- Flat file and a rag — clean mounting surface, no nicks or burrs

## Mount the brackets

Clamp one precision bracket to each shaft (or hub), bridging the coupling without disconnecting it. Before you clamp down:

1. Clean the mounting surface on both shafts/hubs. File off any nicks or burrs — a bracket that isn't seated flat will give you bad readings no matter how careful the rest of the job is.
2. Aim each indicator stem directly at the centerline of the shaft it's reading.
3. Snug the clamps enough that the bracket can't shift, but don't overtighten to the point you're deforming anything.

## Measure A, B, and C

**[EXISTING ASSET — place on page, route to design-visual-specialist only if cleanup/relabeling is needed]** Use the original diagram: `introd2.jpeg` / `introd3.jpeg` / `introd4.jpeg` (Site Files > Introduction folder). These show two machines labeled "Fixed" (blue, left — the stationary pump) and "Moveable" (red, right — the motor being aligned), joined by a coupling, with brackets A, B, C labeled left to right beneath them: A nearest the coupling, B in the middle, C furthest right at the Moveable machine's feet. Pick whichever of the three variants best matches current site image sizing/style; all three appear to show the same diagram.

| Measurement | What it is |
|---|---|
| **A** | Distance between the two indicators |
| **B** | Distance from the indicator to the near ("front") foot of the machine being moved |
| **C** | Distance between that machine's front and back feet |

Write these down before you touch anything else. B and C are what let you convert the indicator readings you take on the Horizontal Move and Vertical Move pages into actual shim and move amounts at each foot — get them wrong and every downstream calculation is wrong with them.

## Take your readings

With both brackets mounted and A/B/C recorded, rotate the shafts together and take indicator readings at four positions — top, bottom, left, and right — at each indicator.

## What's next

- Check [Alignment Tolerances](/alignment-tolerances) to know what target you're working toward before you start moving anything.
- Run a [Sag Check](/sag-check) using this same bracket span before you trust any vertical readings.
- Run a [Soft Foot Check](/soft-foot-check) on the machine before final bolt-up.
- Then move to [Horizontal Move](/horizontal-move) and [Vertical Move](/vertical-move) with A, B, and C in hand.

---

## Restoration & assumption notes (internal — strip before publishing)

**Directly sourced (high confidence, matched across 2+ independent cache queries of this exact URL):**
- The opening definition paragraph ("Reverse alignment is the measurement of the axis or centerline of one shaft to the relative position of the axis of an opposing shaft centerline... projected the full length of both shafts... allow for thermal movement... position of the shaft centerlines at the coupling flex planes, for the purpose of selecting an allowable tolerance") — this is close to verbatim from Google's index of this specific URL.
- The A/B/C definitions ("distance between indicators" / "distance between the indicator and the front foot" / "distance between feet") — returned identically across separate search queries, strong signal this is real restored text, not an AI paraphrase drifting.
- The bracket-mounting detail ("clean the mounting surface... file off nicks and burrs... indicator stem aimed directly toward the center line of the shaft") — sourced from cached `procedure.htm` content.
- "Bridging the coupling," "four readings recorded — top, bottom, left, right, at each indicator" — sourced from cached site copy describing the method; can't confirm with certainty this exact phrasing lived on `introduction.htm` specifically vs. a general site description, but it's consistent with ALINE's own stated method elsewhere, so I've kept it.

**Confirmed (no longer a flag):**
- **Which machine's feet B and C refer to.** Confirmed from the original diagram, sourced from Site Files > Introduction (`introd2.jpeg`/`introd3.jpeg`/`introd4.jpeg`, plus a 2022-10-06 screenshot). The diagram labels the two machines "Fixed" (stationary pump) and "Moveable" (motor), with A, B, and C all measured on the Moveable side, from the coupling face out to its feet. My original inference from the Vertical Move worked example was correct — the table above is accurate as written and does not need to change.

**Inferred — flag before publishing, don't treat as confirmed:**
- **The BEFORE YOU START tool list.** The cleaning/filing detail is sourced; the full tool list (tape measure, wrench, file, rag) is a reasonable reconstruction matching what the procedure implies you'd need, not a verbatim restored checklist. Format matches the live pages' BEFORE YOU START box convention.
- **The exact reading sequence** ("four readings... top, bottom, left, right") — I could not confirm whether readings are taken in a fixed 90° rotation starting at 12 o'clock, or whether both shafts must be rotated together vs. independently. Someone who's actually run the ALINE bracket hardware should confirm this line before it ships.
- **Diagram** — resolved. The original legacy diagram was located in Wix Media Manager (Site Files > Introduction: `introd2.jpeg`, `introd3.jpeg`, `introd4.jpeg`, and a 2022-10-06 screenshot). No new diagram needs to be commissioned.

**Next specialist:** No design-visual-specialist work needed to create this diagram — the real asset already exists and just needs to be placed on the page in Wix. If, on closer look, the existing JPEGs need relabeling or cleanup (e.g. resolution too low for the new page layout, or labels that don't match this page's exact A/B/C table wording), route that specific fix to design-visual-specialist rather than a from-scratch build. Otherwise this page is ready for Wix implementation — no live-publishing agent exists yet, so this stays a draft until someone enters it manually.
