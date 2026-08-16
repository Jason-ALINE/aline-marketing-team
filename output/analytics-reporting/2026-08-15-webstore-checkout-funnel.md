# Webstore + Amazon Sales — Last 7 Days (Aug 8–14, 2026)

Pulled directly from GA4 (property: ALINE Manufacturing, alinemfg.com) and Amazon Seller Central (A-Line Manufacturing) by the Manager on 2026-08-15, in response to Jason asking what's behind the recent sales increase. Raw data below — not yet a full analysis.

## Top-line ecommerce numbers
- **Revenue:** $6,225.00 (100% ecommerce)
- **Total purchasers:** 2 (both first-time)
- **Items purchased:** 3
- **Avg purchase revenue per active user:** $259.38
- **Items viewed (site-wide):** 69 | **Added to cart:** 6 | **Purchased:** 3

## Product concentration
| Item | Viewed | Added to cart | Purchased | Revenue |
|---|---|---|---|---|
| A-3000 Tool Set | 20 | 5 | 3 | $6,225.00 (100%) |
| A-3000 Tool Set with Indicators | 14 | 1 | 0 | $0 |
| A-1000 Tool Set with Indicators | 10 | 0 | 0 | $0 |
| A-1000 Tool Set | 9 | 0 | 0 | $0 |
| A-750 Tool Set | 5 | 0 | 0 | $0 |
| A-750 Tool Set with Indicators | 5 | 0 | 0 | $0 |
| A-2000 Tool Set | 2 | 0 | 0 | $0 |
| A-2000 Tool Set with Indicators | 2 | 0 | 0 | $0 |

**100% of this week's revenue came from one SKU: A-3000 Tool Set.** No other product converted, despite A-3000 with Indicators pulling nearly as many views (14 vs 20).

## Traffic source breakdown (sessions, last 7 days)
| Channel | Sessions | % of sessions | Key events | Revenue |
|---|---|---|---|---|
| Organic Search | 55 | 51.9% | 0 | $0 |
| **Direct** | **33** | **31.1%** | **2 (100%)** | **$6,225.00 (100%)** |
| Referral | 9 | 8.5% | 0 | $0 |
| Unassigned | 9 | 8.5% | 0 | $0 |

**Both purchases came through Direct traffic.** Organic Search brings in the majority of sessions but converted at 0% this week.

## Amazon — Seller Central Business Reports (A-Line Manufacturing)

Pulled from Business Reports > Sales and Traffic (By Date) and Detail Page Sales and Traffic (By ASIN), both set to the same Aug 8–14 window and cross-checked against the 30-day daily time series (7/14–8/12).

**The entire month is $0 revenue except a single day.** Daily breakdown from 7/14/2026 through 8/11/2026: every day shows $0.00 revenue, 0 units, 0 orders — including all of the Aug 8–14 window except one day. Then:

- **8/12/2026: $5,150.00 revenue, 2 units, 1 order, 1 session, 100% order-item-session conversion.**

That single order is 100% of Amazon's revenue for the week (and for the trailing 30 days). It was for the **Aline A-3000W Reverse Dial Indicator Shaft Alignment Set (with Indicators)** — SKU A-3000W, ASIN B0C2B3XSLC — the "with Indicators" variant. (Notably the *opposite* of the webstore, where the base A-3000 without indicators is what sold and the "with Indicators" variant got views but zero purchases — see product concentration table above. Sample sizes on both sides are too small to call this a real pattern yet.)

No other ASIN in the 8-SKU catalog had any sessions, page views, or orders in this window at all — the "Products with Increasing/Declining Traffic" dashboard cards corroborate this: A-3000 Tool Set and A-3000W both registered as **declining-traffic** ASINs week-over-week (-85.71% and -78.57% sessions respectively) even in the same period this one order landed.

## Known data-quality caveats
1. **Small sample, webstore.** 2 purchasers / 3 units. Do not treat percentages (e.g. "100% of revenue from Direct") as a stable pattern yet — it's 2 data points.
2. **Even smaller sample, Amazon.** 1 order. Not a trend — it's the first sale after roughly a month of zero Amazon sales. Don't build a narrative ("Amazon is picking up") on n=1.
3. **GA4's pre-built "Checkout journey" funnel report is broken for this site.** It expects a standard `add_shipping_info` step name; the site fires a custom `checkout_progress` event instead, so the funnel visualization shows 0% at steps 2–4 even though purchases are completing. Numbers above were pulled from the Ecommerce purchases and Traffic acquisition reports instead, which aren't affected by this mismatch. Someone should either rename the site's event to match GA4's standard funnel step or rebuild the funnel report with the custom event name — flagging as a fix item, not blocking.
4. **`qualify_lead` / `close_convert_lead` key events still have zero data** (see 2026-08-15 update to conversion-funnel-next-steps memory) — this data covers Buy-Now purchases only, not any quote-request or sales-assisted path.
5. **"Direct" traffic is not necessarily brand-new/no-history visitors** — GA4 buckets a session as Direct when it can't attribute a source, which includes typed URLs, bookmark clicks, and untagged links. **Ruled out:** Jason confirmed (2026-08-15) no outreach/email campaign went out this week, so the Direct-traffic concentration isn't an artifact of untagged outreach links. Still unexplained — could be direct URL typing, a bookmark, word-of-mouth, or a referral source GA4 couldn't attribute (e.g. a link from a platform GA4 doesn't parse, like a PDF, text message, or internal company doc).

## Possible next steps
- **analytics-reporting-specialist**: revisit this once another 1–2 weeks of data exists on both channels — right now combined n=3 orders is too thin to set a sales-goal number or call a trend. Ties to the paused sales-goal discussion.
- **content-copywriting-specialist / seo-technical-content-specialist**: worth understanding why A-3000 (not A-3000 with Indicators, despite comparable traffic) is the one converting on the webstore — could be price point, page copy, or the page-thinness issue already flagged for A-1000/A-2000/A-750 in the paused conversion-funnel thread.
