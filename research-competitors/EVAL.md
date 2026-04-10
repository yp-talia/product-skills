# Research Competitors — Evaluation Framework & Test Data

## How to evaluate this skill

Four layers of evaluation, in increasing subjectivity.

### Layer 1: Process compliance (mechanical, binary)

| Check | Pass condition |
|---|---|
| Source rules read before research | Yes — `references/source-and-triangulation.md` consulted |
| Three competitor categories mapped | Yes — direct, strategic, and adjacent all present |
| Feature comparison matrix present | Yes — 8–15 features, uses ✅/❌/🟡/❓ with sources |
| Audience segmentation per competitor | Yes — not just "SMEs" — specific size, industry, persona |
| Pricing comparison with access date | Yes — table present, date noted |
| Underserved segments identified | Yes — with supporting evidence |
| Inline citations on every factual claim | Yes — no grouped sources |
| Feature claims verified beyond marketing page | Yes — ❓ used where unverified, not ✅ |
| Review volume noted as market signal | Yes — not just sentiment, but volume itself analysed |
| Interview Test applied | Yes — feature claims pass insider contradiction check |
| Conciseness target met | Yes — 1,500–2,500 words |

### Layer 2: Comparison quality (requires human judgement)

Does the feature matrix reveal genuine differentiation, or does it just list features where everyone has ✅?

Generic (bad): A matrix where 80% of cells are ✅ — tells you nothing.
Specific (good): A matrix that reveals distinct positioning — Company A strong on X but weak on Y, Company B the opposite. The matrix tells a strategic story.

Rate: **Reveals positioning / Adequate / Undifferentiated**

### Layer 3: Strategic insight (requires human judgement)

Does the analysis help someone understand why the market looks the way it does, or just describe what exists?

Generic (bad): "Company A targets enterprises and Company B targets SMEs."
Specific (good): "The market is bifurcating: incumbents are moving upmarket to sustain margins, leaving a widening gap in the £10–50/user/month range that two well-funded startups are now targeting. The target company sits between these segments with no clear positioning advantage in either."

Rate: **Strategic / Descriptive / Cataloguing**

### Layer 4: Actionability (requires human judgement)

Could someone use this analysis to make a product or positioning decision?

Rate: **Decision-ready / Informative / Reference only**

---

## What good looks like

A strong output:
- Competitor map covers direct, strategic, and adjacent — with reasoning for each category assignment
- Feature matrix tells a strategic story — you can see positioning gaps
- Each direct competitor deep-dive reveals a distinct strategic bet, not just feature differences
- Underserved segments are supported by evidence (review gaps, pricing gaps, geographic gaps)
- SimilarWeb and review volume data used as market signals, not just decoration
- Brand perception section captures themes, not just star ratings
- Distribution comparison reveals genuinely different go-to-market approaches

A weak output:
- Lists competitors without categorising them
- Feature matrix is a wall of ✅ that reveals nothing
- All competitors described in the same terms ("leading provider of...")
- Underserved segments are guesses without evidence
- Pricing table has no date
- Feature claims all sourced from marketing pages only
- "No underserved segments identified" — almost always wrong

---

## Test cases

### Test 1: Crowded B2B SaaS market

**Input:**
> Map the competitive landscape for Notion.

**Expected:**
- Direct: Coda, Confluence, Slite, Nuclino
- Strategic: Google Docs + Sheets (job-to-be-done overlap), Airtable (database use case), Monday.com/Asana (project management overlap)
- Adjacent: AI writing tools (Jasper, Copy.ai), Microsoft Loop
- Feature matrix reveals: Notion strong on flexibility, weak on structured project management. Confluence strong on enterprise, weak on UX
- Audience segmentation shows: Notion skews startup/SME, Confluence enterprise, Coda power users
- Underserved segment: teams that need Notion's flexibility with Confluence's enterprise controls

**Pass condition:** All three competitor categories populated with reasoning. Feature matrix has ≤60% cells as ✅ (i.e., reveals actual differentiation). Underserved segment is evidence-backed.

---

### Test 2: Emerging market with few established players

**Input:**
> Map the competitive landscape for Tessl.

