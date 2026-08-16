# ALINE Manufacturing — Prioritized SEO Fix List (Search Console-Driven)
**Date:** 2026-08-10
**Supersedes prioritization (not findings) of:** `2026-08-03-website-seo-audit.md`
**What changed:** Real Google Search Console data (last 3 months, site-wide) now exists for the first time. This re-ranks the Aug 3 fast/cheap fix list by proven demand instead of theoretical SEO value. GA4 just went live today — too new for behavioral data (bounce, time on page), so this pass is GSC + Aug 3 findings only.

**Site-wide baseline (3 mo):** 500 clicks / 37,400 impressions / 1.3% CTR / avg. position 12.9 (page 2 — most searchers never see it).

---

## Headline finding before the punch list

**Real buyer-intent demand exists at high volume and the site is on page 2 for almost all of it.** Three near-identical high-volume queries are getting seen tens of thousands of times combined and converting almost nobody:

| Query | Impressions | Clicks | CTR |
|---|---|---|---|
| shaft alignment tools | 3,480 | 2 | 0.06% |
| pump alignment tool | 3,109 | 2 | 0.06% |
| shaft alignment tool | 1,163 | 2 | 0.17% |
| *(for contrast)* aline tool (branded) | 89 | 14 | 15.7% |

This is not a title-tag/CTR problem primarily — at average position 12.9, expected CTR is naturally low (page 2 gets clicked rarely regardless of how good the snippet is) even for compelling copy. **The real signal is a ranking-depth problem, not a click-through problem**: the site can't crack page 1 for exactly the generic terms real buyers (millwrights, maintenance supervisors, contract-firm PMs — matches the brief's persona, good sign) are typing. That tracks with what the Aug 3 audit already flagged as content gaps: no API 686/ANSI S2.75 page, seven empty `/instructions` pages, thin product descriptions. Thin, shallow site = hard to out-rank competitors on competitive generic terms even when the pages that do exist are decently optimized. Fixing titles/meta on existing pages is still worth doing (see below) but won't move position 12→1 on its own — that needs the content-depth build-out from Aug 3 §5 (longer-term list), now with hard evidence it's the actual bottleneck, not a nice-to-have.

I want to flag this distinction clearly because it changes what "fixing SEO" means here: technical/on-page cleanup earns back clicks on pages *already* getting impressions; it does not by itself fix why the site sits on page 2 for its highest-value generic terms. Both need to happen, but they're different projects with different owners (this list = me; content depth = content-copywriting-specialist).

---

## Tier 0 — Fix these first: pages with proven clicks/impressions already

Ranked by clicks, since that's the clearest signal of "real people already land here."

### 1. `/instructions` — highest-leverage item on this entire list
**Data:** 9 clicks / 503 impressions (1.8% CTR — above the 1.3% site average) on a page the Aug 3 audit found to be **almost entirely empty** (no body text, no H1, legacy content never migrated from the old `.htm` site).

This is the single most important new finding from the GSC pull: real buyers are already finding and clicking into a page with nothing on it. That's not a hypothetical content gap anymore — it's demand with no landing content to serve it. Every other fix on this list is optimization; this one is a page actively failing people who already showed up.

