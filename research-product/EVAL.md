# Research Product — Evaluation Framework & Test Data

## How to evaluate this skill

Four layers of evaluation, in increasing subjectivity.

### Layer 1: Process compliance (mechanical, binary)

| Check | Pass condition |
|---|---|
| Source rules read before research | Yes — `references/source-and-triangulation.md` consulted |
| Full product portfolio mapped | Yes — not just the headline product |
| Users, buyers, and beneficiaries distinguished | Yes — all three identified separately |
| Value chain articulated | Yes — input → transformation → output → beneficiary |
| Pricing captured from Tier 1 source | Yes — company's own pricing page, with access date |
| Unit economics assumptions stated | Yes — every estimate shows its working |
| Market sizing uses 2+ methodologies | Yes — top-down and bottom-up, with triangulation |
| Product teardown has specific observations | Yes — 3–5 observations with "what / why it matters / improvement hypothesis" |
| Inline citations on every factual claim | Yes — no paragraph ends with grouped sources |
| Interview Test applied | Yes — key claims pass the insider contradiction check |
| Conciseness target met | Yes — 1,500–2,500 words |

### Layer 2: Estimation quality (requires human judgement)

For unit economics and market sizing: are the assumptions reasonable? Could you defend them to a sceptical product leader?

Generic (bad): "CAC is estimated to be moderate."
Specific (good): "CAC estimated at £800–£1,200 based on: 12-person sales team (LinkedIn), enterprise sales cycle (no self-serve), average SaaS AE quota assumption of £600k. Confidence: low — team size is the only hard data point."

Rate: **Defensible / Reasonable / Hand-wavy**

### Layer 3: Teardown quality (requires human judgement)

Does the product teardown produce observations a product leader would find useful? Not feature descriptions — opinionated observations about UX quality, strategic choices, and gaps.

Generic (bad): "The onboarding flow asks for your email and company name."
Specific (good): "Onboarding asks for company size in the second step — this is likely a routing mechanism for PLG-to-sales handoff. But the threshold isn't visible to the user, creating an uncanny moment when large-company users suddenly get a 'book a demo' CTA instead of the product."

Rate: **Insightful / Competent / Descriptive only**

### Layer 4: Strategic value (requires human judgement)

Does the output help someone understand the product as a business, not just as a feature set? Could you use this to brief a new PM joining the company?

Rate: **Strategic / Functional / Surface-level**

---

## What good looks like

A strong output:
- Maps the full product portfolio, not just the hero product
- Distinguishes users from buyers from beneficiaries with specific evidence
- Has a value chain that reveals where value is created vs captured
- Shows unit economics working with explicit assumptions and confidence levels
- Market sizing uses two methodologies and explains the discrepancy
- Product teardown has observations that show genuine product thinking — not just screenshots described
- Identifies the product maturity stage with evidence, not just assertion
- Partnerships section reveals strategic dependencies

A weak output:
- Describes features from the marketing page without analysis
- Conflates users and buyers
- Has market sizing with one number and no methodology
- Unit economics section says "insufficient data" without attempting estimation
- Product teardown reads like a feature walkthrough
- No distinction between what the product does and what makes it interesting
- Partnerships listed without strategic assessment

---

## Test cases

### Test 1: B2B SaaS with public pricing and free trial

**Input:**
> Analyse Notion's product.

**Expected:**
- Full portfolio mapped: wikis, docs, databases, projects, AI, calendar — not just "Notion is a note-taking app"
- Users (individual contributors), buyers (team leads, IT), and beneficiaries (whole team) clearly distinguished
- Pricing captured with date: free, Plus, Business, Enterprise tiers with specific prices
- Product teardown includes specific UX observations (template gallery as onboarding, blank page problem, performance on large databases)
- Unit economics estimated with assumptions: freemium conversion rate, estimated ARPU across tiers
- Market sizing addresses the "which market is Notion in?" problem — productivity, project management, knowledge management, or all three?

