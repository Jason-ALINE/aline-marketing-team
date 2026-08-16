# ALINE Manufacturing — Tier 3 Quick Wins + A-3000 / Homepage / Category Page Pass
**Date:** 2026-08-10
**Scope:** Draft-and-hold recommendations only — I don't have Wix publish access. Someone with Wix editor access (Jason or a developer) applies these directly.
**Covers:** Master list Tier 3 #10 (brand capitalization), #13 (About Us H1), Tier 2 #7 (`/a-3000`), Tier 2 #6 (homepage meta description), Tier 2 #8 (`/tool-sets`, `/shop`).

**A note on verification method, per team standard of distinguishing checked-vs-assumed:**
- `/about-us` and `/a-3000` render enough static content for my WebFetch tool to pull real title tags and body copy — those items below are marked **CONFIRMED (live check today)**.
- The homepage, `/tool-sets`, `/shop`, and `/contact` are JS-heavy Wix pages that WebFetch can't get past (same limitation the Aug 3 audit hit — it returns rendered body text but not the `<head>` title/meta tags). I don't have Wix SEO Settings panel login access as an agent, so I couldn't complete the panel check the task suggested. Those items were originally marked **UNVERIFIED — needs direct Wix panel check.**
- **Update, later same day (2026-08-10):** the Manager pulled the live Wix SEO Settings table directly (Marketing > SEO & GEO > SEO Settings > Main Pages, all 20 rows) via browser. That closes the gap above — every item below that was previously UNVERIFIED is now marked **CONFIRMED (Wix panel pull, Manager, 2026-08-10)**, with the real current title tags and meta descriptions as pulled. Note: the Manager's table view truncates long strings (shown as "..." below) — full untruncated text needs a click into each individual row in Wix, which hasn't been done yet. Treat the truncated fragments as confirmed-as-far-as-they-go, not confirmed-complete.

---

## 1. Brand-name capitalization ("ALINE" vs "ALine" vs "A-Line") — Tier 3 #10

**Full picture, now confirmed** — the Manager pulled the complete Wix SEO Settings table (all 20 main pages) directly, closing out the "I'd bet there are more" flag from my earlier draft. There are **three variants in the wild, not two**: correct "ALINE," wrong "ALine," and a separate wrong hyphenated "A-Line" (Tool Sets meta only). **8 of 20 main pages need a fix, both title tag and meta description on each** (not just the title tag, as my earlier draft assumed):