**Correction, 2026-08-10 (Manager's direct browser verification of the live site, not a re-audit of this list):** `/alignment-tolerances` is confirmed LIVE with full real content, including the exact ".0005\" per inch of coupling span" figure referenced below — this sub-page is no longer part of the gap and can be dropped from the restoration action. `/introduction`, `/soft-foot-check`, and `/sag-check` are confirmed still empty, matching the original Aug 3 finding. Horizontal/Vertical/Thermal Movement weren't individually re-checked in this pass — assume still empty until confirmed otherwise. Net effect: this is now a 6-page gap (or possibly fewer, pending a check on the three unverified Movement pages), not 7, and the "restoration job" framing below still holds for the remaining pages.

- **Action:** Restore/rebuild the remaining `/instructions` sub-pages with real body content (Introduction, Sag Check, Soft Foot Check, Horizontal/Vertical/Thermal Movement — Alignment Tolerances is done, see correction above). Legacy Google cache of `tolerances.htm` shows this content existed pre-migration (e.g., the ".0005" per inch of coupling span" tolerance figure, now confirmed restored on `/alignment-tolerances`) — this is very likely a restoration job for the rest too, not a from-scratch write.
- **Add H1s** while rebuilding (was already flagged Aug 3 as missing sitewide on these 7 pages — do it in the same pass as the content restoration, not separately).
- **Flag to content-copywriting-specialist:** this needs their voice/procedure-accuracy ownership, not an SEO-only rewrite. I can spec headers/titles once drafted (see Tier 2 title proposals below).
- **My contribution now (no content dependency):** propose title tag + H1 pairs per sub-page so Content has a target to write into, e.g.:

| Page | Proposed title tag | Proposed H1 |
|---|---|---|
| Soft Foot Check | Soft Foot Check | Detect & Correct Soft Foot in Pump/Motor Alignment \| ALINE Manufacturing | Soft Foot Check — How to Detect and Correct Soft Foot |
| Alignment Tolerances | ~~Shaft Alignment Tolerances \| Reverse-Indicator Method \| ALINE Manufacturing~~ | ~~Shaft Alignment Tolerances — Reverse-Indicator Method~~ — **page confirmed live 2026-08-10 with real content already published; this proposed title/H1 is moot unless the live page's actual title/H1 needs a separate on-page check against the pattern below.** |
| Introduction | Shaft Alignment Instructions — Reverse-Indicator Method \| ALINE Manufacturing | How to Perform Reverse-Indicator Shaft Alignment |
| Sag Check | Sag Check Procedure for Shaft Alignment \| ALINE Manufacturing | Sag Check — Correcting Bracket Sag Before Alignment |
| Horizontal / Vertical / Thermal Movement | [Movement Type] Correction in Shaft Alignment \| ALINE Manufacturing | Same pattern per page |

(Carried forward from Aug 3 audit §5 item #4, unchanged — just reprioritized to the top given the traffic evidence.)

---

### 2. `/post/shaft-runout-deflection-and-whip` — proven organic performer, currently a dead end
**Data:** 54 clicks / 5,956 impressions — the strongest non-homepage page on the site by impressions, and a real content asset (clean H2 structure per Aug 3 audit).

**Problem (from Aug 3, now higher priority given the traffic):** this post doesn't link anywhere. Someone reads a well-ranking technical post about shaft runout and hits a wall instead of a next step.

- **Specific edit:** Add internal links from this post to:
  - A relevant product page (`/a-3000` or whichever tool actually addresses runout checking)
  - The matching `/instructions` sub-page once restored
  - A CTA at the end: "Upgrade to ALINE alignment tools" (or similar existing phrase, per Aug 3) should be a hyperlink, not bare text.
- **Meta description:** unverified whether one exists (same gap as Aug 3 §1) — write/confirm one now since this page has proven search volume; low effort, direct payoff.
- **Flag:** don't touch the body copy/voice — this is link/meta scaffolding only, not a rewrite.

---

### 3. Homepage — 256 clicks / 21,596 impressions, by far the site's biggest page
Already the strongest performer and already targets real buyer language well per Aug 3 §2 (uses "reverse indicator," "millwright" correctly). Two things worth doing here:

- **Verify/optimize meta description** — same sitewide gap flagged Aug 3 §1, but this page has the most impressions on the site so it's the highest-value place to fix it first if descriptions are indeed missing or generic.
- **Natural title/H1 check against the two big missed queries** ("shaft alignment tool(s)," "pump alignment tool") — if the current title/H1 doesn't already contain a natural variant of these phrases, consider working one in verbatim rather than only the "precision brackets" phrasing the Aug 3 audit found in the indexed snippet. Example, not a rewrite: if current H1 is close to "Precision Shaft Alignment Tools," that already covers it — I don't have the exact current H1 text to confirm, so this needs a direct check before editing anything. **Do not force "pump alignment tool" in if it reads awkwardly** — propose instead as a sub-head or About-adjacent sentence ("built for pump and compressor alignment in the field") which covers the term without stuffing.
- **Bigger point:** don't expect a title/meta tweak here to move the position-12.9 needle much on its own — see the headline finding above. This page's ceiling on those generic terms is a content-depth/authority problem across the site, not something this one page can fix by itself.

---

### 4. `/a-3000` — 68 clicks / 719 impressions (9.5% CTR — well above site average, this page already converts what it gets)
- **Title tag** (carried from Aug 3 §5 #4): current *"A-3000 Tool Set"* → proposed *"A-3000 Reverse Indicator Alignment Tool Set | ALINE Manufacturing"*.
- **Alt text** (carried from Aug 3 §5 #5): current *"A 3000 Alignment Tool Set Near me USA"* → proposed *"A-3000 reverse indicator shaft alignment tool set with dial indicators."* Drop "near me" — this is B2B/mail-order, not local-storefront search intent.
- **Thin product description** (Aug 3 Content Gap E) — flag to content-copywriting-specialist to expand using proven homepage language (reverse-indicator method, no batteries/calibration, millwright-learnable-in-a-shift). Given this page already has a strong CTR, better copy here is likely to lift conversion more than most other fixes on the list — worth moving up Content's queue.

---

### 5. `/tool-sets` (16 clicks / 1,347 impressions, ~1.2% CTR) and `/shop` (11 clicks / 507 impressions, ~2.2% CTR)
- Apply the same title-tag and meta-description pass as above. No page-specific findings beyond what Aug 3 already flagged sitewide (thin titles, unverified meta descriptions) — these just move up the queue because they have measured traffic and the other pages with zero GSC data don't.

---

## Tier 1 — Sitewide technical fixes with no page-specific traffic data, but cheap and still worth doing

These were "fast/cheap" in the Aug 3 audit and remain so — they just rank below Tier 0 now because there's no GSC evidence yet that a specific page is losing clicks over them. Do these once Tier 0 is done, or in parallel if it's a five-minute fix.

| # | Fix | Where | Note |
|---|---|---|---|
| 1 | Brand-name capitalization | Tool Sets, A-3000, Contact titles ("ALine" → "ALINE") | Polish, not ranking-impactful, but free to fix while editing these titles anyway (overlaps with #4/#5 above). |
| 2 | Legacy URL 301 redirects | `/products.htm`, `/customers.htm`, `/tolerances.htm`, `/A-2000.htm`, `/A-3000.htm`, `/procedure.htm`, `/sagcheck.htm`, `/vertical.htm` | Still unverified whether these are true 404s (Aug 3 flagged this). No GSC data was given for these old URLs specifically, so I can't confirm how much current search traffic is hitting a dead end here — recommend checking Search Console's Page Indexing / crawl-error report directly (not covered by the query data provided) before spending time on this. Do it, but it's not urgent based on what's confirmed so far. |
| 3 | Sitewide meta descriptions | All pages not covered in Tier 0 | Same gap as Aug 3 §1 — still unverified via my tooling (fetch doesn't expose raw `<meta>` tags). Needs a direct Wix SEO panel check. |
| 4 | Schema markup / Core Web Vitals / mobile rendering | Sitewide | Still unverified, same as Aug 3. Not indicated as urgent by the GSC numbers given (avg. position problem looks like a content/ranking issue, not a technical-penalty pattern — but I can't rule out CWV as a contributing factor without PageSpeed Insights access). |

---

## Tier 2 — What this data adds that wasn't in the Aug 3 audit

1. **Target these three queries directly and explicitly**, since they're the single biggest concentration of unmet demand on the site:
   - "shaft alignment tools" (3,480 impr.)
   - "pump alignment tool" (3,109 impr.)
   - "shaft alignment tool" (1,163 impr.)
   These map cleanly onto real buyer language (matches company-brief personas — millwrights/maintenance supervisors search functionally, not by standards jargon first), so this isn't a stale/reliability-engineer-drift risk. Natural home for these terms: homepage H1/title (see Tier 0 #3) and potentially a dedicated `/tool-sets` or category-page reinforcement, not a new landing page from scratch — the site doesn't need more pages, it needs the existing ones to rank higher, which is a content-depth issue (see headline finding).

2. **`/instructions` performing at all with empty content is itself new evidence**, not just a coincidence — it confirms Aug 3's Content Gap C (thin `/instructions` pages) is not a theoretical gap, it's the top proven-ROI item on the whole list. Elevated to Tier 0 #1 above.

3. **Page-2 average position (12.9) reframes the whole "fast/cheap fixes" list.** Technical/on-page cleanup (titles, alts, H1s, internal links) is still worth doing — it's what recovers clicks on impressions the site is already getting — but it won't be what moves the big three queries above from page 2 to page 1. That requires the content-depth build Aug 3 already scoped (API 686/ANSI S2.75 explainer, restored `/instructions` pages, expanded product descriptions) — now with hard data that this, not technical debt, is the binding constraint on the site's biggest opportunity.

4. **Branded search converts fine (15.7% CTR on "aline tool")** — confirms the problem isn't distrust of the brand or bad on-SERP presentation once someone's already looking for ALINE by name. The gap is entirely top-of-funnel: getting found by people who don't know the brand yet and are searching functionally.

---

## Needs content-copywriting-specialist before finalizing

- `/instructions` full rebuild (Tier 0 #1) — I've proposed titles/H1s; body content and procedure accuracy is theirs.
- `/a-3000` product description expansion (Tier 0 #4) — flagged as elevated priority given strong existing CTR.
- Any homepage copy change beyond a possible title/H1 tweak (Tier 0 #3) — I haven't proposed a rewrite, only flagged where a natural keyword variant might fit; needs their voice call if it goes beyond title tag/meta.
- Longer-term: API 686/ANSI S2.75 explainer and complementary-use-with-laser content remain unassigned from the Aug 3 audit and are now more clearly tied to the ranking-depth problem above — recommend the Manager sequence one of these next given this data.

## Still unverified (carried from Aug 3, unchanged by this pass)
- Actual meta description tags (no raw HTML access)
- Schema markup
- Core Web Vitals / page speed / mobile rendering
- True 404 status of legacy `.htm` URLs
