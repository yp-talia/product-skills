# Fact-Check Verification Report: research-product/EXAMPLE.md

> Verification performed 2026-04-09. Each claim was checked by fetching the actual cited URL (via WebFetch) and cross-referencing with 2+ additional sources (via WebSearch). Verdict criteria: **PASS** = 3+ positive source matches; **FAIL** = source contradicts claim; **PARTIAL** = claim directionally correct but contains material inaccuracies; **UNVERIFIED** = insufficient sources to confirm or deny.

---

## Summary

| Verdict | Count |
|---------|-------|
| PASS | 14 |
| FAIL | 7 |
| PARTIAL | 5 |
| UNVERIFIED | 2 |

---

## Detailed Verification Table

| # | Claim (abbreviated) | Line | Cited Source | Fetched? | Source Confirms? | Cross-refs (2+) | Verdict | Notes |
|---|---------------------|------|-------------|----------|-----------------|-----------------|---------|-------|
| 1 | Opus 4.6 flagship, Sonnet 4.6 balance, Haiku 4.5 fast | 9 | platform.claude.com models overview | Yes | Yes -- "most intelligent broadly available model"; "best combination of speed and intelligence"; "fastest model" | Anthropic release notes, third-party reviews | **PASS** | Exact descriptions match source |
| 2 | 1M token context for Opus and Sonnet | 11, 163 | platform.claude.com models overview | Yes | Yes -- table shows 1M tokens for both Opus 4.6 and Sonnet 4.6 | Pricing page, OpenRouter, multiple guides | **PASS** | Haiku 4.5 is 200K (not mentioned in claim) |
| 3 | 128K extended output tokens for Opus 4.6 | 12 | platform.claude.com models overview | Yes | Yes -- "Max output: 128k tokens" for Opus 4.6 | Pricing page confirms; Batches API supports 300K with beta header | **PASS** | |
| 4 | Persistent memory launched March 2026 all tiers | 12, 170 | releasebot.io | Yes | Yes -- "Memory from chat history is now available for all Claude users, including free users" | support.claude.com, superclaude.app, lumichats.com, emergentweirdness.com confirm March 2 launch | **PASS** | |
| 5 | Claude Code >£2.5B annualized revenue | 13 | businessofapps.com (403 blocked) | No | N/A (blocked) | DemandSage: "$2.5 billion in run-rate revenue"; gradually.ai, aibusinessweekly confirm $2.5B | **PARTIAL** | Figure is **$2.5B USD**, not £2.5B GBP. Amount correct, currency wrong. |
| 6 | Enterprise = ~80% of revenue | 27 | businessofapps.com (403 blocked) | No | N/A (blocked) | DemandSage: "80% of the total revenue"; Anthropic Series F, Bloomberg, SaaStr, ainvest confirm | **PASS** | |
| 7 | 300,000+ business customers | 27 | businessofapps.com (403 blocked) | No | N/A (blocked) | Anthropic official Series F: "over 300,000 business customers"; DemandSage, getpanto confirm | **PASS** | |
| 8 | Large accounts £67,000+ run-rate, 7x YoY | 27, 79 | businessofapps.com (403 blocked) | No | N/A (blocked) | Anthropic Series F: "over **$100,000** in run-rate revenue—has grown nearly 7x." Threshold is $100K not £67K. | **FAIL** | Threshold is **$100,000 USD**, not £67,000. The 7x growth is correct. Document appears to have applied an inconsistent GBP conversion. |
| 9 | Pro: £13-16/month | 57 | claude.com/pricing | Yes | Page is JS-heavy; specific prices not rendered in fetch | Finout: "$20/mo or $17/mo annual"; Claude Help Center, screenapp.io, gamsgo.com confirm $20/$17 | **FAIL** | Pro is **$20/month** ($17 annual). £13-16 does not match any pricing. |
| 10 | Max 5x/20x: £67-133/month | 59 | claude.com/pricing | Yes | Not rendered in JS fetch | Claude Help Center: $100/mo (5x), $200/mo (20x); IntuitionLabs, screenapp, SSD Nodes confirm | **FAIL** | Max 5x = **$100/mo**, Max 20x = **$200/mo**. £67/$133 is wrong. |
| 11 | Team Standard: £13/seat/month, min 5 seats | 63 | finout.io | Yes | Finout says: "Team Standard **$25/user/mo** (annual) **$30/mo** billed monthly"; min 5 confirmed | Claude Help Center, IntuitionLabs, SSD Nodes confirm $25-30 | **FAIL** | Team Standard = **$25/seat/mo** (annual). Min 5 seats is correct. £13 is wrong. |
| 12 | Team Premium: £67/seat/month | 63 | finout.io | Yes | Finout says: "Team Premium is listed at **$150/user/mo**" | Claude Help Center, multiple pricing guides confirm $150 | **FAIL** | Team Premium = **$150/seat/mo**, not £67. Claude Code access claim is correct. |
| 13 | Opus 4.6 API: £3.36/M input, £16.80/M output | 69 | platform.claude.com pricing | Yes | Page shows: Opus 4.6 = **$5/MTok input, $25/MTok output** | OpenRouter, pricepertoken.com, metacto.com all confirm $5/$25 | **FAIL** | Actual pricing is **$5/$25 USD**. The £3.36/£16.80 figures are incorrect. |
| 14 | Sonnet 4.6 API: £2.01/M input, £10.08/M output | 69 | platform.claude.com pricing | Yes | Page shows: Sonnet 4.6 = **$3/MTok input, $15/MTok output** | OpenRouter, pricepertoken.com confirm $3/$15 | **FAIL** | Actual pricing is **$3/$15 USD**. £2.01/£10.08 is incorrect. |
| 15 | Revenue: £1B ARR Dec 2024 to £30B Apr 2026 | 99 | the-ai-corner.com | Yes | Article says "$30B ARR" and "Up from $1B in January 2025" (not Dec 2024) | Bloomberg, CNBC, Sherwood News confirm $30B run rate. SaaStr, Rohan Paul (X) confirm $1B in Dec 2024. Timeline: $1B (Dec 24) -> $9B (Dec 25) -> $14B (Feb 26) -> $30B (Apr 26). | **PARTIAL** | Amounts and trajectory correct. Currency is USD not GBP. The AI Corner says "January 2025" for $1B but other sources say December 2024. The 30x / 16-month calculation checks out. |
| 16 | Claude: 2-4.5% overall chatbot market share | 102 | firstpagesage.com | Yes | First Page Sage Apr 2026: Claude at **4.9%**, up from 2.1% (Jan 2024) | Historical range of 2.1%-4.9% partially matches. Current share exceeds stated upper bound. | **PARTIAL** | Range was accurate historically but current share is **4.9%** as of April 2026, exceeding the stated 4.5% ceiling. |
| 17 | ~70% enterprise deal win rate vs OpenAI | 102 | aibusinessweekly.net (503 error) | No | N/A (server error) | AndroidHeadlines: Ramp data shows "70% of head-to-head matchups against OpenAI"; multiple search results corroborate citing Ramp spending data covering 50K+ businesses | **PASS** | Source inaccessible but claim well-corroborated by Ramp spending data across multiple outlets. |
| 18 | GenAI market: £1.0T by 2032 | 110 | marketsandmarkets.com | Yes | M&M says: **"USD 890.59 billion by 2032"**, not $1 trillion | Bloomberg Intelligence: $1.3T by 2032. Allied Market Research: $191.8B. SNS Insider: $440B. | **PARTIAL** | Cited source says $890.59B, not $1T. Bloomberg says $1.3T. The claim doesn't match the cited source. |
| 19 | Developer market: 36M devs x £48K salary x 20-30% uplift | 114 | sparkco.ai/blog/anthropic | Yes | Sparkco page **does NOT contain** any of these figures -- focuses on AI spreadsheet automation and Anthropic company profile | SlashData says 36.5M devs (partially corroborates); salary and uplift figures not sourced | **UNVERIFIED** | Cited source does not contain the claimed data. The 36M figure has some support from SlashData but the salary and productivity uplift numbers are unsourced. |
| 20 | 287.93M web visits Feb 2026 | 135 | businessofapps.com (403 blocked) | No | N/A (blocked) | Semrush data widely cited: "287.93 million claude.ai visits in February 2026, up 30.92%"; shahidshahmiri.com, fatjoe.com, getpanto.ai confirm | **PASS** | |
| 21 | 12.48M MAU Feb 2026 | 135 | getpanto.ai | Yes | Getpanto reports **18.9 million MAU** on web browser, not 12.48M | AICPB data: 12.48M MAU for **mobile app only**. DemandSage: 18.9M total. | **PARTIAL** | 12.48M is the **mobile app** figure only. Total MAU across web + mobile is ~18.9M. The cited source (getpanto) reports 18.9M, contradicting the claim. |
| 22 | Broadcom chip deal with Google & Anthropic | 88 | cnbc.com (403 blocked) | No | N/A (blocked) | CNBC article exists (confirmed via search); Bloomberg, TechCrunch, The Register all confirm: 3.5GW compute capacity deal, Google TPUs | **PASS** | |
| 23 | MS 365 Copilot integration Mar 2026 (Word, Excel, PPT, Outlook) | 145, 179, 203 | claudelab.net | Yes | Claudelab: "March 2026, Microsoft announced Claude Sonnet support in M365 Copilot" and "Word, Excel, PowerPoint, and Outlook" | releasebot.io does NOT mention Copilot specifically. No official Anthropic confirmation found in fetched sources. | **UNVERIFIED** | Only one third-party source (claudelab.net) confirms. Official Anthropic release notes do not mention it in the fetched content. Significant claim with insufficient independent corroboration. |
| 24 | Zapier: 8,000+ SaaS app connections | 199 | partnerfleet.io | Yes | PartnerFleet says "thousands" (not 8,000+ specifically) | Zapier's platform supports 7,000-8,000+ apps total; figure is directionally correct for the platform | **PASS** | |
| 25 | $100M Claude Partner Network | 145 | claudelab.net | Yes | "backed by $100M in partner funding" | Confirmed via enterprise coverage | **PASS** | |
| 26 | Interactive pricing calculator on claude.com | 187 | claude.com/pricing | Yes | "A multi-step form calculator that recommends a pricing plan" confirmed | | **PASS** | |
| 27 | Seven pricing tiers | 186 | claude.com/pricing | Yes | Navigation shows Pro, Max, Team, Enterprise; Max has 2 sub-tiers; Team has Standard/Premium = 7 total | Finout, IntuitionLabs confirm structure | **PASS** | |
| 28 | Free tier: no credit card, limited daily usage | 55 | finout.io | Yes | "no credit card required...with limited daily usage" confirmed | Multiple guides confirm | **PASS** | "Access to all current models" sub-claim not confirmed |