| Page | Current title tag | Current meta description | Verification | Corrected title tag |
|---|---|---|---|---|
| A-1000 | `A-1000 Alignment Tool Set \| ALine...` (truncated) | Not flagged as wrong in the pulled data — verify on click-in | CONFIRMED (Wix panel pull, Manager, 2026-08-10) | `A-1000 Alignment Tool Set \| ALINE...` |
| A-750 | `A-750 Alignment Tool Set \| ALine...` (truncated) | `...by ALine Manufacturing replaces the...` (truncated) | CONFIRMED (Wix panel pull, Manager, 2026-08-10) | `A-750 Alignment Tool Set \| ALINE...` / meta: `...by ALINE Manufacturing replaces the...` |
| A-2000 | `A-2000 Alignment Tool Set \| ALine...` (truncated) | `...by ALine Manufacturing is perfect...` (truncated) | CONFIRMED (Wix panel pull, Manager, 2026-08-10) | `A-2000 Alignment Tool Set \| ALINE...` / meta: `...by ALINE Manufacturing is perfect...` |
| A-3000 | `A-3000 Alignment tool \| ALine Manufacturin...` (truncated) | `...by ALine Manufacturing is the top...` (truncated) | CONFIRMED both by Wix panel pull and my own live WebFetch check today — see item 3 below, title tag is being replaced entirely, capitalization fix folds into that edit | `A-3000 Reverse-Indicator Alignment Tool Set \| ALINE Manufacturing` (title); meta needs "ALine" → "ALINE" at minimum, fuller rewrite proposed in item 3 |
| Contact | `CONTACT \| ALine Manufacturing \| Texa...` (truncated) | `CONTACT ALine Manufacturing USA for...` (truncated) | CONFIRMED (Wix panel pull, Manager, 2026-08-10) | `CONTACT \| ALINE Manufacturing \| Texas, USA` / meta: `CONTACT ALINE Manufacturing USA for...` |
| Accessories | `Accessories \| ALine Manufacturing Texas...` (truncated) | `...ALine Manufacturing tool sets are...` (truncated) | CONFIRMED (Wix panel pull, Manager, 2026-08-10) | `Accessories \| ALINE Manufacturing Texas...` / meta: `...ALINE Manufacturing tool sets are...` |
| About Us | `ABOUT US \| ALine Manufacturing Texas...` | `We manufacture patented precision shaft alignment tools. ALine...` (truncated) | CONFIRMED both by Wix panel pull and my own live WebFetch check today (title only, via WebFetch — meta confirmed via panel pull) | `ABOUT US \| ALINE Manufacturing Texas, USA` / meta: `...ALINE...` |
| Tool Sets | `Precision Alignment Tool Sets \| ALine...` (truncated) | `Alignment tool sets, by A-Line Manufacturing serve chemical...` (truncated) — **note: this is the one page using the separate hyphenated "A-Line" variant, not "ALine"** | CONFIRMED (Wix panel pull, Manager, 2026-08-10) | `Shaft Alignment Tool Sets \| ALINE Manufacturing` (also serves Tier 2 #8, see below) / meta: `A-Line` → `ALINE` |

**SHOP does not need this fix** — confirmed via the same panel pull that SHOP's title ("SHOP \| Shaft Alignment Tools \|...") and meta ("Shop shaft alignment tools from ALINE Manufacturing, the industr...") already use correct "ALINE" capitalization in both fields. Dropped from the affected-pages list; earlier drafts of this item did not have SHOP flagged either, so no correction needed there, just confirming it's clean.

**Pages already correct, no fix needed (confirmed via the same pull):** HOME, Alignment Tolerances, Soft Foot, Vertical Movement, Horizontal Movement, INSTRUCTIONS, Introduction, Sag Check, SHOP, BLOG, Thermal Movement — all already read "ALINE" in both title and meta.

**One-line note on Introduction and Sag Check specifically:** these are the two pages content-copywriting-specialist just rebuilt body content for (Tier 0 #1 in the master list). Good news — they don't need any title-tag/meta work from me; both already have solid, correctly-branded tags in the Wix table (Introduction: "Introduction | ALINE Manufacturing" / "Learn the reverse dial indicator method of shaft alignment. ALINE..."; Sag Check: "Sag Check | ALINE Manufacturing" / "Learn how to measure and compensate for indicator bracket..."). These were set up correctly before the content gap existed — only the body copy needed restoring, not the metadata.

Recommend a single Wix title/meta editing pass across these 8 pages rather than treating each as a separate task — same fix pattern (swap "ALine"/"A-Line" for "ALINE") applied 8 times.

---

## 2. About Us — missing H1 (Tier 3 #13)

**Confirmed missing** (no H1 tag on the page — logo/nav straight into body copy).

**Actual opening body copy, quoted verbatim from a live check today:**
> "Welcome to Aline Manufacturing. We manufacture and sell our patented line of precision shaft alignment tools." ... "Aline is the Industry Standard for chemical plants, water treatment plants, pipeline companies, and other industries." ... "Aline Manufacturing was founded by Richard Massey in 1983 and continues to provide reliable, accurate, and affordable alignment tools."

So the page's own voice leans on: precision, patented, industry-standard, founded 1983, reliable/accurate/affordable. A generic H1 would undersell what's already there.

**Recommendation — two options, your call on how much personality vs. straightforward SEO you want:**

| Option | H1 | Why |
|---|---|---|
| A — safe/generic | `About ALINE Manufacturing` | Matches what was suggested in the task; clean, unambiguous, no risk of clashing with body tone |
| B — matches the page's actual opening line (recommended) | `About ALINE Manufacturing — Precision Shaft Alignment Tools Since 1983` | Echoes the page's own "precision," "1983," and "shaft alignment tools" language rather than being generic. Also naturally reinforces "shaft alignment tools" — the exact phrase the site is stuck on page 2 for site-wide (master list Tier 2 #3) — without forcing it in artificially, since it's already the page's own wording. |

I'd go with B — it's not a rewrite, it's just surfacing language the page already uses into the H1 slot. Not flagging to content-copywriting-specialist since this is a straightforward "lift the H1 from existing copy" job, not a new tone decision. If you want a third option or think B overreaches into their lane, easy to fall back to A.

---

## 3. `/a-3000` — title tag, alt text, thin description (Tier 2 #7)

**Title tag**
- Current (CONFIRMED, live check today): `A-3000 Alignment tool | ALine Manufacturing USA`
- Note: this differs from what the master list's Tier 2 #7 entry stated as current ("A-3000 Tool Set") — that entry was likely carried from an earlier check or GSC snippet rather than the literal live tag. Using today's live-verified text as the actual baseline.
- Proposed: **`A-3000 Reverse-Indicator Alignment Tool Set | ALINE Manufacturing`**
  - Fixes capitalization (item 1 above) in the same edit.
  - Hyphenates "reverse-indicator" to match the company's own standard phrasing (company-brief.md: "reverse-indicator alignment method").
  - Runs ~68 characters — a little past the ~60-char safe zone for full display in search results, but front-loads "A-3000 Reverse-Indicator Alignment Tool Set" so the important part won't get truncated even if the tail end does. Acceptable tradeoff; flag if you'd rather shorten further (e.g., drop to "A-3000 Alignment Tool Set | ALINE Manufacturing" if truncation risk bothers you more than the added keyword).

**Alt text**
- Task brief and master list state current alt text as: `A 3000 Alignment Tool Set Near me USA`
- My live check today instead found: `A 3000 Alignment Tool Set in USA` on the $2,575 "with indicators" product image — no "near me" in what I could retrieve. Flagging this discrepancy rather than picking one silently; worth a 10-second look in the Wix Media Manager to see the literal current string before editing. Possible explanations: it's been edited since the master list's Aug 10 note, or my tool is only surfacing one of several alt-text variants Wix stores.
- **Regardless of which exact string is currently live, the fix is the same direction**: drop "near me" (this is B2B/mail-order, not local-storefront search intent — a millwright ordering a $2,000+ tool set isn't searching "near me") and make it descriptive.
- Proposed: **`A-3000 reverse indicator shaft alignment tool set with dial indicators.`**

**Other product images on the same page — checked as requested**
The `/a-3000` page has two SKU images: "A-3000 Tool Set with Indicators" ($2,575) and "A-3000 Tool Set" ($2,075, base kit). I could only confirm alt text on the first. **The second image appears to have no alt text at all** — a bigger gap than "near me" phrasing, since it's contributing nothing to accessibility or image search. Proposed alt text for it, kept deliberately generic since I don't have a verified spec for what's excluded from the base kit (don't want to invent a feature claim):
**`A-3000 reverse indicator shaft alignment tool set — base kit, ALINE Manufacturing.`**
If content-copywriting-specialist can confirm what's actually different about the base kit (indicators sold separately? different bracket count?), that alt text could be sharpened — flagging as a nice-to-have, not blocking.

**Product description — flagging, not writing**
Current description ("This is the Combination Set...") is thin, as the master list already notes. This is content-copywriting-specialist's lane. Flagging again here since it's sitting right next to the alt-text/title-tag fix and easy to bundle into the same edit pass once they're ready — language already proven elsewhere on the site (reverse-indicator method, no batteries/calibration/subscriptions, millwright-learnable-in-a-shift) would be the natural source material.

---

## 4. Homepage meta description (Tier 2 #6)

**Status: CONFIRMED it exists (Wix panel pull, Manager, 2026-08-10).** This resolves the "possibly missing" framing in my earlier draft — it's not a presence question anymore, it's a quality question.

- Title tag (truncated in the panel view): `ALINE Manufacturing Precision Alignment...`
- Meta description (truncated in the panel view): `ALINE Precision Shaft Alignment Tools offer industry alignment tool...`
- Both fields already use correct "ALINE" capitalization and the meta opens with the core positioning (precision, shaft alignment). The panel table view truncates both fields, so full text hasn't been read yet — that needs someone to click into the HOME row directly in Wix. Given what's visible, this is likely fine as-is; I'd hold off rewriting until the full text is pulled rather than replacing something that may already be solid.

**Draft meta description, kept as a candidate** in case the full text turns out weak or generic once pulled (not because presence is in doubt anymore):

> **ALINE Manufacturing makes reverse-indicator shaft alignment tools for millwrights & maintenance crews. Precision pump and motor alignment — no lasers, no calibration.**

~140 characters, fits within display limits with room to spare. Hits: reverse-indicator method (the core differentiator), millwright language (correct buyer, not "reliability engineer"), and works in "pump" alignment naturally as a descriptor rather than forcing the exact GSC query phrase "pump alignment tool" — matches the guidance in master list item #3 not to force that phrase in if it reads awkwardly. Use only if the full existing text (once pulled) is actually thin — don't swap out a description that's already doing its job.

---

## 5. `/tool-sets` and `/shop` — title/meta pass (Tier 2 #8)

**Status: CONFIRMED for both (Wix panel pull, Manager, 2026-08-10).** H1s were already confirmed correct in my earlier draft:
- `/tool-sets` H1: "Shop ALINE Manufacturing Tool Sets" (correct capitalization, fine as-is)
- `/shop` H1: "Shop ALINE Manufacturing" (correct capitalization, fine as-is)

Now title/meta are confirmed too, and they need **different treatment from each other**:

- **`/shop` — no fix needed.** Confirmed title: `SHOP | Shaft Alignment Tools |...` and meta: `Shop shaft alignment tools from ALINE Manufacturing, the industr...` (both truncated in panel view). Both look solid and correctly branded — this is the same page flagged clean in item 1 above. Leave as-is beyond the duplicate-content-risk check below, which still holds.
- **`/tool-sets` — needs the brand fix.** Confirmed title: `Precision Alignment Tool Sets | ALine...` (wrong — "ALine") and meta: `Alignment tool sets, by A-Line Manufacturing serve chemical...` (wrong — and specifically the hyphenated "A-Line" variant, the only page using that exact form). This is the same fix scoped in item 1's table above; draft replacement below.

| Page | Current (confirmed) | Draft/proposed |
|---|---|---|
| `/tool-sets` title | `Precision Alignment Tool Sets \| ALine...` | `Shaft Alignment Tool Sets \| ALINE Manufacturing` |
| `/tool-sets` meta | `Alignment tool sets, by A-Line Manufacturing serve chemical...` | `Complete reverse-indicator shaft alignment tool sets for millwrights and maintenance crews — no lasers, no calibration required.` (or, if a lighter edit is preferred, just swap "A-Line" → "ALINE" in the existing sentence and keep the rest) |
| `/shop` title | `SHOP \| Shaft Alignment Tools \|...` | No change — already correct |
| `/shop` meta | `Shop shaft alignment tools from ALINE Manufacturing, the industr...` | No change — already correct |

**One thing still worth a quick sanity check while you're in there:** if `/shop` and `/tool-sets` list overlapping or identical products, make sure their meta descriptions stay distinct (as drafted above) so they don't cannibalize each other in search results — not flagging this as a confirmed problem, just a five-minute check worth doing since both pages showed up separately in the master list's GSC data.

---

## Summary table — what's confirmed vs. what needs a direct check

**Update, 2026-08-10 (later same day):** the Manager pulled the full Wix SEO Settings table (all 20 main pages), closing out nearly everything that was UNVERIFIED in the original draft below. Only the alt-text discrepancy and full-untruncated-text pulls remain open.

| Item | Verification status |
|---|---|
| About Us title tag (has "ALine") | CONFIRMED (WebFetch live check + Wix panel pull, both today) |
| About Us missing H1 | CONFIRMED live today |
| A-3000 title tag (has "ALine") | CONFIRMED (WebFetch live check + Wix panel pull, both today) |
| A-3000 alt text wording | Still a discrepancy between master list and my live check — verify exact string in Wix Media Manager before editing (not part of the SEO Settings table, so the panel pull doesn't resolve this one) |
| A-3000 second product image missing alt text entirely | CONFIRMED live today (found via check) |
| A-1000 / A-750 / A-2000 / A-3000 / Contact / Accessories / About Us / Tool Sets — brand capitalization (title + meta) | CONFIRMED (Wix panel pull, Manager, 2026-08-10) — 8 pages, both fields, see item 1 above. SHOP confirmed clean, dropped from the list. |
| Homepage meta description presence | CONFIRMED it exists (Wix panel pull) — full untruncated text still needs a click-into-row pull; quality (not presence) is now the open question |
| `/tool-sets` title/meta | CONFIRMED needs the brand fix — "ALine" (title) and "A-Line" (meta) |
| `/shop` title/meta | CONFIRMED clean, no fix needed |
