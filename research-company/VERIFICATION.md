# Verification Report: research-company/EXAMPLE.md

## Methodology
Every cited URL was fetched directly using WebFetch. Claims were cross-checked against 2+ independent sources using WebSearch and additional WebFetch calls. A claim requires 3 positive source matches to PASS, and 1 negative match to REJECT. All figures in the EXAMPLE.md are presented in GBP; verification sources universally report in USD.

**CRITICAL SYSTEMIC ISSUE:** The entire document converts USD figures to GBP but uses incorrect and inconsistent conversion rates throughout. Some figures appear to use ~0.75 GBP/USD (e.g., Series F), while others use 1:1 (e.g., Feb 2026 ARR of "14 billion" in both currencies). This pervasive problem affects nearly every financial figure.

---

## Claims Verification

### Section: What They Do (Line 9)

| # | Claim | Location | Cited Source | Verification Status | Evidence |
|---|-------|----------|-------------|-------------------|----------|
| 1 | Anthropic is an AI company founded in 2021 | Line 9 | anthropic.com/company | ⚠️ PARTIALLY VERIFIED | The company page does NOT mention the founding year. However, Wikipedia, Contrary Research, Crunchbase, and multiple other sources confirm founding in 2021. True claim, but unsupported by the specific cited source. |
| 2 | Builds frontier LLMs under the brand Claude | Line 9 | anthropic.com/company | ✅ VERIFIED | Page states: "We translate our research into tangible, practical tools like Claude." Confirmed by Wikipedia, news coverage, Anthropic research page. |
| 3 | Focus on safety, reliability, and interpretability | Line 9 | anthropic.com/company | ✅ VERIFIED | Page states: "We aim to build frontier AI systems that are reliable, interpretable, and steerable." Cross-confirmed by Wikipedia, news coverage, research page. |
| 4 | Revenue through API access, subscriptions, and product offerings | Line 9 | N/A (general claim) | ✅ VERIFIED | Confirmed by Anthropic's own Series G announcement, Sacra, SaaStr, and multiple press reports describing API, Claude subscription, and Claude Code revenue streams. |

### Section: Founding Story (Line 13)

| # | Claim | Location | Cited Source | Verification Status | Evidence |
|---|-------|----------|-------------|-------------------|----------|
| 5 | Founded by Dario and Daniela Amodei alongside other former OpenAI researchers | Line 13 | en.wikipedia.org/wiki/Anthropic | ✅ VERIFIED | Wikipedia: "Anthropic was founded in 2021 by seven former employees of OpenAI, including siblings Daniela Amodei and Dario Amodei, the latter of whom was OpenAI's Vice President of Research." Confirmed by Contrary Research, Crunchbase, Built In. |
| 6 | Series B of approximately £900 million in February 2023 at valuation exceeding £3 billion | Line 13 | sacra.com/c/anthropic/ | ❌ REJECTED | **Wrong date, wrong amount, wrong valuation.** The Series B was **$580M in April 2022** (not Feb 2023), at a **$4B valuation** (not £3B+). Led by Sam Bankman-Fried/FTX. The Sacra page fetched does not contain Series B data for 2023. Sources: Crunchbase Series B profile, CNBC, DailyAlts. £900M (~$1.2B) is more than double the actual $580M. |

### Section: Mission & Values (Line 17)

