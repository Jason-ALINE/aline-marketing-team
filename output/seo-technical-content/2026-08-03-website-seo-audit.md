# ALINE Manufacturing — Website SEO Audit (alinemfg.com)
**Date:** 2026-08-03
**Scope:** Organic web search visibility only (alinemfg.com). Amazon marketplace SEO is out of scope — owned by content-copywriting-specialist.
**Method:** Direct page fetches (homepage, About Us, Contact, all 7 /instructions pages, Shop, Tool Sets, 3 product pages, Blog index, 2 full blog posts), sitemap.xml + sub-sitemaps, robots.txt, and Google search-index spot checks (`site:alinemfg.com` and phrase searches). No access to Google Search Console, PageSpeed Insights/Lighthouse, or a rendering crawler (Screaming Frog) in this environment — flagged explicitly wherever that limits confidence.

Platform: **Wix** (confirmed via robots.txt signature — `/_partials*`, `/pro-gallery-webapp/*`, auto-generated-by-SEO-tools note — and `/product-page/`, `/post/` URL patterns).

---

## 1. Technical SEO

| Item | Finding | Confidence |
|---|---|---|
| Indexability / robots.txt | Not blocking any real content. Only blocks `?lightbox=` params, `/_partials*`, `/pro-gallery-webapp/*` (Wix internals), and PetalBot. Sitemap correctly referenced. | Verified |
| Sitemap | `sitemap.xml` → 4 sub-sitemaps (pages, blog posts, blog categories, store products), all resolve, all URLs 200-reachable. 19 pages, 5 blog posts, 12 product URLs indexed. Reasonable structure for site size. | Verified |
| **Legacy URL cleanup — biggest technical finding** | Old pre-Wix URLs are **still live in Google's index**: `alinemfg.com/products.htm`, `/customers.htm`, `/tolerances.htm`, `/A-2000.htm`, `/A-3000.htm`, `/procedure.htm`, `/sagcheck.htm`, `/vertical.htm` all show up in search results today. When fetched now, these return errors rather than resolving or 301-redirecting to the current Wix pages. That means: (a) Google may still be crawling/re-indexing dead URLs, wasting crawl budget and creating broken-link SERP entries; (b) any backlinks or bookmarks pointing at the old URL structure aren't passing link equity to the new site because there's no redirect chain. | **Verified that old URLs are indexed** (search); **fetch attempts returned HTTP 400**, but I can't fully rule out that's a fetch-tool artifact rather than the live server's actual response (e.g. true 404 vs. something else). Recommend confirming directly in a browser and in Google Search Console's Page Indexing report before filing this as certain. |
| Title tags | Present and mostly unique across templates (see §2 for content). | Verified |
| Meta descriptions | **Could not verify.** The fetch tool renders visible page text/title, not raw `<meta>` tags — no fetch surfaced a distinct meta description separate from the title on any page. This is a gap in my method, not a confirmed finding that they're missing. | **Unverified — needs direct check** (Wix SEO panel per-page, or a crawler like Screaming Frog) |
| H1 structure | **Missing entirely** on About Us and on all 7 `/instructions` sub-pages (Introduction, Alignment Tolerances, Sag Check, Soft Foot Check, Horizontal/Vertical/Thermal Movement). Present and correct on Shop, product-category pages, and blog posts. | Verified across 6 independently fetched pages |
| Header hierarchy on blog | Blog posts (Pipe Strain, Soft Foot) have clean, logical H2 structure (e.g., "What Causes Pipe Strain?" → "What It Does to Your Equipment" → "Preventing..." → "Identifying..." → "Key Takeaways"). This is the strongest on-page structure on the site. | Verified |
| Thin/empty content on `/instructions` pages | All 5 instructional pages I fetched directly (Soft Foot Check, Alignment Tolerances, Introduction, Horizontal Movement, plus About Us as a related case) returned **no body text at all** — just global nav, social icons, and footer/contact boilerplate. No images with alt text, no embedded PDFs found either. Notably, Google's cache of the *old* `tolerances.htm` page shows this content used to exist as real text (e.g., a tolerance rule-of-thumb figure: ".0005\" per inch of coupling span for general purpose equipment ≤3600 rpm"). This strongly suggests real instructional content existed pre-migration and either didn't carry over to Wix or isn't rendering as text. | High confidence given 5 independent examples + legacy-cache corroboration, but recommend a direct browser check (not just fetch) to rule out a JS-rendering blind spot in my tooling. |
| Schema markup | Could not verify — fetch tool doesn't expose JSON-LD/structured data. Wix stores/blogs often add baseline Organization/Product schema by default, but that's a platform generalization, not a confirmed fact for this site. | **Unverified — run through Google's Rich Results Test** |
| Mobile-friendliness / page speed / Core Web Vitals | Could not verify — no Lighthouse/PageSpeed Insights access in this environment. Wix templates are responsive by default as a platform characteristic, but I have not measured actual load time or CWV for alinemfg.com. | **Unverified — run PageSpeed Insights / check Search Console's Core Web Vitals report directly** |
| Brand-name consistency in titles | "ALINE Manufacturing" (homepage, About Us) vs. "ALine Manufacturing" (Tool Sets, A-3000, Contact) — inconsistent capitalization in title tags across templates. Minor, but an easy fix and a slight brand-polish issue. | Verified |

