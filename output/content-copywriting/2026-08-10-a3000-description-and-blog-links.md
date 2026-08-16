# A-3000 Product Description Expansion + Blog Post Link Fixes
**Date:** 2026-08-10
**Source tasks:** Master website improvement list (`output/seo-technical-content/2026-08-10-master-website-improvement-list.md`), Tier 2 items 5 and 7.
**Scope:** Draft-and-hold. No Wix publish access — someone with Wix editor access executes both pieces below.

---

## Task 1 — `/a-3000` product description (ready to copy-paste)

**Context:** This is the site's best-converting product page (9.5% CTR vs. site average, per Search Console data) with the thinnest copy on the site. Current live body copy:

> "This is the Combination Set. Features both the A-2000 and A-1000 in the same case. This is our most popular set because it fits most everything from 1" to 10". Great for field servicemen."

**Proposed replacement:**

> This is the Combination Set. It features both the A-2000 and A-1000 in the same case — everything you need to cover shafts from 1" to 10" — which is why it's our most popular set. One case, almost every job.
>
> Like every ALINE set, the A-3000 uses the reverse-indicator method: no batteries, no calibration, nothing to charge or reset between jobs. Set the brackets, turn the shafts, read the dials.
>
> Each set ships with Starrett 196B1 dial indicators, accurate to .001" — tight enough for the tolerances referenced in API 686 and ANSI S2.75, the standards most plants and contract alignment jobs are already specifying work to.
>
> Any millwright can learn the procedure in a single shift. Great for field servicemen and crews who need one case that handles almost everything that comes through the shop or out to the field.

