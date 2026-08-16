# Amazon Marketplace Listing Audit — ALINE Manufacturing
**Date:** 2026-08-03
**Status:** LIVE-VERIFIED (Manager, via browser, 2026-08-03) — the link works. See "Live verification" section below; it supersedes the "INCOMPLETE" findings underneath, which are kept for the tool-limitation record but should not be treated as current.

---

## Live verification (Manager, browser check, 2026-08-03)

Jason's link is correct: `https://www.amazon.com/s?srs=121078674011&rh=p_89%3AA-Line%2BMfg`
returns **8 real ALINE listings**, deliverable to Johnson City TX, seller of
record "A-Line Manufacturing" (self-fulfilled, not FBA):

| Product | Price |
|---|---|
| A-3000W (combo, with indicators) | $2,575 |
| A-2000W (combo, with indicators) | $2,375 |
| A-3000 (combo, no indicators) | $2,075 |
| A-2000 (combo, no indicators) | $1,875 |
| A-750W (with indicators) | $1,420 |
| A-1000W (with indicators) | $1,845 ("See options" / 1 new offer — worth checking, reads like a possible buy-box/offer issue) |
| A-750 (no indicators) | $920 |
| A-1000 (no indicators) | $1,345 |

**Biggest finding: every listing has zero reviews, and they're brand new.**
Opened the A-1000 listing (ASIN B0HBZ4T342) directly — "Date First Available:
July 28, 2026," six days before this audit, "There are 0 customer reviews."
None of the 8 search-result cards show a star rating either, consistent with
all of them being newly (re)published rather than one listing being an
outlier. **This means Tomas Tinajero's incoming testimonial (pending as of
2026-08-03, see project memory) has a real chance of becoming the first-ever
Amazon review on the exact listing his replacement bracket came from** — the
A-1000 listing's "What's in the box" line is literally "1000A and 1000B
Brackets, Telescoping Tubes, Mounting Hardware, Instructions." If he's open
to it, this is worth prioritizing over a generic ask once his reply comes in.