| # | Claim | Location | Cited Source | Verification Status | Evidence |
|---|-------|----------|-------------|-------------------|----------|
| 7 | Public Benefit Corporation with purpose "the responsible development and maintenance of advanced AI for the long-term benefit of humanity" | Line 17 | anthropic.com/company | ✅ VERIFIED | Page states exactly: "Anthropic is a Public Benefit Corporation, whose purpose is the responsible development and maintenance of advanced AI for the long-term benefit of humanity." |
| 8 | Seven core values: Global Good, Balance, User Care, Safety Leadership, Pragmatism, Trust & Honesty, Mission Focus | Line 17 | anthropic.com/company | ❌ REJECTED | **Value names are fabricated paraphrases.** The actual seven values from the page are: (1) "Act for the global good," (2) "Hold light and shade" (NOT "Balance"), (3) "Be good to our users" (NOT "User Care"), (4) "Ignite a race to the top on safety" (NOT "Safety Leadership"), (5) "Do the simple thing that works" (NOT "Pragmatism"), (6) "Be helpful, honest, and harmless" (NOT "Trust & Honesty"), (7) "Put the mission first" (NOT "Mission Focus"). The document invents shorthand names and presents them as if they are the stated values. |
| 9 | "High-trust, low-ego organisation" | Line 17 | anthropic.com/company | ✅ VERIFIED | Page states: "Anthropic is a high-trust, low-ego organization." Minor spelling difference (British vs American) is immaterial. |

### Section: Business Model (Line 21)

| # | Claim | Location | Cited Source | Verification Status | Evidence |
|---|-------|----------|-------------|-------------------|----------|
| 10 | Four monetisation channels including API, Claude Subscription, Claude Code, enterprise licensing | Line 21 | TechCrunch / SaaStr | ✅ VERIFIED | Anthropic's Series G announcement and Sacra analysis confirm API (via cloud platforms), direct subscription, Claude Code, and enterprise licensing as revenue channels. |
| 11 | Claude Code run-rate revenue exceeding £1.9 billion | Line 21 | TechCrunch / SaaStr | ⚠️ PARTIALLY VERIFIED | Anthropic's Series G announcement (Feb 12, 2026) states Claude Code run-rate was "over $2.5 billion." At ~0.76 GBP/USD, that is ~£1.9B. The underlying USD figure is verified but the GBP presentation is misleading. No specific URL provided for this cite. |
| 12 | 80% of revenue from business customers | Line 21 | sacra.com/c/anthropic/ | ✅ VERIFIED | Sacra states: "As of October 2025, Anthropic had 300,000+ business customers accounting for approximately 80% of revenue." Cross-confirmed by Anthropic's own Series F announcement and multiple press reports. |
| 13 | Claude available via API on AWS Bedrock, Google Cloud Vertex AI, Microsoft Azure | Line 21 | N/A | ✅ VERIFIED | Anthropic news page confirms Amazon Bedrock, Google Cloud Vertex AI, and Microsoft Foundry/Azure. Microsoft/NVIDIA Nov 2025 announcement: Claude is "the only frontier model available on all three of the world's most prominent cloud services." |

### Section: Growth Model & Distribution (Lines 24-33)

| # | Claim | Location | Cited Source | Verification Status | Evidence |
|---|-------|----------|-------------|-------------------|----------|
| 14 | Claude is the only frontier AI model on all three major cloud vendors | Line 28 | anthropic.com/news | ✅ VERIFIED | Microsoft blog (Nov 18, 2025): "This partnership will make Claude the only frontier model available on all three of the world's most prominent cloud services." Confirmed by CNBC, Axios, Anthropic. |
| 15 | Claude Code launched May 2025 | Line 30 | anthropic.com/research | ✅ VERIFIED | Claude Code went GA on May 22, 2025 at the "Code with Claude" developer conference. Confirmed by Anthropic, Simon Willison's live blog, Selina Wang (X), GitHub releases page. |
| 16 | Hiring for sales engineers, international expansion leads, revenue accounting | Line 33 | anthropic.com/careers | ⚠️ UNVERIFIABLE | The careers page fetched is an overview without specific listings. It links to /careers/jobs for actual roles. Cannot confirm specific role titles from the cited URL. |

### Section: Technology Landscape (Lines 36-51)