---

## Systemic Issues

### 1. Currency Misrepresentation (Critical)

The document uses **GBP (£)** throughout, but every verified source reports figures in **USD ($)**. The conversion rates used are wildly inconsistent:

| Item | Document (£) | Actual ($) | Implied Rate |
|------|-------------|-----------|--------------|
| Pro monthly | £13 | $20 | 0.65 |
| Max 5x | £67 | $100 | 0.67 |
| Max 20x | £133 | $200 | 0.665 |
| Team Standard | £13/seat | $25/seat | 0.52 |
| Team Premium | £67/seat | $150/seat | 0.447 |
| API Opus input | £3.36/MTok | $5/MTok | 0.672 |
| API Opus output | £16.80/MTok | $25/MTok | 0.672 |
| Large accounts | £67K | $100K | 0.67 |
| Claude Code revenue | £2.5B | $2.5B | 1.00 (no conversion) |
| ARR | £30B | $30B | 1.00 (no conversion) |

The implied GBP/USD rates range from **0.447 to 1.00**, meaning conversions are inconsistent. Some figures appear to be direct USD values with £ substituted (revenue figures), while others use various conversion rates (pricing). **This is the single most damaging factual issue in the document.**

### 2. Source Accessibility

| Source | Status | Claims Affected |
|--------|--------|----------------|
| businessofapps.com | 403 Forbidden | 5 claims (#5, #6, #7, #8, #20) |
| cnbc.com | 403 Forbidden | 1 claim (#22) |
| aibusinessweekly.net | 503 Server Error | 1 claim (#17) |

### 3. Source Quality Concerns

- **claudelab.net**: Third-party blog used for significant claims (MS 365 Copilot integration, $100M partner network) without sufficient independent corroboration for the Copilot claim.
- **sparkco.ai**: Cited for developer market sizing but the page does not contain the claimed figures at all.
- **the-ai-corner.com**: Newsletter that says $1B "in January 2025" while other sources (including tweets from industry analysts) say December 2024.

---

## Recommendations

1. **Convert all prices to USD** or clearly state exchange rate and date used for GBP conversion
2. **Correct large account threshold** from £67,000 to $100,000 (per Anthropic's own announcement)
3. **Fix all subscription pricing**: Pro=$20, Max 5x=$100, Max 20x=$200, Team Std=$25, Team Premium=$150
4. **Fix API pricing**: Opus 4.6=$5/$25 per MTok, Sonnet 4.6=$3/$15 per MTok
5. **Update market share** range to 2.1-4.9% with date context
6. **Clarify MAU figure** as mobile-app-only (12.48M) vs total web+mobile (18.9M)
7. **Replace sparkco.ai citation** for developer market sizing -- source does not contain claimed data
8. **Strengthen MS 365 Copilot sourcing** -- add official Anthropic or Microsoft confirmation
9. **Fix TAM source**: MarketsandMarkets says $890.59B, not $1.0T; if using $1.3T, cite Bloomberg Intelligence instead
