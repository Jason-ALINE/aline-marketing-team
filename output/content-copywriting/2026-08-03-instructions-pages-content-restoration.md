# /instructions Pages — Content Restoration
**Date:** 2026-08-03
**For:** Whoever rebuilds these 7 pages on Wix (not implemented here — this is copy only)
**Source task:** SEO audit finding that all 7 `/instructions` sub-pages are indexed but text-empty; legacy pre-Wix `.htm` pages had real procedural content that didn't carry over.

## How I recovered this

I don't have live browser or Wayback Machine fetch access in this environment — I could only search. Google's search index still has the legacy `.htm` pages (`tolerances.htm`, `procedure.htm`, `sagcheck.htm`, `softfoot.htm`, `horizontal.htm`, `vertical.htm`) and current Wix pages both indexed, and repeated, differently-phrased searches against each surfaced **specific, consistent technical detail** — not generic industry boilerplate — for 6 of the 7 topics. Where the same fact/figure/procedure step came back **verbatim or near-verbatim across multiple independent queries**, I've treated that as recovered original content. Where a search only ever returned generic industry knowledge (found on Fluke, Acoem, and similar third-party sites, not tied specifically to ALINE's page), I did not treat it as recovered — I flagged it and wrote fresh instead.

**I could not confirm true page order, exact original phrasing, or original page length** — what follows is reconstructed procedural content, in ALINE's voice, built on the confirmed facts. Treat this as "restored," not "verified word-for-word archive pull." **A direct Wayback Machine check (web.archive.org/web/*/alinemfg.com) is worth doing before this goes live**, if someone has interactive browser access — it may turn up the exact original page text I couldn't reach through search alone.

**Recovery status, 7 pages:**
- **Recovered (high confidence):** Introduction, Sag Check, Soft Foot Check, Horizontal Movement
- **Recovered (high confidence, but contains a specific worked numeric example — flag for sign-off):** Vertical Movement
- **Partially recovered:** Alignment Tolerances (the one rule-of-thumb figure is solid; a fuller tolerance table, if one ever existed, did not surface)
- **Newly written, NOT a verified restoration — needs technical sign-off before publishing:** Thermal Movement

---

## 1. Introduction
**Status: Recovered**

### H1: Introduction to Reverse Indicator Alignment

Reverse indicator alignment measures the centerline of one shaft relative to the centerline of the opposing shaft — not the coupling faces, the shaft centerlines themselves. Indicators mounted on brackets read the position of each shaft in both the horizontal and vertical planes, and that measurement can be projected out along the full length of both shafts to get a true picture of how they're actually sitting relative to each other.

It's the most widely used shaft alignment method in the field for a practical reason: the readings translate directly into a graphical picture of shaft position, which makes the math straightforward and the corrections easy to communicate on the shop floor. Any millwright can learn the graphical procedure in a single shift.

### The alignment procedure, start to finish

1. **Get familiar with the terms, techniques, and procedure** before you're standing at the machine. Knowing what you're measuring and why makes every step after this one faster.
2. **Walk the machine first.** Visually check the coupling, pipe hangers, base bolts, and coupling spacing before you touch an indicator. Problems you catch here — a loose hanger, a stripped bolt — save you from chasing a bad reading later.
3. **Know your tool.** Reverse indicator brackets, dial indicators, and mounting hardware all behave a little differently depending on setup. Confirm yours before you're mid-job.
4. **Prepare the machine.** Remove all existing shims from under the feet and clean the base thoroughly. Old shim stacks and debris under the feet will throw off every reading that follows.
5. **Install the brackets.** Mount the alignment brackets and clean the mounting surface so the bracket sits flat and doesn't introduce its own error.
6. **Take your measurements**, then work through soft foot, horizontal movement, vertical movement, and — where the equipment runs hot — thermal movement. See the individual pages below for each step.

### Related pages
- [Alignment Tolerances](/alignment-tolerances)
- [Sag Check](/sag-check)
- [Soft Foot Check](/soft-foot-check)
- [Horizontal Movement](/horizontal-move)
- [Vertical Movement](/vertical-move)
- [Thermal Movement](/thermal-movement)

---

## 2. Alignment Tolerances
**Status: Partially recovered — flag before publishing**

### H1: Alignment Tolerances

A good rule of thumb for general-purpose equipment running at 3600 RPM or less: **.0005" (half a thousandth) per inch of coupling span.** This figure uses only two variables — shaft speed and coupling span — which is exactly why it works as a fast field check: no reference tables, no equipment-specific data sheet required, just a number a millwright can apply on the spot.

It's a rule of thumb, not a substitute for manufacturer-specified tolerances when you have them. Higher-speed equipment, specialty couplings, and critical service applications typically call for tighter, equipment-specific tolerances — check the OEM spec or your plant's alignment standard when one exists.