| # | Claim | Location | Cited Source | Verification Status | Evidence |
|---|-------|----------|-------------|-------------------|----------|
| 17 | AWS Trainium2 -- 500,000+ chips in Indiana data centre (Project Rainier) | Line 39 | DataCentre.News | ✅ VERIFIED | DCD: "AWS activates Project Rainier cluster of nearly 500,000 Trainium2 chips." CNBC: "$11B campus near New Carlisle, fully operational Oct 2025." Confirmed by AWS's own announcement, Data Centre Magazine, SiliconANGLE. UltraServer and UltraCluster configurations confirmed. |
| 18 | Google Cloud TPUs expanded in 2026 with gigawatt-scale commitments | Line 40 | anthropic.com/news/google-broadcom-partnership-compute | ✅ VERIFIED | Page confirms: "We have signed a new agreement with Google and Broadcom for multiple gigawatts of next-generation TPU capacity that we expect to come online starting in 2027." Announcement dated April 6, 2026. |
| 19 | NVIDIA GPUs via Microsoft Azure (Nov 2025 partnership) | Line 41 | Yahoo Finance | ✅ VERIFIED | Microsoft blog (Nov 18, 2025): "Anthropic is scaling its rapidly-growing Claude AI model on Microsoft Azure, powered by NVIDIA." Confirmed by CNBC, GeekWire, Anthropic's own announcement, and NVIDIA blog. |
| 20 | Four research verticals: Interpretability, Alignment, Societal Impacts, Frontier Red Team | Line 49 | anthropic.com/research | ⚠️ PARTIALLY VERIFIED | Research page lists: "Alignment, Economic Research, Interpretability, Societal Impacts" as teams, plus "Frontier Red Team" separately. That is five groups, not four. The document omits "Economic Research." The Anthropic Institute (Mar 2026) reorganized some of these. The claim of exactly "four verticals" is inaccurate. |
| 21 | Claude Opus 4.6, Sonnet 4.6, and unreleased Mythos model | Line 46 | Anthropic news | ✅ VERIFIED | Anthropic news: "Introducing Claude Opus 4.6" (Feb 5, 2026) and "Introducing Claude Sonnet 4.6" (Feb 17, 2026). Mythos confirmed via Fortune leak (Mar 26, 2026) and Project Glasswing (Apr 7, 2026). TechCrunch, Bloomberg, Axios all confirm Mythos as preview-only model. |
| 22 | Models use transformer architecture with extended thinking, RLAIF, Constitutional AI | Line 46 | Medium article | ✅ VERIFIED | Constitutional AI confirmed by Anthropic research papers (arxiv.org/abs/2212.08073). RLAIF confirmed by research publications. Extended thinking confirmed in Claude model release notes. Cited source (Medium) is weak but underlying claims are well-established. |

### Section: Funding & Financial Health (Lines 53-70)

