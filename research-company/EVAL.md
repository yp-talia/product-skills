# Research Company — Evaluation Framework & Test Data

## How to evaluate this skill

Four layers of evaluation, in increasing subjectivity.

### Layer 1: Process compliance (mechanical, binary)

| Check | Pass condition |
|---|---|
| Source rules read before research | Yes — `references/source-and-triangulation.md` consulted |
| Company's own voice captured first | Yes — website, about, careers, blog checked before external sources |
| Inline citations on every factual claim | Yes — no paragraph ends with a grouped source list |
| Companies House lookup follows procedure | Yes — used company number (Route 1) or verified directors (Route 2), not name-only search |
| Multi-perspective analysis present | Yes — company vs investor vs employee vs customer views compared |
| Misalignments flagged | Yes — contradictions between perspectives explicitly called out |
| Negative claims checked against 3+ sources | Yes — "does not" / "has no" / "hasn't" claims cite verification attempts |
| Information gaps acknowledged | Yes — missing data stated, not silently omitted |
| Interview Test applied | Yes — key claims pass the "could an insider easily contradict this?" check |
| Conciseness target met | Yes — 1,500–2,500 words |

### Layer 2: Source quality (requires human judgement)

For each major claim, check:
- Is the source appropriate for the claim type? (Tier 1 for company self-reported, triangulated for external claims)
- Is the citation placed immediately next to the specific claim?
- Are inferences clearly labelled as inferences?

Rate: **Strong sourcing / Adequate / Weak sourcing**

### Layer 3: Analytical depth (requires human judgement)

Does the output go beyond summarising what the company says about itself? The multi-perspective analysis should surface genuine tensions — not just restate each perspective in sequence.

Generic (bad): "Employees generally report positive experiences. Customers are mostly satisfied."
Specific (good): "Glassdoor reviews consistently praise engineering culture but flag sales team turnover. This aligns with customer complaints about account manager churn on G2, suggesting a retention issue concentrated in commercial roles."

Rate: **Insightful / Competent / Surface-level**

### Layer 4: Practical value (requires human judgement)

Would someone preparing for a meeting with this company learn something they couldn't get from 10 minutes on the company's website?

Rate: **Significantly additive / Somewhat additive / Mostly restatement**

---

## What good looks like

A strong output:
- Opens with a concise summary that tells you what this company is about in 2–3 sentences
- Names specific competitors, investors, and market context — not just what the company says about itself
- Has a multi-perspective section where perspectives genuinely conflict and those conflicts are analysed
- Flags something surprising — a signal most people would miss
- Has financial data from Companies House that's been correctly attributed to the verified entity
- Uses employee sentiment to triangulate culture claims
- Identifies growth model clearly (PLG, sales-led, content, partnerships) with evidence
- Every claim is verifiable from its inline citation

A weak output:
- Reads like a rewritten "About us" page
- Has a multi-perspective section where all perspectives suspiciously agree
- Reports Companies House data without verifying it's the right entity
- States "no negative press found" without evidence of searching
- Has inline citations that all point to the company's own website
- Misses obvious public information (recent funding round, leadership change)
- Exceeds 2,500 words with padding rather than insight

---

## Test cases

### Test 1: Well-known company with rich data

**Input:**
> Research Monzo for me.

**Expected:**
- Company number found on website footer → Companies House lookup via Route 1
- Funding history detailed (Series A through recent rounds)
- Employee sentiment from Glassdoor shows specific patterns (not just "4.2 stars")
- Customer sentiment captures both the fan base and common complaints (customer service wait times, account freezes)
- Growth model identified as PLG with specific evidence (referral programme, freemium model)
- Multi-perspective analysis surfaces tension: strong brand loyalty vs profitability pressure
- Technology section captures their cloud-native, microservices architecture

**Pass condition:** Companies House entity verified. At least 3 perspectives represented with at least 1 genuine conflict surfaced. Names specific investors and amounts for most recent round. Growth model clearly identified with evidence.

---

### Test 2: Early-stage company with sparse data

**Input:**
> Research Tessl for me.

**Expected:**
- Acknowledges data limitations upfront — early-stage company with limited press
- Website thoroughly mined as primary source
- Founding team and background captured
- Funding data found (if any) or absence noted
- SimilarWeb likely unavailable — noted as a signal about scale
- Technology signals inferred from job postings and product description
- Does NOT fabricate data to fill gaps
- Information gaps section is substantive, not a throwaway line

**Pass condition:** Output explicitly states what couldn't be found and why. No fabricated data. Companies House lookup attempted. Word count may be below 1,500 — that's acceptable if the data genuinely isn't there.

---

### Test 3: Company where trading name differs from registered name

**Input:**
> Research amicable for me.

**Expected:**
- Website footer checked for company number
- If name-only search used: "amicable" returns wrong results; skill follows Route 2 and verifies directors
- Correct entity identified (E-Negotiation Ltd or similar) with verification evidence shown
- Does NOT report financial data from wrong entity
- If entity can't be confidently matched, states this explicitly

**Pass condition:** Either finds correct entity with director verification, or explicitly states it couldn't confidently match. Does NOT silently report data from an unverified entity.

---

### Test 4: Company with strong PR but weak fundamentals

**Input:**
> Research a company that has recently received negative press (e.g. a startup post-layoff or post-controversy).

**Expected:**
- Does not lead with the company's own positive narrative
- Captures both the positive PR and the negative signals
- Multi-perspective section genuinely engages with the tension
- Employee sentiment section doesn't shy away from patterns in negative reviews
- Financial signals cross-referenced with headcount changes
- Balanced — doesn't pile on, but doesn't whitewash either

**Pass condition:** Negative press is present and contextualised. Employee sentiment includes specific themes from reviews. Output doesn't read like either a hit piece or a press release.

---

### Test 5: Non-UK company (Companies House not applicable)

**Input:**
> Research Figma for me.

**Expected:**
- Companies House step correctly skipped (US company) with brief note
- Financial data sourced from Crunchbase, press, SEC filings where available
- Does NOT attempt UK Companies House lookup for a US company
- All other research steps followed normally
- Adobe acquisition context included

**Pass condition:** No Companies House lookup attempted. Financial data sourced appropriately for a US company. Output quality doesn't degrade because one step was skipped.

---

## Scorecard (per test run)

| Dimension | Score | Notes |
|---|---|---|
| Process compliance | /10 | One point per check (see Layer 1) |
| Source quality | /3 | 3=strong, 2=adequate, 1=weak |
| Analytical depth | /3 | 3=insightful, 2=competent, 1=surface-level |
| Practical value | /3 | 3=significantly additive, 2=somewhat, 1=restatement |
| Multi-perspective quality | /3 | 3=genuine conflicts surfaced, 2=perspectives listed, 1=single voice |
| **Total** | **/22** | |

**Target:** ≥18/22 across test cases. Any test below 13/22 warrants immediate skill revision.

---

## Red flags requiring immediate revision

- Companies House data reported from an unverified entity
- "No negative press found" without evidence of searching for it
- Multi-perspective section where all perspectives agree
- Inline citations missing — sources grouped at end of sections
- Company's own claims presented as verified facts without triangulation
- Financial data presented without source or methodology
- Output exceeds 3,000 words without proportionally more insight
- Information gaps not acknowledged — output appears artificially complete
- Interview Test not applied — claims that an insider would immediately dispute