---

## 2. On-page keyword targeting — is the site ranking-oriented around real buyer language?

**Verdict: partially, and unevenly.** The homepage and About Us page do target real buyer language well. The instructional pages, product pages, and standards terminology are the gaps.

| Target term (from brief) | Found on site? | Where | Notes |
|---|---|---|---|
| "reverse indicator" / "reverse-indicator alignment" | **Yes** | Homepage (per Google-indexed snippet), About Us ("reverse indicator alignment procedure") | Core positioning term is present and used correctly — good. Not reinforced on product pages or instructions pages, though. |
| "pipe strain" | **Yes** | Dedicated blog post title + full post | Real content asset exists, but see Content Gap A below — it never connects the topic back to ALINE tools or the laser-complementary angle. |
| "soft foot" / "soft foot check" | **Yes** | Blog post (full, well-structured) + nav page (empty) | Blog post is solid. The short-URL nav page `/soft-foot-check` — better-positioned for the exact search term — is empty. |
| "API 686" | **No — zero mentions anywhere on site** | — | Verified absent across homepage, About Us, all instructions pages, all product pages, both blog posts checked in full. |
| "ANSI S2.75" | **No — zero mentions anywhere on site** | — | Same as above. |
| "shaft alignment bracket" | **No** | — | Google's cached homepage snippet uses "precision brackets" mechanically, but this phrase isn't reinforced on product pages where a searcher using this term would land. |
| "millwright" | **Yes** | About Us, homepage (per indexed snippet: "Any millwright can learn the graphical procedure in a single shift") | Correct persona targeting — see §3. |
| "maintenance supervisor" | **No** (About Us uses "maintenance technicians," close but not exact) | — | Gap — see §3. |
| "contract-firm project manager" / "contract PM" | **No — zero mentions anywhere** | — | Gap — see §3. |

**Quick assessment:** the site is not generic/brand-only — there's real evidence of intentional buyer-language targeting on the homepage and in blog content. But it's inconsistent: the pages structurally best-positioned to rank for exact-match instructional queries (the `/instructions` nav pages) currently carry the least content.

---

## 3. Persona-language check (known team pitfall: defaulting to reliability engineer)

**No drift toward "reliability engineer" detected — zero mentions anywhere on the site.** This is good; the on-page copy doesn't carry the team's known persona mistake.

However, coverage across the three real buyer personas is **uneven, not wrong**:
- **Millwright** — present and used correctly (About Us, homepage).
- **Maintenance supervisor** — not used verbatim anywhere; closest is "maintenance technicians" (About Us).
- **Contract-firm project manager** — absent entirely.

This isn't a drift problem, it's a coverage gap — worth a note to content-copywriting-specialist rather than a correction. The "outfits an entire team" / team-purchasing language already on the homepage is actually a decent hook for both maintenance supervisors and contract-firm PMs (who buy in bulk for crews) — it just isn't developed into dedicated content for those roles anywhere.

---

## 4. Content gaps, ranked

**A. Complementary-use-with-laser angle — zero content anywhere on site.** *(Highest priority — see summary below.)*
Verified absent from the Pipe Strain post (the single most relevant place for it), the Soft Foot post (which mentions "laser alignment systems" only as one item in a generic list of devices — not the complementary positioning), product pages, and About Us. Given this is Jason's newest confirmed positioning and directly expands the addressable market (owners of a laser tool who don't think they need anything else), this is the biggest gap relative to opportunity size.
*Needs content-copywriting-specialist to draft; SEO can spec structure/keywords once drafted.*

**B. API 686 / ANSI S2.75 — zero content anywhere on site.**
The site's own stated audience (About Us: chemical plants, water treatment, pipeline companies) is exactly the regulated-industry crowd that references these standards in specs and RFQs. Per the brief, this is a real technical hook for this audience, not SEO padding — but there's currently no page that would surface for "API 686 alignment" or similar searches.
*Needs content-copywriting-specialist for the actual explainer; SEO can spec title/headers.*