**On API 686 / ANSI S2.75:** these are the two reference standards most commonly cited for shaft alignment tolerance and methodology in industrial and petrochemical settings. If your plant or your customer's spec calls out API 686 or ANSI S2.75 compliance, use their documented tolerance tables rather than the general rule of thumb above — this page gives you the fast field number, not a substitute for a cited spec.

**What I could not recover:** the legacy page may have included a fuller tolerance table (offset/angularity broken out by RPM band) — search only ever surfaced this single rule-of-thumb figure, consistently and identically, across multiple queries. I'm not including additional numbers because I can't verify them. **If a fuller table existed on the original page, it needs to come from an archived copy or from Jason directly — not reconstructed from memory or industry norms**, since a wrong tolerance number here is the kind of error that actually costs a customer.

---

## 3. Sag Check
**Status: Recovered**

### H1: Sag Check

Before you trust a reading from your alignment brackets, confirm the brackets themselves aren't introducing error. Bracket sag — the amount an indicator bracket physically droops under its own weight across a given span — is real, and it shows up as false misalignment in your readings if you don't account for it.

### How to check for sag

Clamp the brackets on a sturdy piece of pipe, set at the same distance apart they'll be when mounted on the actual equipment. Zero both indicators at the top position, then rotate them to the bottom.

The difference between the top reading and the bottom reading is your sag value.

Sag will always show as a negative value. That means when you're accounting for sag during the vertical move, **always start your dial indicator with a plus (+) reading** — build the sag allowance in before you take your working measurements, not after.

### Why this matters

Skip the sag check and you're correcting for an error that doesn't exist in the machine — it exists in your bracket setup. That's a wasted shim adjustment at best, and a genuinely misaligned machine at worst if it masks a real problem underneath the false reading.

---

## 4. Soft Foot Check
**Status: Recovered**

### H1: Soft Foot Check

Soft foot happens when one of a machine's feet doesn't sit flat on its base — the foot or the base has warped, or there's debris/paint buildup underneath — so tightening that foot's bolt physically distorts the machine frame. Left uncorrected, it throws off every alignment reading you take afterward, because you're aligning a machine that's being twisted by its own mounting bolts.

Check for soft foot before you do anything else with your indicators — it's step one for a reason.

### How to check for soft foot

1. Move both indicators to the 12 o'clock position, depress them, and zero them out.
2. Loosen one base bolt. If the indicator moves away from zero, that foot has soft foot — note how much movement you see, since that's roughly how much shim you'll need to correct it.
3. Slide the correct amount of shim stock under that foot, retighten the bolt, and confirm the dial indicator needle doesn't move when you retighten. If it holds at zero, the foot is corrected.
4. Repeat for each remaining foot.

### Why this comes first

Every later step — sag check, horizontal move, vertical move — assumes the machine is sitting flat and undistorted on its base. Correct soft foot before you touch the coupling alignment, or you'll be chasing a moving target.

---

## 5. Horizontal Movement
**Status: Recovered**

### H1: Horizontal Movement

The horizontal move positions the two shaft centerlines correctly side-to-side. There are two ways to work it, depending on whether you want a documented graphical record or you just need the machine moved fast.

### Method 1: Graph it

Using square grid graph paper, mark the point under each indicator position that represents half the indicator reading. Connect those two points with a line, and extend that line past the motor's feet. Where the line crosses each foot position tells you exactly how far — and in which direction — that foot needs to move.

This method gives you a documented, visual record of the move, which is useful if you need to show the correction or file it with the job.

### Method 2: Walk it in

If you don't need the graphical record, you can walk the machine into position directly: zero the indicators on the left, then rotate to the right. Turn the indicator needles halfway back toward zero, then start moving the machine — move the farthest foot toward zero first, then the nearest foot. Alternate between the two feet, moving each a little at a time, until both indicators read zero.

Either method gets you to the same result. Graph it when you need the record; walk it in when you just need the machine moved.

Once the horizontal move is complete, move on to the vertical move.

---

## 6. Vertical Movement
**Status: Recovered — but contains a specific worked numeric example. Confirm before publishing.**

### H1: Vertical Movement

The vertical move positions the two shaft centerlines correctly up and down — this is the step that usually calls for adding or removing shims under the feet.

### How it works

Zero your indicators at the top position and take your reading at the bottom. Each indicator's reading represents twice the actual offset at that point — so the real correction at each measurement point is half the total indicator reading.

**Worked example:** say the pump-side indicator reads -12 and the motor-side indicator reads +8. Half of each of those readings — -6 and +4 — is the actual offset at each point.

Using square grid graph paper, mark those half-reading points under each indicator position (-6 for the pump side, +4 for the motor side), then connect them with a line and extend it past the positions representing the motor's feet. Where that line crosses each foot tells you the shim correction needed at that foot — in this example, the front foot needs a .003" shim added and the back foot needs a .001" shim added.

### A flag on this example