**Listing copy is better than expected — already carrying current
positioning, not stale:**
- A-1000 bullets already reference API 686, ANSI S2.75, pipe strain, soft
  foot, runout, and bearing clearance by name, and already frame the tool
  against laser systems on a price/capability basis ("LAB-GRADE METHOD,
  CREW-LEVEL PRICE... same reverse-indicator accuracy behind $5,000–$15,000+
  laser alignment systems").
- The product description explicitly says the reverse-indicator method
  "surfaces pipe strain, soft foot, runout, and bearing clearance problems —
  issues that live outside what a laser reads."
- **Gap: this is a laser-replacement/comparison framing, not the newer
  complementary-use angle** (run ALINE *alongside* a laser tool, confirmed
  2026-08-01 in company-brief.md). The listing copy predates that positioning
  update — worth revisiting once there's bandwidth, lower priority than the
  review gap.

**Images are thin.** Only 3 thumbnails on the A-1000 listing, all
case/product shots (case closed, case open, one partial view) — no in-use or
lifestyle photography anywhere. This directly matches the ask already sent to
Tomas Tinajero for an in-use photo — if he sends one, it's a legitimate
candidate for the Amazon image gallery, not just a website testimonial.

**Did not check:** the "A-LINE-IT" brand-collision risk the earlier pass
flagged (unrelated woodworking product), full image galleries on the other 7
listings, or Q&A/review content on other ASINs. Worth a follow-up pass, not
urgent given the zero-review finding is the bigger story right now.

---

## Original pass (tool-limited — kept for record, see live verification above)

I could not confirm the link Jason provided, and I could not independently
locate any live "A-Line Mfg" branded Amazon listings through fallback
searches. This is not the same as confirming ALINE has zero Amazon
listings — it means my available tools (web search, no live browser/fetch,
no Seller Central access) were not able to surface them either way. Before
treating "no listings" as fact, someone needs to actually open the link in
a browser or paste in a product URL/ASIN.

**Recommended immediate next step:** Jason (or outreach-sales-specialist,
who owns the Amazon distributor relationship and may already have Seller
Central visibility) confirms with a screenshot or pasted ASIN/URL whether
ALINE has active listings. Once that exists, I can do the actual
title/bullets/images/reviews audit this task originally scoped.

---

## What I tried

1. **The link Jason gave**
   `https://www.amazon.com/s?srs=121078674011&rh=p_89%3AA-Line%2BMfg`
   The `p_89` parameter is Amazon's brand-refinement filter, and `A-Line
   Mfg` is URL-encoded correctly in it — structurally, this looks like a
   plausible "all listings under brand A-Line Mfg" search. But I have no
   browser/fetch tool, only a web-search tool that queries an index, not a
   live page renderer. Amazon's search-results pages are dynamic/JS-driven
   and generally aren't captured in a way a search index can return. My
   search tool returned generic, unrelated Amazon boilerplate for this
   URL — not a rendered result, not a "0 results" confirmation either.
   **I cannot verify this link one way or the other.**

2. **Fallback brand searches** — `"A-Line Mfg" Amazon`, `ALINE
   Manufacturing Amazon`, `A-Line Mfg Amazon brand store`, `A-Line Mfg
   Amazon shaft alignment bracket`, `A-1000 alignment tool set A-Line
   site:amazon.com`, `ALINE Johnson City Texas shaft alignment tool
   amazon.com` — none surfaced a genuine ALINE Manufacturing / A-Line Mfg
   product page, ASIN, or brand storefront on Amazon.

3. **Category/keyword searches** a buyer might use — `reverse indicator
   shaft alignment bracket API 686 amazon`, `pipe strain alignment bracket
   amazon buy` — surfaced only competitor and unrelated products (Starrett,
   SKF, generic pipe clamp brackets), never ALINE.

## Findings worth flagging even without a confirmed listing

- **Brand-name collision risk.** Multiple searches surfaced a product
  called **"CDIYTOOL A-LINE-IT"** — a woodworking table-saw/band-saw
  dial-indicator alignment gauge, completely unrelated to ALINE
  Manufacturing, sold by a different company. The name is close enough
  ("A-Line-It" vs. "A-Line") that it's plausibly already competing for the
  same search terms and could dilute or confuse buyers searching "a line
  alignment tool" on Amazon. If ALINE does list on Amazon (or plans to),
  this is worth a defensive-SEO check: does "A-Line" / "ALINE" search
  traffic on Amazon actually land on ALINE's listings, or on this
  unrelated woodworking product? Worth a manual check by whoever has
  Seller Central or browser access.
- **ALINE's own site has a direct `/shop` page** (`alinemfg.com/shop`).
  Combined with not being able to find Amazon listings, it's possible
  ALINE's primary online sales channel today is direct-to-web rather than
  Amazon — which would reframe this from "optimize existing listings" to
  "should we be on Amazon at all, and if so with what." That's a strategy
  question, not a copy question — flagging so it doesn't get missed.
- **Unverified location discrepancy** — a third-party business directory
  (ZoomInfo) lists "A-line Mfg., Inc." at Liberty Hill, TX, while
  `company-brief.md` states Johnson City, TX. I'm not treating either as
  confirmed fact here (directory data is often stale/wrong), but flagging
  per the known-pitfalls protocol: this should be verified once, not
  carried forward silently either direction.

## What I could NOT verify (tool limitations — be honest about these)

- No live browser or URL-fetch capability — I cannot open and render the
  actual Amazon search-results page Jason linked.
- No Seller Central or Amazon MCP access — backend search terms, sales
  rank, ad performance, and account-level listing data are invisible to
  me regardless.
- Web search indexing of Amazon's own dynamic search pages is
  unreliable/sparse — a "no results found" from my tool is not equivalent
  to "no listings exist." Treat my search as inconclusive, not negative.

## What the original audit scope still needs (once listings are confirmed)

For each real listing, once someone hands me a URL, ASIN, or screenshots:
- Title keyword coverage (reverse-indicator alignment, shaft alignment
  bracket, API 686, pipe strain, soft foot, specific model numbers like
  "1000A bracket")
- Bullet/description quality against the real buyer (millwright,
  maintenance supervisor, contract-firm PM) and real use case — not a
  reliability-engineer-flavored generic feature dump
- Image count/type — plain product-on-white vs. in-use/lifestyle shots
- Review count, average rating, recurring themes
- Whether the complementary-use-with-laser-tools angle appears anywhere,
  or whether copy is still framed only as a laser replacement
- Visible-copy keyword density as a proxy for likely backend search-term
  richness (can't see backend terms directly)

I'm not fabricating placeholder findings for any of these — there's no
real listing content to evaluate yet, and inventing plausible-sounding
scores would be worse than reporting the gap.

---

## Ranked opportunities (based on what's actually confirmed today)

1. **Confirm listing status at all — highest priority.** Everything else
   is blocked on this. Five minutes of Jason (or anyone with a browser)
   opening the link and reporting what's there unblocks the real audit.
2. **Check the "A-LINE-IT" collision** once someone has browser access —
   if ALINE brand search traffic on Amazon is landing on an unrelated
   woodworking product, that's a real, fixable diversion of buyer intent.
3. **Decide the Amazon strategy question** — if there are no (or minimal)
   live listings, this becomes a market-research-specialist /
   outreach-sales-specialist conversation about whether Amazon is worth
   building out as a channel at all, separate from optimizing copy on
   listings that may not exist yet.
4. **Once real listing content exists**, prioritize title + bullet rewrite
   for keyword coverage and buyer-persona alignment (millwright/contract
   PM, not reliability engineer) — that's typically the highest-leverage,
   lowest-cost fix in Amazon marketplace SEO, and squarely in this
   specialist's lane.
5. **Add the complementary-use-with-laser angle** to any listing copy
   once confirmed live — this is newer positioning (confirmed 2026-08-01
   per company-brief) and likely hasn't made it into any existing
   marketplace copy yet, since it postdates most existing ALINE content.

---

## Key assumptions made
- None of the "top opportunities" above assume specific listing content
  exists — they're sequenced to get to ground truth first rather than
  audit content I never actually saw.
- I treated the ZoomInfo Liberty Hill, TX detail as unverified noise, not
  a correction to company-brief.md — did not edit company-brief based on
  a single unconfirmed third-party directory entry.

## Next specialist / person
- **Jason** — confirm the link directly (or paste an ASIN/product URL/
  screenshot) so a real audit can run.
- **outreach-sales-specialist** — likely already has or can get Seller
  Central visibility as the owner of the Amazon distributor relationship;
  worth checking before assuming this needs to start from zero.
- **content-copywriting-specialist (me)** — ready to run the full
  title/bullets/images/reviews audit and rewrite as soon as real listing
  content is available. Do not hand this to design or SEO yet — nothing
  to act on until listings are confirmed.
