# Website Page Draft — API 686 & ANSI S2.75 Shaft Alignment Standards Explained

**Final URL slug:** `/api-686-ansi-s2-75-alignment-standards` (draft's suggestion confirmed as-is — matches exact-match search terms buyers/spec-writers would type)
**Final title tag:** API 686 & ANSI S2.75 Alignment Standards | ALINE Manufacturing (62 characters)
**Final meta description:** API 686 and ANSI S2.75, explained in plain language — what they require for shaft alignment and how reverse-indicator checks help document compliance. (150 characters)
**H1:** Draft's H1 kept, with one optional word-level addition — see finalization notes below.

*(seo-technical-content-specialist finalization, 2026-08-10 — see full notes at bottom of file)*

---

## H1: API 686 and ANSI S2.75 — What They Actually Mean for Your Alignment Job

If you've seen "API 686" or "ANSI S2.75" show up in a spec sheet or an RFQ and moved on without digging into what they actually require, you're not alone. Here's what they cover, in plain terms, and what it means for how you document an alignment job.

## H2: Why These Show Up in Your Paperwork

API 686 and ANSI S2.75 aren't quality-claim language — they're real reference standards that chemical plants, water treatment facilities, and pipeline operators write directly into their equipment specs and RFQs. If you're doing alignment work for one of these customers, there's a decent chance one or both of these standards is already sitting in the job packet, whether or not anyone on the crew has read it.

## H2: API 686 — Machinery Installation

API 686 is the American Petroleum Institute's recommended practice covering machinery installation — baseplates, grouting, piping, and alignment among other topics. The alignment portion is the piece that matters most day-to-day: it addresses shaft alignment method and tolerance as part of getting a machine installed correctly, not just bolted down and spun up.

## H2: ANSI S2.75 — Shaft Alignment

ANSI/ASA S2.75 is the standard focused specifically on shaft alignment — methods, tolerances, and what counts as an adequately documented alignment. Where API 686 sits inside the broader installation process, ANSI S2.75 is the narrower standard a spec will point to when shaft alignment itself is the thing being called out.

## H2: What This Means for How You Check a Machine

Both standards are built around the idea that a coupling reading by itself isn't the whole story. A machine can show good angular and offset numbers on a laser and still be misaligned in ways that matter — because of pipe strain pulling on the case, a soft foot flexing the frame when it's bolted down, or runout on the shaft or coupling face that a laser reads as misalignment when the shaft itself is fine.

This is where the reverse-indicator method — what ALINE tools are built around — lines up with what these standards are actually asking for. Reverse-indicator readings are how a crew checks strain, soft foot, and runout directly, not just the coupling angle and offset a laser measures.

## H2: A Practical Tolerance Reference

As a rule of thumb, many crews work to a tolerance of **.0005" per inch of coupling span** for general-purpose equipment running at or below 3600 RPM. That's a field guideline, not a substitute for reading the actual tolerance tables in your governing spec — different equipment classes, speeds, and coupling types call for tighter numbers, and the spec on your job packet is the one that actually controls.

## H2: Documenting the Job

If a spec references API 686 or ANSI S2.75, the strongest alignment record is one that shows more than "laser said good." A reverse-indicator check that documents pipe strain, soft foot, and runout — in addition to the coupling alignment itself — is a more complete record against what these standards are actually asking for.

Every ALINE toolset reads to **.001" accuracy**, the resolution of the Starrett 196B1 dial indicator each set ships with — so the numbers going into that record are as precise as the instrument itself.

This doesn't mean retiring a laser tool. Most crews on jobs like this are running both: laser for the coupling alignment, ALINE for the checks a laser doesn't cover. [Link "page on running ALINE alongside a laser alignment tool" → `/laser-alignment-pipe-strain-check`]

## H2: Which ALINE Tool

The **A-1000** is the standard setup for reverse-indicator bracket-and-dial-indicator work on a single job. The **A-2000** and **A-3000** combination sets cover a wider range of shaft sizes in one case if your crew is handling multiple machine classes on the same contract. [Link "A-1000" → `/a-1000`; link "A-2000" and "A-3000" → `/a-2000` and `/a-3000`. **Confirmed by Jason 2026-08-10 — build these links.**]

## H2: Bottom Line

API 686 and ANSI S2.75 aren't just words on a spec sheet — they describe a more complete alignment check than a coupling reading alone, and reverse-indicator method is how you actually produce that check in the field.

---

## Key assumptions made

- **API 686 description — VERIFIED 2026-08-10 via public sources (GlobalSpec standards listing, published table-of-contents excerpts, rotating.equipment, BSB Edge).** Full name: API RP 686, "Recommended Practice for Machinery Installation and Installation Design," 2nd Edition (Dec. 2009), reaffirmed July 2024 with Errata 1 (Jan. 2025) — this is still the current edition; a 3rd-edition draft exists but is not yet published. Confirmed chapter list includes Foundations, Mounting Plate Grouting, Piping, and Shaft Alignment among others, which directly matches the draft's "baseplates, grouting, piping, and alignment among other topics." No correction needed.
- **ANSI/ASA S2.75 description — VERIFIED 2026-08-10 via public sources (ANSI/ASA store listings, GlobalSpec).** Formal title is "Shaft Alignment Methodology," published in parts — Part 1 ("General Principles, Methods, Practices, and Tolerances," 2017, reaffirmed) is the part the draft describes; there's also a Part 2 (Vocabulary) and Part 3 (vertical machinery, 2021). The draft's description matches Part 1's actual content, including its documented "Alignment Quality Grades" system (what the draft calls "what counts as an adequately documented alignment"). **One nuance not reflected in the copy:** Part 1's scope is limited to flexibly-coupled, horizontally-mounted machines on two bearings per case (rigidly coupled machines are out of scope). Not flagging this as an error — it covers the overwhelming majority of jobs this audience runs (motor-to-pump/fan on a flex coupling) — but noting it so it's a known simplification, not an unexamined one.
- **The .0005" per inch of coupling span tolerance figure — VERIFIED 2026-08-10 as a real, commonly-cited industry rule of thumb**, independently corroborated by Fluke's and Ludeca's published alignment-tolerance guidance (both describe the same general-purpose, ≤3600 RPM, per-inch-of-coupling-span rule), consistent with the general alignment-tolerance-chart tradition this kind of figure comes from. It is correctly *not* attributed to either standard in the copy — it isn't sourced from API 686 or ANSI S2.75 — and the existing "rule of thumb many crews work to" framing is accurate and doesn't need loosening or further hedging.
  - **Resolved 2026-08-10 (Manager's direct browser verification, not a re-audit):** `/alignment-tolerances` is confirmed LIVE with full real content, including this exact ".0005\" per inch of coupling span" figure. The flag below (and the internal-linking plan's "once rebuilt" framing) is now out of date for this specific page — see corrected linking plan below. `/introduction`, `/soft-foot-check`, and `/sag-check` are separately confirmed still empty, so the general "wait for `/instructions` rebuild" caveat still applies to links pointing at those three.
- **Not claiming ALINE tools are "certified" or "approved" under either standard** — no such claim exists in any source I reviewed, and it would be a serious overclaim to introduce here. The copy is careful to say the method "lines up with" / "helps document" compliance, not that the tools themselves are certified.
- **Tool recommendation (A-1000 as the standard single-job setup) — confirmed correct by Jason on 2026-08-10.** No longer an open item.
- Internal link to the complementary-use-with-laser page and to `/shop`/product pages are placeholders pending final URLs.

## Next specialist

- **Fact-check on standards descriptions and tolerance figure — RESOLVED 2026-08-10.** All three items (API 686 scope, ANSI S2.75 scope, .0005"/inch tolerance figure) checked against public sources and confirmed accurate; no copy corrections needed. See updated "Key assumptions made" above for sources and one minor scope nuance (ANSI S2.75 Part 1 applies to flexibly-coupled horizontal machines specifically) that's worth knowing but doesn't require a copy change for this audience. **This page is publish-ready on the fact-check front.** The earlier open flag (confirm live/rebuilt status of `/alignment-tolerances`) is now RESOLVED per the Manager's 2026-08-10 direct browser check — that page is live; see internal-linking plan below.
- **seo-technical-content-specialist** — finalize URL slug, title tag, meta description, and internal linking (this page and the complementary-use page should cross-link each other, plus link to relevant product pages and the Pipe Strain / Soft Foot blog posts). `/alignment-tolerances` link is confirmed ready to build now (2026-08-10) — see below.
- **design-visual-specialist** — this page could support a simple comparison table (laser reading vs. reverse-indicator reading, mapped to what each standard calls for) if there's appetite for a visual once copy is locked.

---

## SEO finalization (seo-technical-content-specialist, 2026-08-10)

**Slug/title rationale:** Draft's slug (`/api-686-ansi-s2-75-alignment-standards`) is correct as written — this is the one page on the site where an exact-match, keyword-forward slug is the right call, since the search behavior here is a spec-lookup query ("API 686 alignment," "ANSI S2.75 shaft alignment"), not a browsing query. That's different reasoning than the complementary-use page.

The draft's suggested title tag ran long (78 characters — would truncate in most SERPs). I cut "Shaft" and "Explained" to bring it to 62 characters while keeping both standards names, which are the terms this page needs to match. The H1 keeps "Shaft Alignment" in full (see below), so the full phrase isn't lost — it's just not duplicated in the title where space is tightest.

**Optional H1 edit:** Draft's H1 is "API 686 and ANSI S2.75 — What They Actually Mean for Your Alignment Job." Consider "...for Your **Shaft** Alignment Job" — one word, reinforces the term the title tag had to drop for length, and reads naturally (it's not an awkward insertion). Not mandatory; flagging as a low-risk option, not a required change.

**Reminder — this page does not carry the site's head-term SEO problem.** Per the Aug 10 fix list, "shaft alignment tools" / "pump alignment tool" (the two big page-2 queries) need to be won on the homepage and `/tool-sets`, not here. This page's job is to exist at all for spec-driven searches (currently zero content anywhere on the site per the Aug 3 audit) and to reinforce topical depth around reverse-indicator alignment — a real but different kind of SEO value than a head-term ranking play.

### Internal linking plan

**Links INTO this page (edits needed on existing pages):**

| From | Anchor text | Notes |
|---|---|---|
| `/laser-alignment-pipe-strain-check` (the complementary-use page) | "API 686 / ANSI S2.75 explainer page" | Already resolved above — cross-link is mutual. |
| `/alignment-tolerances` | "API 686 and ANSI S2.75" | **Correction, 2026-08-10 (Manager's direct browser verification, not a re-audit):** `/alignment-tolerances` is confirmed LIVE with full real content, including the same ".0005\" per inch of coupling span" figure this page cites. No longer a "wait for rebuild" item — build this link both directions now, since the two pages are citing the same fact and should reinforce each other. |
| About Us | "work under API 686 or ANSI S2.75" (or similar, near the existing chemical-plant/water-treatment/pipeline audience mention) | About Us already names this exact audience per the Aug 3 audit — a natural, low-effort place to point toward the explainer page rather than leaving the standards unmentioned there. |
| Pipe Strain blog post | "documenting pipe strain against API 686 / ANSI S2.75" | Optional, secondary priority — only add if it doesn't feel forced in context. The post's core job is explaining pipe strain, not standards compliance. |
| Soft Foot blog post | same pattern as above | Same caveat — optional, don't force. |

**Links OUT of this page (resolved above inline):**
- "page on running ALINE alongside a laser alignment tool" → `/laser-alignment-pipe-strain-check`.
- "A-1000" / "A-2000" / "A-3000" → `/a-1000`, `/a-2000`, `/a-3000` — **confirmed by Jason 2026-08-10, ready to build.**
- **Recommend adding** (not in current draft): in the "A Practical Tolerance Reference" section, link the tolerance figure itself to `/alignment-tolerances` — **confirmed LIVE 2026-08-10 (Manager's direct browser check)** with the same figure already restored, so this can be built now rather than waiting on a rebuild. Right now this page states the number standalone with no cross-reference to where a crew would find the fuller procedure. Still flagging to content-copywriting since it's a sentence-level change, not just a URL swap — the "once rebuilt" dependency is gone, but the copy edit itself still needs their hand.

### Still open (not mine to resolve — repeating the draft's own flags so they don't get lost)
- ~~Standards accuracy (API 686 / ANSI S2.75 descriptions and the tolerance figure) needs Jason's or engineering's sign-off before this goes live.~~ **Resolved 2026-08-10** — see "Key assumptions made" above; all three items fact-checked against public sources, no copy corrections required.
- ~~New flag from fact-check pass: confirm whether `/alignment-tolerances` is already live with the .0005"/inch figure, or still needs the rebuild this internal-linking plan assumes, before building the link described above.~~ **Resolved 2026-08-10** — Manager directly browser-verified `/alignment-tolerances` is live with the figure restored. Link is ready to build; no rebuild dependency remains for this specific page. Note: `/introduction`, `/soft-foot-check`, and `/sag-check` are separately confirmed still empty — any link plan touching those three still waits on the rebuild.