**Notes on what's reused vs. new:**
- "Combination Set... A-2000 and A-1000... 1" to 10"... most popular... Great for field servicemen" — kept from the existing copy, lightly tightened, not replaced.
- "No batteries, no calibration" and "any millwright can learn the procedure in a single shift" — pulled from language already proven live elsewhere on the site (homepage: "Any millwright can learn the graphical procedure in a single shift," per the Aug 3 audit's verbatim capture) rather than invented fresh.
- ".001" accuracy" and "Starrett 196B1" — pulled directly from `company-brief.md`'s verified product specs (confirmed by Jason, 2026-08-10). Deliberately did **not** use the .0005"/inch-of-coupling-span figure here — that's a separate alignment-tolerance rule of thumb, not the tool's own accuracy, and the brief is explicit these shouldn't be conflated.
- API 686 / ANSI S2.75 — included as the standards-reference hook per company-brief positioning guidance, phrased as "referenced" / "specifying work to" rather than claiming ALINE tools are certified/compliant to either standard, since no certification claim is sourced anywhere in the brief or on the site.
- No pricing, no new specs beyond what's listed above — nothing here isn't traceable to the current live copy or `company-brief.md`.

**Not included in this draft (already owned by SEO, don't duplicate):** title tag, alt text — those are scoped separately in `seo-technical-content-specialist`'s Tier 3 quick-wins draft and shouldn't be touched as part of this body-copy edit.

---

## Task 2 — `/post/shaft-runout-deflection-and-whip` — link fixes (instructions, not verified live wording)

**I do not have live access to this post's current rendered content** (Wix JS rendering blocks the fetch tools available to me, consistent with what the rest of the team has hit today). Everything below is a set of precise instructions for whoever has Wix editor access to execute — not guessed exact wording pulled from a page I can't see. Please sanity-check exact phrasing against the live post before publishing any of this.

What I do know, second-hand from the SEO audits: the post has clean H2 structure (something like "What Causes Pipe Strain / Runout" → "What It Does to Your Equipment" → "Preventing..." → "Identifying..." → "Key Takeaways" pattern, per the Aug 3 audit) and an existing but unlinked CTA phrase: **"Upgrade to ALINE alignment tools."** Zero outbound links currently. 54 clicks / 5,956 impressions — this is the strongest non-homepage page on the site, so this is worth doing carefully rather than fast.

### Link additions — what to add, where, why

| # | Add this link | Suggested anchor text (verify against actual post wording before using) | Where to place it | Why this link |
|---|---|---|---|---|
| 1 | `/a-3000` | "ALINE's A-3000 combination set" (or whatever the post's existing phrase for "our tools" is, if one exists) | Wherever the post currently mentions correcting or checking for runout/whip with a tool — likely in the "Preventing" or "Identifying" H2 section. If no natural sentence exists, add one short sentence at the end of that section, e.g.: "A reverse-indicator set like the A-3000 gets you real dial readings on shaft position through a full rotation — no guesswork." | A-3000 covers the widest shaft range (1"–10") of any ALINE set, so it's the safest single-product link for a post that isn't scoped to one specific shaft size. If the post's actual content leans toward a smaller/larger shaft range specifically, swap for A-1000 or A-2000 instead — flag back to me if so. |
2 | Hyperlink the existing **"Upgrade to ALINE alignment tools"** CTA | (use the exact existing phrase — just add the link, don't reword it) | Wherever it currently sits (sounds like a closing CTA near "Key Takeaways") | This is bare text right now — it's the post's own call to action and currently goes nowhere. Point it at `/shop` if it's meant as a general upgrade prompt, or `/a-3000` if it's meant to point at one specific product — since #1 above is already sending readers to A-3000 mid-post, pointing this closing CTA at `/shop` avoids repeating the same link twice and gives a browsing option instead. |
| 3 | `/laser-alignment-pipe-strain-check` (published-ready per today's earlier SEO/content work) | "if you're already running a laser system" or similar, adapted to actual post wording | In the "Preventing" or "What It Does to Your Equipment" section, wherever the post discusses causes/detection methods | Strong natural fit: runout is one of the four things company-brief.md explicitly lists as what laser alignment tools *don't* fully cover (pipe strain, soft foot, runout, bearing clearance). A post about shaft runout is a natural bridge into the complementary-use pitch — "your laser handles alignment, an ALINE tool catches what it doesn't." |
| 4 | `/alignment-tolerances` (confirmed live with real content as of today) | "shaft alignment tolerances" or similar | Wherever the post references acceptable runout/deflection thresholds, if it does | Optional but worth it if the post references any tolerance figures — gives readers a next-step page with the real ".0005\"/inch of coupling span" guideline instead of a dead end. Skip if the post doesn't naturally reference tolerances anywhere. |

**Do not add** a link to `/soft-foot-check` or `/sag-check` yet — both are still empty pages per the master list's Tier 0 item 1 (not yet rebuilt). Once those are live, they're a strong candidate for a future pass on this same post (sag can cause false runout readings), but don't link to an empty page now.

**Body copy/voice:** leave untouched. This is link scaffolding only, per the master list's own scoping — don't rewrite sentences beyond what's needed to add the links above.

### Meta description

I don't have live access to confirm whether one currently exists. Draft below, to be used **only if live verification confirms one is missing or is generic/weak** — don't overwrite something that's already doing its job:

> **Shaft runout and whip signal real alignment problems — learn what causes them, what they do to your equipment, and how reverse-indicator alignment catches what other methods miss.**

~155 characters. Uses "reverse-indicator alignment" (core positioning term) and implies the complementary-use angle without overclaiming. Flagging explicitly: **needs a live verification pass** by whoever has Wix access before either confirming the existing one is fine or publishing this replacement.

---

## Key assumptions made

1. Assumed the post's actual content matches the H2 pattern described secondhand in the Aug 3 SEO audit (I have not read the live post directly) — if the real structure or content differs meaningfully, the placement guidance above may need adjusting on the fly by whoever has Wix access.
2. Assumed A-3000 is the right single product link given its 1"–10" range covers the broadest set of "runout" scenarios; flagged as swappable if the post's actual content is scoped to a narrower shaft size.
3. Did not fabricate any exact quote from the live blog post — all anchor text above is suggested/adaptable, not a claim about the post's literal current wording.
4. A-3000 description reuses only language already confirmed live elsewhere on the site (homepage's millwright/single-shift phrasing per the Aug 3 audit's verbatim capture) or in `company-brief.md`'s verified specs — no new stats, pricing, or claims invented.
5. Did not claim ALINE tools are "certified" or "compliant" to API 686/ANSI S2.75 — the brief documents these as reference standards/credibility hooks, not a certification claim, so the A-3000 copy stays at "tight enough for the tolerances referenced in" rather than asserting compliance.

## Next specialist

- **seo-technical-content-specialist** (or whoever has Wix editor access, per the master list's draft-and-hold pattern) — to execute the link additions and meta description on the blog post, and to confirm/paste the A-3000 body copy live. Also the right party to verify the post's actual H2 structure and existing CTA wording against the instructions above before publishing.
- **design-visual-specialist** — not needed for either piece here (copy-only changes to an existing page template).
- Once both are live, **analytics-reporting-specialist** is a natural follow-up in a few weeks to check whether the A-3000 conversion rate moved and whether the runout post's exit rate/next-page behavior improved (GA4 just went live today per the Aug 10 fix list, so behavioral data should start accumulating).