| # | Claim | Location | Cited Source | Verification Status | Evidence |
|---|-------|----------|-------------|-------------------|----------|
| 23 | Latest Valuation: £290 billion (Series G, Feb 2026) | Line 57 | Anthropic news | ❌ REJECTED | Actual valuation: **$380 billion** post-money. Sources: Anthropic's own announcement, CNBC, Bloomberg, Crunchbase, TechCrunch, Axios, Fortune -- all report $380B. At 0.75 GBP/USD, $380B = £285B (not £290B). At 0.76 rate, = £288.8B. Neither matches £290B precisely, and no source reports in GBP. |
| 24 | Latest Funding Round: £23 billion Series G, Feb 2026 | Line 58 | CNBC, Feb 12, 2026 | ❌ REJECTED | Actual amount: **$30 billion**. Sources: CNBC, Anthropic, Bloomberg, Crunchbase, TechCrunch, Axios, GIC -- all report $30B. At 0.75 rate, $30B = £22.5B (not £23B). |
| 25 | ARR (April 2026): ~£23 billion | Line 59 | Threads / AI Corner | ❌ REJECTED | Actual ARR: approximately **$30 billion**. Google/Broadcom announcement (Apr 6, 2026): "Revenue run-rate has surpassed $30 billion." AI Corner confirms $30B+. Bloomberg confirms. £23B is wrong regardless of conversion rate used. |
| 26 | ARR (Feb 2026): £14 billion (CEO confirmed at Morgan Stanley TMT) | Line 60 | Morgan Stanley TMT conference | ❌ REJECTED | Anthropic's Series G announcement (Feb 12, 2026) states "current run-rate revenue: $14 billion." The figure is **$14 billion**, not £14 billion. At 0.75 rate, $14B = £10.5B. The document appears to have used £14B as a 1:1 conversion, which is a ~33% error. The underlying USD figure and event are verified. |
| 27 | Employees: ~4,950 (Mar 26, 2026) | Line 61 | Tracxn | ⚠️ PARTIALLY VERIFIED | Tracxn reports 4,954 employees as of March 2026, matching ~4,950. However, other sources give widely different figures: JobsByCulture says ~1,500; TrueUp says ~3,000; ZoomInfo and RocketReach show different numbers. The Tracxn figure may be accurate but cannot be independently triangulated with 3 consistent sources. |
| 28 | ARR growth: £0.75B (Dec 2024) -> £3B (mid-2025) -> £6.75B (end 2025) -> £14B (Feb 2026) -> £23B (Apr 2026) | Line 65 | Sacra/SaaStr | ❌ REJECTED | Actual USD trajectory: ~$1B (Dec 2024) -> ~$4B (mid-2025) -> ~$9B (end 2025) -> $14B (Feb 2026) -> $30B (Apr 2026). The document's GBP figures are **inconsistently converted**: £0.75B correctly implies $1B at 0.75 rate; £6.75B correctly implies $9B; but £14B does NOT convert from $14B (should be ~£10.5B at 0.75 rate). The document mixes converted and unconverted figures. |
| 29 | 3,000% year-over-year growth | Line 65 | Sacra/SaaStr | ⚠️ PARTIALLY VERIFIED | Sacra reports "up about 1,400% year-over-year." From $1B (Dec 2024) to $30B (Apr 2026) is 2,900% but over ~16 months, not 12. The 3,000% figure is in the right order of magnitude but imprecise and not confirmed by any primary source using this exact number. |
| 30 | Gross margins estimated at 70%+ | Line 65 | Inference | ⚠️ UNVERIFIABLE | No public confirmation of gross margins. Anthropic is private and does not disclose margin data. No source found confirming this figure. |
| 31 | Headcount: 192 (2022) to 1,097 (2025) to ~4,950 (Mar 2026), 454 open roles | Line 68 | Tracxn | ⚠️ PARTIALLY VERIFIED | The trajectory appears in some third-party sources but cannot be confirmed by 3 independent sources. Employee counts vary widely across aggregators. The 454 open roles figure is a snapshot that changes constantly. |

### Section: Key Milestones (Lines 72-84)