**Expected:**
- Acknowledges the market is nascent — categories may not be clean
- Direct competitors may be limited; identifies the closest comparable approaches
- Strategic competitors include the "do nothing" option and manual alternatives
- Adjacent: large platform companies that could enter (e.g. GitHub Copilot extensions, Cursor, Replit)
- Feature matrix adapted for emerging market — may use capability themes rather than specific features
- Underserved segments may be the entire market if no one serves it well yet

**Pass condition:** Analysis doesn't force a mature-market framework onto a nascent market. "Do nothing" or manual alternatives acknowledged as the real competitor. Feature matrix adapted rather than forced.

---

### Test 3: Consumer market with strong brand dynamics

**Input:**
> Map the competitive landscape for Monzo.

**Expected:**
- Direct: Starling, Revolut, Chase UK
- Strategic: traditional banks (Lloyds, NatWest) with improved apps, Apple Pay / Google Pay (unbundling payments)
- Adjacent: credit builders (Loqbox), savings apps (Plum, Chip), BNPL (Klarna)
- Review volume analysis: massive review volumes across Trustpilot/App Store → mature demand-capture market
- Brand perception captures emotional loyalty (Monzo) vs functional trust (Starling) vs feature breadth (Revolut)
- Pricing comparison addresses the "free core product" dynamic — compares premium tier monetisation

**Pass condition:** Brand perception goes beyond star ratings to themes. Review volume used as market signal. The "free product" pricing challenge addressed rather than ignored.

---

### Test 4: Market with dominant incumbent

**Input:**
> Map the competitive landscape for a Salesforce challenger (e.g. HubSpot CRM, Pipedrive, or Attio).

**Expected:**
- Analysis frames everything relative to the incumbent's gravity
- Explains why challengers can exist despite Salesforce's dominance (complexity, price, specific use cases)
- Feature matrix doesn't try to compare everything — focuses on where challengers differentiate
- Distribution analysis captures how challengers acquire customers who might default to Salesforce
- Underserved segments: teams too small for Salesforce, specific verticals, teams that hate Salesforce's UX

**Pass condition:** Salesforce's dominance shapes the analysis rather than being listed as "another competitor". Challenger positioning articulated as strategic choices, not just feature gaps.

---

### Test 5: Market where the biggest competitor is "do nothing"

**Input:**
> Map the competitive landscape for a startup automating pension transfers (e.g. PensionBee).

**Expected:**
- Acknowledges that the primary competitor is inertia — people leaving pensions untouched
- Direct competitors listed but analysis notes low awareness across the category
- Review volume analysis reveals low volumes → demand generation market
- Distribution comparison emphasises education and trust-building over feature comparison
- Underserved segments: younger workers with multiple small pots, people approaching retirement with scattered pensions

**Pass condition:** "Do nothing" / inertia identified as the primary competitive force. Demand classification (generation, not capture) informs the analysis. Feature matrix is secondary to the distribution and trust comparison.

---

## Scorecard (per test run)

| Dimension | Score | Notes |
|---|---|---|
| Process compliance | /11 | One point per check (see Layer 1) |
| Comparison quality | /3 | 3=reveals positioning, 2=adequate, 1=undifferentiated |
| Strategic insight | /3 | 3=strategic, 2=descriptive, 1=cataloguing |
| Actionability | /3 | 3=decision-ready, 2=informative, 1=reference only |
| **Total** | **/20** | |

**Target:** ≥16/20 across test cases. Any test below 11/20 warrants immediate skill revision.

---

## Red flags requiring immediate revision

- All competitors listed as "direct" — no strategic or adjacent category
- Feature matrix where 80%+ cells are ✅ — no differentiation visible
- Feature claims sourced only from marketing pages — no verification attempted
- Pricing table without access date
- "No underserved segments identified" — nearly always indicates insufficient analysis
- Competitors described with their own marketing language rather than assessed
- Review volume ignored — only star ratings reported
- Inline citations missing or grouped at section end
- Market structure not addressed — is this consolidating, fragmenting, or bifurcating?
- Interview Test not applied — feature or positioning claims an insider would dispute