**Pass condition:** Portfolio has 4+ product lines identified. Users ≠ buyers ≠ beneficiaries. Market sizing acknowledges the category ambiguity. Teardown has at least 3 specific observations with improvement hypotheses.

---

### Test 2: Consumer product with opaque economics

**Input:**
> Analyse Monzo's product.

**Expected:**
- Product portfolio: current accounts, savings, borrowing, business accounts, Monzo Plus/Premium, energy switching, salary sorting
- Revenue model complexity captured: interchange, Plus/Premium subscriptions, lending, marketplace referrals
- Users and buyers are the same person (consumer) — but beneficiaries may differ (joint accounts, under-18 accounts)
- Unit economics honestly addresses the profitability challenge with available data
- Product teardown captures what makes Monzo's UX distinctive vs traditional banking
- Market sizing scoped to UK digital banking, not "the global banking market"

**Pass condition:** Revenue model names at least 3 distinct revenue streams. Unit economics attempts estimation with stated assumptions. Teardown produces observations specific to Monzo, not generic "good mobile banking" praise.

---

### Test 3: Early-stage product with minimal public information

**Input:**
> Analyse Tessl's product.

**Expected:**
- Acknowledges limited public data
- Reconstructs product understanding from website, blog, job postings, founder interviews
- Product teardown flagged as inferred (no public product access)
- Market sizing attempted with wide confidence intervals and explicit methodology
- Does NOT fabricate specifics to fill gaps
- Identifies what's knowable vs unknowable at this stage

**Pass condition:** Output clearly labels inferred vs observed. No fabricated pricing or unit economics. Market sizing shows methodology even if ranges are wide.

---

### Test 4: Product with complex value chain (marketplace or platform)

**Input:**
> Analyse Deliveroo's product.

**Expected:**
- Multi-sided value chain mapped: restaurants, riders, consumers, grocery partners
- Each side has its own users/buyers/beneficiaries analysis
- Pricing captures all sides: consumer delivery fees, restaurant commission, rider economics
- Unit economics addresses the per-order economics challenge
- Product teardown covers consumer app AND restaurant portal (at least from external evidence)
- Growth vs capture analysis addresses the Uber Eats/Just Eat competitive dynamic

**Pass condition:** All marketplace sides identified and analysed. Unit economics attempts per-order breakdown. Value chain shows where value is created (convenience, aggregation) vs captured (commission, delivery fee).

---

### Test 5: Mature product in a commoditised space

**Input:**
> Analyse Mailchimp's product.

**Expected:**
- Portfolio evolution captured: email → marketing platform → website builder → CRM
- Product maturity assessed as optimising with evidence
- Market sizing acknowledges the email marketing vs marketing automation distinction
- Competitive moat analysis: what keeps customers despite many alternatives?
- Teardown observes the tension between simplicity (original value prop) and feature bloat
- Intuit acquisition context and what it means for the product direction

**Pass condition:** Portfolio shows evolution over time. Maturity stage matches evidence. Teardown identifies at least one strategic tension.

---

## Scorecard (per test run)

| Dimension | Score | Notes |
|---|---|---|
| Process compliance | /11 | One point per check (see Layer 1) |
| Estimation quality | /3 | 3=defensible, 2=reasonable, 1=hand-wavy |
| Teardown quality | /3 | 3=insightful, 2=competent, 1=descriptive |
| Strategic value | /3 | 3=strategic, 2=functional, 1=surface-level |
| **Total** | **/20** | |

**Target:** ≥16/20 across test cases. Any test below 11/20 warrants immediate skill revision.

---

## Red flags requiring immediate revision

- Product described as a feature list with no strategic analysis
- Users, buyers, and beneficiaries conflated without acknowledgement
- Market sizing presents a single number with no methodology
- Unit economics claims precision that exceeds available evidence
- Product teardown describes features instead of making observations
- "Insufficient data" used as a reason to skip estimation entirely — should always attempt with caveats
- Inline citations missing or grouped at section end
- Full product portfolio ignored — only the headline product analysed
- Interview Test not applied — product maturity or economics claims an insider would dispute