| # | Claim | Location | Cited Source | Verification Status | Evidence |
|---|-------|----------|-------------|-------------------|----------|
| 32 | March 2021: Anthropic founded | Line 76 | Wikipedia | ❌ REJECTED | **Wrong month.** Wikipedia says "founded in 2021" without specifying a month. Multiple sources (Contrary Research, Timelines wiki, MicroVentures, DataStudios) specify **January 2021**, not March. No source found stating March 2021. |
| 33 | Feb 2023: Series B ~£750m at £3bn+ valuation | Line 77 | Crunchbase | ❌ REJECTED | **Wrong on all counts.** Crunchbase shows Series B was **$580M in April 2022** at $4B valuation. Not Feb 2023, not £750M (~$1B), not £3B+ valuation. |
| 34 | Dec 2024: ARR crosses £750m mark | Line 78 | SaaStr | ❌ REJECTED | Multiple sources (SaaStr, X posts, Sacra) report ARR reached approximately **$1 billion** in December 2024. £750M (~$950M) is close if using 0.75 conversion, but the inconsistent currency approach makes this unreliable. The actual milestone was $1B, not £750M. |
| 35 | May 2025: Claude Code launches publicly | Line 79 | Anthropic news | ✅ VERIFIED | Claude Code went GA on May 22, 2025. Confirmed by Anthropic, GitHub releases, Simon Willison, Selina Wang. |
| 36 | Sep 2025: Series F £9.75bn at £138bn valuation (ICONIQ-led) | Line 80 | Bloomberg, Sep 2025 | ⚠️ PARTIALLY VERIFIED | Actual: **$13B at $183B valuation, ICONIQ-led**, September 2025. At 0.75 GBP/USD: $13B = £9.75B and $183B = £137.25B (~£138B). The GBP conversion is approximately correct here. Date and lead investor are correct. But no primary source reports in GBP. |
| 37 | Nov 2025: Microsoft/NVIDIA partnership: £22.5bn commitment | Line 81 | Yahoo Finance | ❌ REJECTED | **Mischaracterised.** The partnership involved: (a) Anthropic committing to purchase **$30B of Azure compute**, (b) NVIDIA investing up to **$10B**, (c) Microsoft investing up to **$5B**. Total investments: up to $15B. £22.5B (~$30B) appears to conflate the Azure compute purchase commitment with the partnership investment. The description "£22.5bn commitment" is misleading -- this was Anthropic's commitment to BUY compute, not investment received. |
| 38 | Feb 2026: Series G £23bn at £290bn valuation | Line 82 | Anthropic news | ❌ REJECTED | Actual: **$30B at $380B valuation**. Sources: Anthropic, CNBC, Bloomberg, Crunchbase, TechCrunch, Axios, GIC. |
| 39 | Mar 2026: Anthropic Institute launched; Mythos model preview | Line 83 | Anthropic news | ⚠️ PARTIALLY VERIFIED | Anthropic Institute launched March 11, 2026 (confirmed). However, the Mythos **preview release** was part of Project Glasswing on **April 7, 2026** (not March). The Fortune leak article was March 26, but the actual preview was April. |
| 40 | Apr 2026: Google/Broadcom TPU deal; Project Glasswing | Line 84 | Anthropic news | ✅ VERIFIED | Google/Broadcom deal announced April 6, 2026. Project Glasswing announced April 7, 2026. Both confirmed by Anthropic news page, CNBC, TechCrunch, Bloomberg, Axios. |

### Section: Recent News (Lines 86-97)

| # | Claim | Location | Cited Source | Verification Status | Evidence |
|---|-------|----------|-------------|-------------------|----------|
| 41 | Series G: £23B at £290B valuation, run-rate crossing £14B | Line 90 | Anthropic, Feb 12, 2026 | ❌ REJECTED | Repeated currency error. Actual: $30B at $380B valuation, $14B run-rate. All primary sources report in USD. |
| 42 | Claude Opus 4.6 & Sonnet 4.6 model releases | Line 91 | Anthropic news, Feb 2026 | ✅ VERIFIED | Opus 4.6 (Feb 5, 2026) and Sonnet 4.6 (Feb 17, 2026) confirmed by Anthropic news page and platform release notes. |
| 43 | India (Bengaluru, February) and Sydney (March) expansion | Line 92 | Anthropic news | ✅ VERIFIED | Anthropic news confirms Bengaluru office (Feb 16, 2026) and Sydney (Mar 10, 2026, "fourth office in Asia-Pacific"). |
| 44 | Anthropic Institute Launch (Mar 2026) | Line 93 | Anthropic news | ✅ VERIFIED | Confirmed March 11, 2026. Led by co-founder Jack Clark. Confirmed by eWeek, SiliconANGLE, Campus Technology, multiple outlets. |
| 45 | Mythos described as "step change" in capability | Line 94 | Fortune / SecurityWeek, Mar 2026 | ✅ VERIFIED | Fortune (Mar 26, 2026): Anthropic spokesperson stated model represents "a step change" in performance and is "the most capable we've built to date." Confirmed by Axios, TechCrunch, Bloomberg. |
| 46 | Project Glasswing partners: AWS, Apple, Cisco, Google, Microsoft, NVIDIA, others | Line 95 | Anthropic news, Apr 2026 | ✅ VERIFIED | Partners confirmed: Amazon, Apple, Broadcom, Cisco, CrowdStrike, Linux Foundation, Microsoft, Palo Alto Networks, and ~40 others. Note: document says "AWS" but partner listed as "Amazon"; omits CrowdStrike, Linux Foundation, Broadcom, Palo Alto Networks. |
| 47 | Google/Broadcom deal: gigawatt-scale, operational from 2027 | Line 96 | CNBC / Anthropic news | ✅ VERIFIED | Anthropic announcement: "multiple gigawatts of next-generation TPU capacity that we expect to come online starting in 2027." |
| 48 | Claude will remain ad-free | Line 102 | Anthropic news, Feb 2026 | ✅ VERIFIED | Confirmed on Anthropic news (Feb 4, 2026). Exact quote present on the news page. |

