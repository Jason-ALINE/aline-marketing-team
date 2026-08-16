# ALINE Manufacturing — Master Website Improvement List
**Date:** 2026-08-10
**Status:** This supersedes `2026-08-03-website-seo-audit.md` and `2026-08-10-prioritized-fix-list.md` as the document to work from. Those two aren't deleted — they hold the underlying research/methodology — but don't split attention between three files anymore. This is the punch list.
**Scope:** alinemfg.com organic web presence only. Amazon marketplace SEO is not in here — that's content-copywriting-specialist's lane.
**Sources folded in:** Aug 3 audit, Aug 10 GSC-driven fix list, today's content-draft finalization notes (complementary-use + API 686 pages), the Manager's live-browser check today (instructions pages + Wix SEO Assistant panel), and a second Manager verification pass today using PageSpeed Insights/Lighthouse, Google's Rich Results Test, and direct browser navigation (resolved the legacy `.htm`, schema, and Core Web Vitals items; surfaced a new meta-description rendering bug — item 2a).

---

## Tier 0 — Fix first: broken guided procedure, real users are hitting dead ends right now

### 1. The `/instructions` flow sends users to three pages that don't exist as content
**Status, confirmed by direct browser check today:**
- LIVE with real content: `/alignment-tolerances`, `/horizontal-move`, `/vertical-move`, `/thermal-movement`
- EMPTY (nav/header only, no body): `/introduction`, `/soft-foot-check`, `/sag-check`

**What's wrong:** This isn't just "some pages are thin" — it's a broken multi-step tutorial. The four live pages actively instruct readers to complete the three empty ones first. Horizontal Move and Vertical Move both open with a red linked line — "Haven't measured your bracket distances yet? Set up and measure A, B, and C on the Introduction page first" — and list "BEFORE YOU START" requirements including "A soft foot check already done on the machine" and "a sag check already done on your bracket setup," both pointing at empty pages.

**Why it matters:** A real millwright or technician following the site's own guided sequence — the exact person this site exists to serve — hits three dead ends mid-procedure. This is a functional/trust failure, not a ranking problem, and it's worse than the Aug 10 fix list's framing (which treated `/instructions` as one thin page with traffic). Ranking this above the GSC-driven priorities below because it actively fails people who are already on the page trying to do the job.