The specific numbers above (-12 / +8 readings, .003" / .001" shim corrections) came back consistently across multiple independent recovery searches, which gives me reasonable confidence this is genuinely the original worked example from the legacy page — but I have no way to double-check the arithmetic against a verified original source in this environment. **The method (half the indicator reading, graph it, extend the line to the feet) is solid and matches standard reverse-indicator practice. Before this goes live, have someone check that the specific numbers in the worked example are internally consistent** — I did the arithmetic myself and it holds (half of -12 is -6, half of +8 is +4), but I'd rather flag it than have a bad worked example teaching someone the wrong move.

---

## 7. Thermal Movement
**Status: Newly written — NOT a verified restoration. Needs Jason's technical sign-off before publishing.**

### H1: Thermal Movement

None of the recovery searches for this page returned content specific to ALINE's original page — only generic third-party material (Fluke, Acoem, and similar industry sites) about thermal growth in general. Per instructions, I'm not presenting that as recovered ALINE content, and I'm not including specific thermal-growth formulas or figures as fact, since I can't verify they match what was actually on the original page — or that they're the numbers ALINE wants representing the brand.

What follows is a deliberately general, non-numeric placeholder — enough to have a real H1 and real body text so the page isn't empty, but written to avoid asserting anything technical I can't back up.

### Why thermal movement matters

Machines that run cold and shut down cold are only half the alignment story if they run hot in operation. As equipment comes up to operating temperature, the casing and shaft can grow enough to shift the coupling out of the alignment you set at ambient temperature. On equipment where this matters, the target isn't "aligned when cold" — it's "aligned when running," which means intentionally offsetting the cold alignment so the shafts land on-center once the machine reaches operating temperature.

### What this means in the field

Not every machine needs a thermal growth correction — it depends on operating temperature, shaft length, and equipment type. Where it does apply, getting the cold-alignment offset right requires equipment-specific data (operating temperature, material, centerline height), not a generic rule of thumb.

**This page needs Jason's input before it goes live:** either the original thermal-growth guidance ALINE used to publish (if it can be found in an archive), or a decision on what level of technical detail — including whether to publish a specific growth-calculation method — ALINE wants to stand behind here. I'd rather leave this thin and correct than fill it with a formula I can't verify as either accurate or originally-ALINE's.

---

## Assumptions made
- Treated repeated, independently-worded search results returning the *same specific fact or figure* as a reasonable proxy for "recovered from the original page," since I don't have direct Wayback Machine/browser access in this environment. This is a **search-based reconstruction, not a verified archive pull** — flagging this explicitly so nobody downstream mistakes it for a byte-for-byte restoration.
- Reused two pieces of language already live and verified elsewhere on the current site (per the SEO audit): "any millwright can learn the graphical procedure in a single shift" (homepage) on the Introduction page. Did not invent new product claims.
- Kept persona language to millwright/maintenance technician throughout — no "reliability engineer" language introduced, consistent with the SEO audit's finding that the site has zero drift on this.
- Did **not** add the complementary-laser-tool positioning or API 686/ANSI S2.75 as a dedicated explainer here — those are separate content gaps the SEO audit flagged as their own projects (Content Gap A and B), not something to fold into a restoration pass. I did add one clean, non-fabricated mention of API 686/ANSI S2.75 on the Tolerances page, since it's a direct fit and doesn't require a number I can't back up.
- Internal links on the Introduction page use the current live Wix slugs (`/alignment-tolerances`, `/sag-check`, etc.) as confirmed by the SEO audit — whoever implements this should double check slugs haven't changed since 2026-08-03.

## What needs Jason's technical sign-off before publishing
1. **Thermal Movement** — entirely fresh, not a restoration. Needs either real archived content or Jason's call on what to publish.
2. **Vertical Movement's worked example** (-12/+8 readings, .003"/.001" shims) — high confidence it's genuinely recovered, but worth a second set of eyes on the numbers before it's live and teaching someone a shim correction.
3. **Alignment Tolerances** — the single rule-of-thumb figure is solid and recovery-confirmed; if a fuller original tolerance table existed, it wasn't recoverable through search and shouldn't be reconstructed from general industry knowledge.

## Next steps
- **Whoever rebuilds the Wix pages** (Jason, or a dev) — this is copy-ready content for the 6 non-flagged sections; hold Thermal Movement until sign-off.
- **design-visual-specialist** — the Horizontal Movement and Vertical Movement pages both reference a graph-paper method (plot points, connect a line, extend past the feet). A simple SVG diagram for each would make these pages significantly more usable than text-only description, and it's exactly the kind of precision-diagram work that should be built directly rather than through Claude Design.
- **seo-technical-content-specialist** — once this copy is live, confirm H1s/title tags on all 7 pages match the audit's recommendations (§5 of the audit) and re-check that these pages are actually indexing after the fact.
- If someone gets interactive browser/Wayback Machine access before publishing, it's worth a direct check of `web.archive.org/web/*/alinemfg.com/*.htm` against this draft — particularly for Thermal Movement, where nothing here is a verified restoration.