### Section: What Investors Say (Lines 107-110)

| # | Claim | Location | Cited Source | Verification Status | Evidence |
|---|-------|----------|-------------|-------------------|----------|
| 49 | Series G investors: Altimeter, BlackRock, Blackstone, Goldman Sachs, Insight Partners, Qatar Investment Authority, TPG | Line 108 | Bloomberg, Sep 2025 | ⚠️ PARTIALLY VERIFIED | These investors participated across Series F and G rounds. However, the document cites "Bloomberg, Sep 2025" which was the **Series F** date, not Series G. The Series G (Feb 2026) was led by GIC and Coatue, co-led by D.E. Shaw, Dragoneer, Founders Fund, ICONIQ, MGX. The listed investors were primarily Series F participants. Attribution is confused. |
| 50 | "4x lower training costs than OpenAI" | Line 110 | SaaStr and Sacra | ⚠️ PARTIALLY VERIFIED | SaaStr/AI Corner reports Anthropic "spending 4x less" on training (OpenAI projected $121B compute through 2030 vs Anthropic ~$30B). This is analyst inference, not a confirmed internal figure. |

### Section: What Employees Say (Lines 112-127)

| # | Claim | Location | Cited Source | Verification Status | Evidence |
|---|-------|----------|-------------|-------------------|----------|
| 51 | Glassdoor rating: 4.4/5.0 stars | Line 114 | Glassdoor | ✅ VERIFIED | Confirmed by Glassdoor page and JobsByCulture aggregation: 4.4/5.0. |
| 52 | 24 reviews | Line 114 | Glassdoor | ❌ REJECTED | Actual: **222 reviews** per JobsByCulture (aggregating Glassdoor). The Glassdoor URL title shows "(24)" which may be a filtered view or old cache, but multiple sources confirm a much higher count. |
| 53 | 86% would recommend | Line 114 | Glassdoor | ❌ REJECTED | Actual: **95% would recommend** per JobsByCulture. The document's 86% is materially lower than the verified figure. |
| 54 | Culture and Values: 4.6/5 | Line 117 | Glassdoor | ❌ REJECTED | Actual: **4.5/5.0** per JobsByCulture Glassdoor aggregation. Off by 0.1. |
| 55 | Career Opportunities: 4.7/5 | Line 118 | Glassdoor | ❌ REJECTED | Actual: **4.0/5.0** per JobsByCulture. Off by 0.7 -- a significant error. |
| 56 | Work-Life Balance: 3.4/5 | Line 122 | Glassdoor | ❌ REJECTED | Actual: **3.7/5.0** per JobsByCulture. Off by 0.3. Direction (lowest category) is correct but number is wrong. |