**C. Thin/empty `/instructions` pages.**
Prime nav real estate, short URLs, exact-match topic titles (Alignment Tolerances, Sag Check, Soft Foot Check, Horizontal/Vertical/Thermal Movement) — but no indexable text. Legacy site had real content here. This is likely a content-restoration project more than a net-new one.
*Needs content-copywriting-specialist collaboration — SEO shouldn't rewrite this unilaterally since original voice/procedure accuracy matters.*

**D. No dedicated content for maintenance supervisor or contract-firm PM personas** (see §3).

**E. Product page descriptions are thin.**
Example — full body copy on the A-3000 product page: *"This is the Combination Set. Features both the A-2000 and A-1000 in the same case. This is our most popular set because it fits most everything from 1" to 10". Great for field servicemen."* Good voice, but it doesn't reuse any of the proven language already live elsewhere on the site (reverse-indicator method, no batteries/calibration, millwright-learnable-in-a-shift). Fast, low-risk win — see §5.

---

## 5. Fast/cheap wins vs. longer-term build-out

### Fast, cheap (technical/on-page — hours, not a content project)

| # | Fix | Where | Specific edit |
|---|---|---|---|
| 1 | Legacy URL cleanup | `alinemfg.com/*.htm` old pages | Set up 301 redirects from each old URL to its new-site equivalent (e.g. `tolerances.htm` → `/alignment-tolerances`), or confirm via Search Console they're already fully deindexed. Reclaims stray backlink equity, kills broken-link SERP entries. |
| 2 | Brand-name consistency | Title tags site-wide | Standardize on "ALINE Manufacturing" (all caps) everywhere — currently mixed with "ALine Manufacturing" on Tool Sets, product pages, Contact. |
| 3 | Missing H1s | About Us + all 7 `/instructions` pages | Add one H1 per page using the real target phrase, e.g. About Us → "About ALINE Manufacturing"; `/soft-foot-check` → "Soft Foot Check — How to Detect and Correct Soft Foot." |
| 4 | Thin title tags | `/soft-foot-check`, `/alignment-tolerances`, `/introduction`, product pages | Current: *"Soft Foot | ALINE Manufacturing"* → Proposed: *"Soft Foot Check | Detect & Correct Soft Foot in Pump/Motor Alignment | ALINE Manufacturing"*. Current: *"A-3000 Tool Set"* (no brand, no keyword) → Proposed: *"A-3000 Reverse Indicator Alignment Tool Set | ALINE Manufacturing"*. Natural phrasing, not stuffed — these are literal descriptions of what the page is. |
| 5 | Alt text | A-3000 product images | Current: *"A 3000 Alignment Tool Set Near me USA"* — awkward, and "near me" implies local-storefront search intent that doesn't match how this B2B/mail-order product is actually bought. Proposed: *"A-3000 reverse indicator shaft alignment tool set with dial indicators."* Check other product images for the same pattern. |
| 6 | Internal linking | Blog posts → product/instructions pages | Neither blog post checked links to a relevant product page or matching `/instructions` page. E.g. in the Soft Foot post, the phrase "soft foot detection" could link to `/soft-foot-check`, and "Upgrade to ALINE alignment tools" CTA could link directly to `/shop` or `/a-3000` rather than being a bare phrase. |
| 7 | Meta descriptions | Site-wide | Unverified whether these exist/are unique (see §1) — quick manual pass once confirmed, cheap to write once the gap is identified. |

### Longer-term (real content projects — route to content-copywriting-specialist)

1. Rebuild the 7 `/instructions` pages as full text content (likely needs the original procedure content restored/rewritten, not just an SEO edit).
2. New pillar post/page: complementary-use-with-laser angle (Content Gap A).
3. New page: API 686 / ANSI S2.75 explainer (Content Gap B).
4. Persona-specific content for maintenance supervisor and contract-firm PM (Content Gap D).
5. Expand product page descriptions with the proven homepage language (Content Gap E) — flagging to Content rather than rewriting unilaterally, since product copy tone belongs to them.

---

## What I could NOT verify (be upfront about this)

- Actual meta description tags (no raw HTML/source access via my tools)
- Schema markup / structured data presence
- Core Web Vitals, page speed, actual mobile rendering
- Whether the legacy `.htm` URLs return true 404s vs. some other error — worth a direct browser/curl check
- Whether the `/instructions` pages are truly empty in Google's rendered view (I used a text-extraction fetch, not a JS-rendering crawler) — recommend a direct browser check before treating this as fully confirmed, though the consistency across 5 independent pages plus the legacy-cache corroboration makes me fairly confident.