**Fix:**
- Content-copywriting-specialist restores real body content on `/introduction`, `/soft-foot-check`, `/sag-check`. Aug 3's legacy-cache research strongly suggests this is a restoration job (pre-migration `.htm` content existed) rather than a from-scratch write — same pattern that produced the now-confirmed-live `/alignment-tolerances` content.
- Add H1s to all three while rebuilding (missing sitewide on `/instructions` pages per Aug 3, still true for these three).
- **Note, confirmed 2026-08-10 via Wix SEO Settings panel pull:** Introduction and Sag Check (two of the three) already have solid, correctly-branded title tags and meta descriptions set in Wix — e.g. Introduction: "Introduction | ALINE Manufacturing" / "Learn the reverse dial indicator method of shaft alignment. ALINE..."; Sag Check: "Sag Check | ALINE Manufacturing" / "Learn how to measure and compensate for indicator bracket...". These don't need new title/meta work below, only the body-content restoration itself. Soft Foot Check's title/meta wasn't part of the pulled table (page name may differ in Wix's list) — treat its proposed title/H1 pair below as still open until confirmed.
- Title tag / H1 pairs ready for Content to write into (carried from Aug 10 fix list, unchanged — kept as the fallback/reference version, though Introduction and Sag Check's live tags above are effectively already this or better):

| Page | Proposed title tag | Proposed H1 |
|---|---|---|
| `/introduction` | Shaft Alignment Instructions — Reverse-Indicator Method \| ALINE Manufacturing | How to Perform Reverse-Indicator Shaft Alignment |
| `/soft-foot-check` | Soft Foot Check — Detect & Correct Soft Foot in Pump/Motor Alignment \| ALINE Manufacturing | Soft Foot Check — How to Detect and Correct Soft Foot |
| `/sag-check` | Sag Check Procedure for Shaft Alignment \| ALINE Manufacturing | Sag Check — Correcting Bracket Sag Before Alignment |

- **Interim mitigation worth considering until the rebuild ships** (flagging as a judgment call for Jason, not unilaterally recommending a copy change): the red "BEFORE YOU START" pointers on the four live pages are currently sending real users into dead ends. Until the three empty pages are live, it may be worth softening or temporarily removing those specific prerequisite call-outs (or adding a one-line "content coming soon" placeholder on the empty pages) so the guided flow doesn't actively break mid-procedure. This is a content/UX call, not mine to make unilaterally — flagging to content-copywriting-specialist and Jason together.

---

## Tier 1 — High-priority technical fixes, cheap, no content dependency

### 2. Site not connected to Bing Webmaster Tools — DONE, connected today
**Source:** Wix's own SEO Assistant panel (Marketing > SEO & GEO), checked live today — flagged as the panel's single HIGH-priority item.
**Why it matters:** Google Search Console is connected (confirmed working, GSC data is what drove the Aug 10 fix list), but Bing has zero visibility into the site. Bing + Yahoo + AI-assistant crawlers that lean on Bing's index (Copilot, some others) get nothing.
**Fix:** Connect alinemfg.com in Bing Webmaster Tools and submit `sitemap.xml` (already exists and is correctly structured per Aug 3 audit — no new sitemap work needed). Roughly 15–30 minutes, no content dependency, no developer needed.
**Status:** Connected today (2026-08-10). See the new Off-site / Backlinks section below for what Bing's own tool flagged as its top recommendation now that it has data.

### 2a. NEW (2026-08-10, Manager verification pass) — Homepage meta description configured in Wix but not rendering in live HTML
**Source:** Google's Lighthouse SEO audit (run via PageSpeed Insights on the live homepage, mobile) flagged "Document does not have a meta description." This directly contradicts Wix's own SEO Settings panel, which shows a meta description IS configured for the homepage (title: "ALINE Manufacturing Precision Alignment..." / meta: "ALINE Precision Shaft Alignment Tools offer industry alignment tool..." — confirmed present in the admin panel earlier the same day).
**Why it matters:** The tag is configured correctly in Wix's backend but isn't actually reaching the live page's rendered HTML — this is a real technical bug (possible Wix rendering/caching issue or theme/template override), not a missing-content gap. It directly affects the SERP snippet on the site's single highest-traffic page (256 clicks / 21,596 impressions — see Tier 2 item 6).
**Fix:** Investigate from the Wix dashboard first (re-save the SEO settings, check for a conflicting app/theme override); if it doesn't resolve, file a Wix support ticket. Re-test with Rich Results Test or a view-source check once addressed. No content rewrite needed — the copy itself is fine, it's a rendering problem.
**Priority:** Higher urgency than the rest of Tier 3 below — flagging as Tier 1 because it's cheap to investigate, has no content dependency, and sits on the site's most-visited page.

---

## Tier 2 — Real-data-backed content/SEO gaps (GSC-verified demand, reuse of Aug 10 research)

### 3. Site sits on page 2 (avg. position 12.9) for its three highest-volume buyer-intent queries
**Data:** "shaft alignment tools" (3,480 impr., 2 clicks), "pump alignment tool" (3,109 impr., 2 clicks), "shaft alignment tool" (1,163 impr., 2 clicks) — combined ~7,750 impressions converting almost nobody. For contrast, branded search ("aline tool") converts at 15.7% CTR, so this isn't a trust or snippet-quality problem — it's a ranking-depth problem.
**Why it matters:** This is the single biggest opportunity on the site and it's a content-depth problem, not a title-tag problem — position 12.9 gets clicked rarely no matter how good the snippet is. Thin `/instructions` pages (Tier 0), no API 686/ANSI S2.75 content (until today, see below), and thin product descriptions are almost certainly why the site can't out-rank competitors on these generic terms.
**Fix:** No new landing page needed for these specific terms — natural home is the homepage (already targets "reverse indicator"/"millwright" well; check H1/title contains a natural variant of "shaft alignment tool(s)" without forcing "pump alignment tool" in if it reads awkwardly — propose as a sub-head instead, e.g. "built for pump and compressor alignment in the field") and `/tool-sets` reinforcement. Real movement on these terms requires the site-wide content-depth build-out (items 1, 6, 7, 8 in this list), not a one-page fix.

### 4. Two new pages are drafted, fact-checked, and SEO-finalized — ready to publish, not yet live
**Status as of today:** Both the complementary-use-with-laser page and the API 686/ANSI S2.75 explainer are fully drafted (content-copywriting-specialist) and finalized (slug, title tag, meta description, internal linking plan — this specialist, today):
- `/laser-alignment-pipe-strain-check` — title: "Laser Alignment + Pipe Strain Check | ALINE Manufacturing"
- `/api-686-ansi-s2-75-alignment-standards` — title: "API 686 & ANSI S2.75 Alignment Standards | ALINE Manufacturing"

Both pages' standards claims (API 686 scope, ANSI S2.75 scope, the .0005"/inch tolerance figure) are independently verified against public sources — no fact-check blocker remains.

**What's left, not a research gap — an execution gap:**
- Publish both pages.
- Build the internal links specified in each draft's finalization notes, both directions: Pipe Strain blog post → complementary-use page; Soft Foot blog post → complementary-use page; `/post/shaft-runout-deflection-and-whip` → complementary-use page; `/alignment-tolerances` ↔ both new pages; About Us → API 686 page; the two new pages → each other and → `/a-1000`/`/a-2000`/`/a-3000`.
- These are sentence-level edits on existing pages (adding a hyperlink to existing anchor text, in a few cases extending a sentence) — flagged to content-copywriting-specialist since wording changes, not pure URL swaps, are involved on a few of them (see each draft's "Internal linking plan" section for the full table).

### 5. `/post/shaft-runout-deflection-and-whip` — proven traffic, dead end
**Data:** 54 clicks / 5,956 impressions — the strongest non-homepage page on the site, with clean H2 structure. It has zero outbound links.
**Fix:** Add a link to a relevant product page (`/a-3000` or whichever tool addresses runout), a link to the matching `/instructions` sub-page once rebuilt, and hyperlink the existing "Upgrade to ALINE alignment tools" CTA rather than leaving it as bare text. Also add the new complementary-use-page link here (see item 4). Write/confirm a meta description while in there. Body copy/voice untouched — this is link/meta scaffolding only.

### 6. Homepage — biggest page on the site, worth a targeted check, not a rewrite
**Data:** 256 clicks / 21,596 impressions — by far the site's largest page, already using real buyer language well ("reverse indicator," "millwright").
**Fix:** Verify/write a meta description (unconfirmed whether one exists — highest-value page to fix first if it's missing). Check current H1/title against "shaft alignment tool(s)" phrasing (see item 3) — don't force "pump alignment tool" if it's awkward. This alone won't move position 12→1; it's the cheap part of a bigger content-depth fix.

### 7. `/a-3000` — strong CTR already, worth investing in
**Data:** 68 clicks / 719 impressions, 9.5% CTR (well above site average — this page already converts what it gets).
**Fix:**
- Title tag: "A-3000 Tool Set" → "A-3000 Reverse Indicator Alignment Tool Set | ALINE Manufacturing"
- Alt text: "A 3000 Alignment Tool Set Near me USA" → "A-3000 reverse indicator shaft alignment tool set with dial indicators." (drop "near me" — this is B2B/mail-order, not local-storefront search intent; check other product images for the same pattern)
- Product description is thin ("This is the Combination Set..."). Flag to content-copywriting-specialist to expand using language already proven elsewhere on site (reverse-indicator method, no batteries/calibration, millwright-learnable-in-a-shift). Given the CTR here, better copy is likely to lift conversion more than most other items on this list.

### 8. `/tool-sets` and `/shop` — same title/meta pass, lower urgency
**Data:** `/tool-sets` 16 clicks / 1,347 impr.; `/shop` 11 clicks / 507 impr. No page-specific findings beyond the sitewide thin-title/unverified-meta gap — moved up the queue only because they have measured traffic.

### 9. No dedicated content for two of the three real buyer personas
**Finding:** "Millwright" is used correctly (About Us, homepage). "Maintenance supervisor" is not used verbatim anywhere (closest: "maintenance technicians"). "Contract-firm project manager" is absent entirely. Not a drift problem — the site never says "reliability engineer" — it's a coverage gap. Homepage's existing "outfits an entire team" language is a decent hook for both roles but isn't developed into anything dedicated.
**Fix:** Flag to content-copywriting-specialist as a future content angle, not urgent enough to jump the queue ahead of items 1–8.

---

## Tier 3 — Lower-priority technical/cosmetic items

| # | Item | Note |
|---|---|---|
| 10 | Brand-name capitalization | **Scope confirmed 2026-08-10 via the Manager's direct Wix SEO Settings panel pull (all 20 main pages).** 8 pages affected, both title tag AND meta description on each: **A-1000, A-750, A-2000, A-3000, Contact, Accessories, About Us, Tool Sets.** Two wrong variants in the wild — "ALine" (most pages) and "A-Line" hyphenated (Tool Sets meta only, uniquely). Standardize all to "ALINE" (all caps). SHOP was checked and is already correct in both fields — not part of this fix. The other 11 main pages (HOME, Alignment Tolerances, Soft Foot, Vertical/Horizontal Movement, INSTRUCTIONS, Introduction, Sag Check, BLOG, Thermal Movement) are also confirmed correct. This replaces the earlier narrower guess of 4 pages (Tool Sets, A-3000, Contact, About Us) with the full verified 8-page list. Free to fix while editing these titles anyway (overlaps with #7/#8/#13). See `2026-08-10-tier3-quick-wins.md` item 1 for exact current-vs-corrected text, page by page. |
| 11 | Legacy `.htm` URL cleanup | **DONE (2026-08-10, Manager verification pass).** Confirmed live via direct browser navigation that these return a genuine 400 Bad Request (not a fetch-tool artifact, not a standard 404 — Wix's router appears to reject the `.htm` extension pattern outright). All 8 legacy URLs now handled: `/tolerances.htm` → `/alignment-tolerances`, `/A-2000.htm` → `/a-2000`, `/A-3000.htm` → `/a-3000`, `/sagcheck.htm` → `/sag-check`, `/vertical.htm` → `/vertical-move`, `/procedure.htm` → `/introduction`, `/products.htm` → `/shop` (per Jason's direction — shop includes accessories/individual items, not just tool sets) — all set as 301 redirects via Wix's URL Redirect Manager (Marketing > SEO & GEO > "URL redirect") and verified live/working. `/customers.htm` had no confident current-site mapping, so rather than guess, it was submitted to Google Search Console's Removals tool (temporary ~6-month block, renewable) to stop it cluttering search results — nothing on the current site maps to it and nothing links to it anymore. No further action needed. |
| 12 | Sitewide meta descriptions | Still unverified via available tooling whether these exist/are unique on pages not covered in Tier 2 (fetch tool doesn't expose raw `<meta>` tags). Needs a direct pass through the Wix SEO panel, page by page. |
| 13 | Missing H1 — About Us | Confirmed missing (separate from the `/instructions` pages already covered in Tier 0). Two options drafted in `2026-08-10-tier3-quick-wins.md`, recommending "About ALINE Manufacturing — Precision Shaft Alignment Tools Since 1983" (pulled from the page's own opening copy) over the plain generic version. |
| 14 | Schema markup / structured data | **RESOLVED, confirmed healthy (2026-08-10, Manager verification pass).** Tested live via Google's Rich Results Test on the homepage: 3 valid structured data items detected — Breadcrumbs (1 valid item), Local Business (1 valid item, named correctly "ALINE Manufacturing"; one non-critical optional-field gap, missing `priceRange`, not worth fixing), Organization (1 valid item, one minor non-critical issue, not further detailed). Wix's default schema generation is working correctly. No action needed beyond optionally adding a `priceRange` value if Jason wants it — purely cosmetic. |
| 15 | Core Web Vitals / page speed / mobile rendering | **RESOLVED, confirmed healthy (2026-08-10, Manager verification pass).** Tested live via PageSpeed Insights on the homepage, mobile. Real-user field data unavailable ("No Data" — site doesn't have enough Chrome UX Report traffic yet; expected for a low-traffic site, not a red flag). Lab/simulated scores: Performance 81, Accessibility 93, Best Practices 100, SEO 92. Nothing in the red 0–49 band; Performance at 81 is "orange" (50–89) — not perfect but not concerning, no technical-penalty pattern. Mobile only; desktop wasn't tested — optional low-priority follow-up if Jason wants full coverage. Note: this same test flagged a real bug (missing rendered meta description on homepage) — see new Tier 1 item 2a above, not a Tier 3 item. |
| 16 | Wix SEO Assistant — "Publish a new blog post" | Low-priority Wix nudge. Folds into the broader content-depth need above (Tier 2) rather than being a separate task. |
| 17 | Wix SEO Assistant — "Perform a site inspection" | Low-priority, generic Wix nudge with no specifics attached. Worth a quick look inside the Wix dashboard, but not detailed enough to action from here. |
| 18 | General blog → product/instructions internal linking | Beyond the specific links already scoped in Tier 2 items 4–5, neither the Pipe Strain nor Soft Foot post links to product pages currently. Low priority beyond what's already scoped. |

---

## Off-site / Backlinks (new finding — Bing Webmaster Tools, connected today)

### 19. Bing Webmaster Tools' top recommendation: not enough inbound links from high-quality domains
**Source:** Bing Webmaster Tools, connected today (2026-08-10, see item #2 above) — this was its #1 flagged recommendation once it had site data to work with.
**What it means:** Backlinks — other sites linking to alinemfg.com. Right now Bing sees too few links from domains it considers authoritative. This is a distinct signal from anything else in this list; everything above is on-page or technical. This is off-site.
**Why it's here and not higher priority:** This is a longer-term item, not a quick fix — you can't manufacture quality backlinks in an afternoon the way you can fix a title tag. Flagging it accurately rather than turning it into a project: possible angles worth a future look (not scoping any of these out further right now) — industry directories/supplier listings, distributor partner pages linking back (ties into outreach-sales-specialist's Motion Industries/Grainger work if those relationships produce a listing page), or guest/contributed technical content on an industry publication. This is a candidate for a future outreach-sales-specialist or content-copywriting-specialist angle, not something to action from this list alone.
**Fix:** No action from me this round — logging the finding. Worth a conversation with Jason about whether it's worth pursuing now or parking it.

---

## Not mine to action — referral only

- **"Launch a Google Ads campaign"** — Wix SEO Assistant's medium-priority recommendation. This is paid distribution, not organic SEO — route to paid-ads-specialist if Jason wants to pursue it. Not on this punch list as an SEO task.

---

## Already fine — don't re-do this

- **`/alignment-tolerances`** — confirmed live today with full real content, including the ".0005\" per inch of coupling span" tolerance figure. No longer part of the `/instructions` gap. Both new draft pages already link to it correctly.
- **Wix's 14 completed SEO Assistant items** — search engine indexing enabled site-wide (blog categories, blog posts, gallery items, main pages, store categories), Google Search Console connected, site confirmed indexable. Don't spend time re-checking or re-enabling any of these.
- **robots.txt / sitemap.xml** — verified correct: not blocking real content, sitemap resolves with 4 sub-sitemaps, all URLs reachable.
- **Persona language / no reliability-engineer drift** — verified zero mentions of "reliability engineer" anywhere on site; "millwright" and "reverse indicator" are used correctly on homepage and About Us. The gap here is coverage (item 9 above), not a wrong-persona correction.
- **API 686 / ANSI S2.75 factual claims (in the new draft page)** — independently verified against public sources today (GlobalSpec, ANSI/ASA store listings, Fluke/Ludeca tolerance guidance). No further fact-check needed before publishing.
- **Branded search performance** — "aline tool" converts at 15.7% CTR. The problem is top-of-funnel discovery (page 2 on generic terms), not brand trust or snippet quality once someone's already looking for ALINE.
- **Legacy `.htm` URLs (Tier 3 item 11)** — confirmed done 2026-08-10 (Manager verification pass, live browser + Wix Redirect Manager + GSC Removals tool). All 8 legacy URLs handled. See Tier 3 table for the full mapping. Don't re-check.
- **Schema markup / structured data (Tier 3 item 14)** — confirmed healthy 2026-08-10 via Google's Rich Results Test. Breadcrumbs, Local Business, and Organization all valid; only cosmetic gaps (optional `priceRange`). Don't re-check.
- **Core Web Vitals / page speed (Tier 3 item 15)** — confirmed healthy 2026-08-10 via PageSpeed Insights, mobile (Performance 81 / Accessibility 93 / Best Practices 100 / SEO 92). No technical-penalty pattern. Desktop untested but low-priority optional follow-up only. Don't re-check unless scores are needed again after a site change.

---

## Still genuinely unverifiable from where I sit
All three previously-listed items here were resolved via the Manager's live-tool verification pass on 2026-08-10 (PageSpeed Insights / Lighthouse, Rich Results Test, direct browser navigation) — see Tier 3 items 11, 14, 15 and the "Already fine" section above. Nothing currently sits in this bucket.