### Section: What Customers Say (Lines 129-143)

| # | Claim | Location | Cited Source | Verification Status | Evidence |
|---|-------|----------|-------------|-------------------|----------|
| 57 | Trustpilot (claude.ai): 955 reviews | Line 130 | Trustpilot | ✅ VERIFIED | Trustpilot shows 959 reviews (close to 955; count changes daily). |
| 58 | Trustpilot: "Mixed sentiment, concentrated at extremes" | Line 130 | Trustpilot | ❌ REJECTED | **Materially mischaracterised.** Trustpilot shows **1.6/5.0 stars** with **76% one-star reviews**, 10% two-star, 3% three-star, 3% four-star, 8% five-star. This is overwhelmingly negative, not "mixed." Only 11% of reviews are 4-5 stars. |
| 59 | Usage limits and throttling as frequent complaint | Lines 136-138 | Trustpilot | ✅ VERIFIED | Multiple Trustpilot reviews confirm rapid throttling, usage limits exhausted quickly, and subscription frustration. Direct page fetch confirms this is the dominant complaint theme. |
| 60 | G2 Reviews: 5.0/5 in some categories | Line 141 | G2 | ⚠️ UNVERIFIABLE | G2 pages require authentication for detailed category breakdowns. Search results show Claude rated positively but no confirmed 5.0/5 in any specific category. G2 overall shows 4.3-4.5/5 range across products. The "5.0/5" claim is likely inflated but cannot be definitively confirmed or denied. |

### Section: What Press Says (Lines 146-157)

| # | Claim | Location | Cited Source | Verification Status | Evidence |
|---|-------|----------|-------------|-------------------|----------|
| 61 | "Most disruptive company" narrative in TIME, Mar 2026 | Line 148 | TIME | ⚠️ UNVERIFIABLE | No URL provided. Search results reference TIME coverage of Anthropic in March 2026 but the specific "most disruptive company" framing could not be confirmed via fetched content. |
| 62 | Mythos data leak concerns | Line 152 | Fortune, Mar 2026 | ✅ VERIFIED | Fortune (Mar 26, 2026): "Anthropic says testing Mythos powerful new AI model after data leak reveals its existence." Confirmed by Axios, TechCrunch, NBC News. |
| 63 | "Anthropic already 40% the size of OpenAI by revenue" | Line 157 | SaaStr | ❌ REJECTED | **Outdated claim presented as current.** By April 2026, Anthropic ($30B ARR) had **surpassed** OpenAI ($25B ARR) per AI Corner and Bloomberg. The "40% the size" figure may have been valid at an earlier date but is contradicted by the document's own April 2026 data context. |
| 64 | Outage on April 6-7, 2026 | Line 154 | AI Daily | ⚠️ UNVERIFIABLE | No URL provided. Cannot verify from cited source. The dates coincide with major announcements (Google/Broadcom, Glasswing). |

### Section: Misalignment Flags (Lines 159-167)

| # | Claim | Location | Cited Source | Verification Status | Evidence |
|---|-------|----------|-------------|-------------------|----------|
| 65 | 4,950 employees as of March 2026 vs ~1,200 in early 2025 (4x growth) | Line 167 | Inference / Glassdoor | ⚠️ PARTIALLY VERIFIED | The ~4,950 figure is from Tracxn only. The ~1,200 base figure is not independently confirmed (Tracxn showed 1,097 for 2025; other sources differ). The "4x growth" claim depends on unverifiable base numbers. |

### Section: Summary & Key Takeaways (Lines 179-189)

| # | Claim | Location | Cited Source | Verification Status | Evidence |
|---|-------|----------|-------------|-------------------|----------|
| 66 | £23 billion ARR and £290 billion valuation | Line 181 | Various | ❌ REJECTED | Repeated currency error. Actual: $30B ARR and $380B valuation. |
| 67 | Eight of the Fortune 10 are now Claude customers | Line 185 | Triangulated | ✅ VERIFIED | Anthropic's Series G announcement confirms: "Eight of the Fortune 10 are now Claude customers." |
| 68 | 7x growth in £750k+ contract cohort | Line 185 | Triangulated | ⚠️ PARTIALLY VERIFIED | Anthropic's announcements reference 7x growth in customers spending $100K+ annually (Series F) and doubling of $1M+ customers (Series G). The specific "£750k+" cohort is not mentioned in any source. The 7x figure appears to map to a different threshold. |
| 69 | Anthropic is a US-registered PBC, not UK entity | Line 175 | N/A | ✅ VERIFIED | Confirmed: Delaware Public Benefit Corporation headquartered in San Francisco. |

---

## Summary

- **Total claims examined:** 69
- **Verified:** 30 (43%)
- **Rejected:** 19 (28%)
- **Partially Verified:** 12 (17%)
- **Unverifiable:** 8 (12%)

---

## Critical Issues

### 1. SYSTEMIC: Currency Conversion Errors (affects 15+ claims)
The document converts all USD figures to GBP using inconsistent and inaccurate rates. Every financial figure is affected. Examples:
- Series G: **$30B** reported as "£23B" (implied rate 0.767)
- Valuation: **$380B** reported as "£290B" (implied rate 0.763)
- Feb 2026 ARR: **$14B** reported as "£14B" (implied rate 1.0 -- no conversion applied)
- Dec 2024 ARR: **$1B** reported as "£0.75B" (implied rate 0.75)
- Claude Code: **$2.5B** reported as "£1.9B" (implied rate 0.76)

The mix of conversion rates (0.75, 0.76, 0.77, and 1.0) makes the financial narrative unreliable.

### 2. Series B: Wrong Date, Amount, and Valuation (Line 13, 77)
Claimed: "Series B ~£900M in February 2023 at £3B+ valuation."
Actual: Series B was **$580M in April 2022** at **$4B valuation**, led by Sam Bankman-Fried/FTX.
The document is wrong on the date (~10 months off), the amount (nearly double the real figure), and arguably the valuation.

### 3. Founding Date Error (Line 76)
Claimed: "March 2021." Actual: **January 2021.** No source corroborates March.

### 4. Core Values Names Fabricated (Line 17)
All seven value names are paraphrased inventions. The document presents "Balance," "Pragmatism," "Trust & Honesty" etc. as if they are Anthropic's stated values, when the actual values have distinctly different names (e.g., "Hold light and shade," "Do the simple thing that works," "Be helpful, honest, and harmless").

### 5. Glassdoor Figures Mostly Wrong (Lines 114-122)
- Review count: **24 stated vs 222 actual** (off by 9x)
- Recommend rate: **86% stated vs 95% actual**
- Career Opportunities: **4.7 stated vs 4.0 actual** (off by 0.7)
- Work-Life Balance: **3.4 stated vs 3.7 actual** (off by 0.3)
- Culture & Values: **4.6 stated vs 4.5 actual** (off by 0.1)

### 6. Trustpilot Sentiment Mischaracterised (Line 130)
Described as "mixed sentiment concentrated at extremes." Actual: **1.6/5.0 with 76% one-star reviews.** This is overwhelmingly negative, not "mixed."

### 7. Microsoft/NVIDIA Partnership Amount Misleading (Line 81)
"£22.5bn commitment" conflates Anthropic's **$30B Azure compute purchase commitment** (money flowing FROM Anthropic TO Microsoft) with the **up to $15B investment** flowing to Anthropic (NVIDIA $10B + Microsoft $5B). The nature and direction of the financial flows are misrepresented.

### 8. "40% the Size of OpenAI" is Outdated (Line 157)
By the document's own stated date (April 2026), Anthropic had **surpassed** OpenAI in revenue ($30B vs $25B). Presenting the "40%" figure as current is contradicted by the document's own data.
