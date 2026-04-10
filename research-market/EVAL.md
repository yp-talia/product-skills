# Research Market — Evaluation Framework & Test Data

## How to evaluate this skill

Four layers of evaluation, in increasing subjectivity.

### Layer 1: Process compliance (mechanical, binary)

| Check | Pass condition |
|---|---|
| Source rules read before research | Yes — `references/source-and-triangulation.md` consulted |
| Market clearly defined before analysis | Yes — industry, segment, and adjacent markets named |
| All five Porter's forces analysed | Yes — each force present with specific evidence |
| Legislation references specific acts/dates | Yes — not just "regulation is increasing" |
| Market trends triangulated | Yes — each trend cited from 2+ sources |
| Demand classification present | Yes — capture, generation, or latent, with evidence |
| Reported vs inferred data distinguished | Yes — inferences labelled as such |
| Inline citations on every factual claim | Yes — no grouped sources |
| Market sizing uses 2+ sources/methodologies | Yes — discrepancies addressed |
| Interview Test applied | Yes — key claims pass insider contradiction check |
| Conciseness target met | Yes — 1,500–2,500 words |

### Layer 2: Specificity of forces analysis (requires human judgement)

For each of Porter's Five Forces: is the analysis specific to this market, or could it describe any industry?

Generic (bad): "Buyers have moderate bargaining power due to available alternatives."
Specific (good): "Mid-market CFOs have high switching costs (6-month implementation cycles) but growing alternatives (FloQast, Numeric) are reducing lock-in. Power is shifting toward buyers as the category matures."

Rate: **Market-specific / Somewhat specific / Textbook generic**

### Layer 3: Demand signal quality (requires human judgement)

Does the demand analysis use real evidence (search volumes, forum activity, content landscape) or just assert that demand exists?

Generic (bad): "There is growing demand for this type of solution."
Specific (good): "Google Trends shows 'pension consolidation' searches up 40% YoY in the UK. Reddit r/UKPersonalFinance has 3 threads per week asking about combining pensions. But page 1 of Google is dominated by IFAs and comparison sites — no product-led results, suggesting a content gap."

Rate: **Evidence-based / Partially evidenced / Asserted**

### Layer 4: Strategic utility (requires human judgement)

Could someone use this analysis to make a market entry, investment, or product strategy decision?

Rate: **Decision-ready / Informative / Academic**

---

## What good looks like

A strong output:
- Market definition is precise and explains why this framing was chosen over alternatives
- Each Porter's force is specific — names companies, cites evidence, assesses direction of change
- Legislation section names specific acts with dates and assesses impact, not just existence
- Demand classification is the most valuable section — clearly distinguishes capture vs generation vs latent
- Google Trends data (where available) adds real-time texture to published reports
- Forum and community signals reveal how real people talk about the problem
- Macro forces are connected to the specific market, not generic economic commentary

A weak output:
- Market definition is vague ("the SaaS market") or too broad
- Porter's forces read like a textbook exercise — could apply to any industry
- Legislation section says "regulation is increasing" without naming specific regulation
- Demand classification is missing or asserted without evidence
- All data comes from published reports — no live demand signals
- Macro forces section is generic economic commentary unconnected to the specific market
- Market sizing presents a single number from one source

---

## Test cases

### Test 1: Mature, well-documented market

**Input:**
> Analyse the market landscape for UK digital banking.

**Expected:**
- Market definition distinguishes digital banking from neobanking from challenger banking
- Porter's forces: high rivalry (Monzo, Starling, Revolut, Chase), moderate new entrant threat (regulatory barriers but open banking lowering technical barriers), substitutes (traditional bank apps improving)
- Legislation: Open Banking regulations, Consumer Duty, APP fraud reimbursement rules — all with specific dates
- Demand classification: demand capture — people actively searching for banking alternatives
- Market sizing: multiple estimates available from analyst firms, should triangulate
- Google Trends shows sustained interest with seasonal patterns

**Pass condition:** Market defined precisely. All five forces specific to UK digital banking. At least 2 named regulations with dates. Demand classified as capture with evidence. Market sizing from 2+ sources.

---

### Test 2: Emerging market with limited published data

**Input:**
> Analyse the market landscape for agentic AI development tools.

**Expected:**
- Acknowledges this is a nascent market — published reports may lag reality
- Market definition includes scope decisions (coding assistants? orchestration frameworks? both?)
- Porter's forces adapted for emerging market: low rivalry but rapid entrant pace, supplier power high (foundation model providers), buyer power low (limited alternatives), substitutes = manual development
- Legislation: AI Act (EU), executive orders, emerging UK AI framework — specific references
- Demand classification likely split: demand capture for coding assistants, demand generation for orchestration tools
- Forum signals (Hacker News, Reddit, Twitter/X) more valuable than published reports

**Pass condition:** Market nascency explicitly acknowledged and shapes the analysis. Forces don't force a mature-market lens. Forum/community signals used to supplement sparse published data. AI regulation cited with specifics.

---

### Test 3: Heavily regulated market

**Input:**
> Analyse the market landscape for UK wealth management / financial advice.

**Expected:**
- Market definition scopes clearly: wealth management vs financial advice vs robo-advice
- Legislation dominates: FCA Consumer Duty, FSCS limits, advice/guidance boundary, pension freedoms, qualification requirements (RDR) — all with specific dates and implications
- Regulatory moats are the central finding — barriers to entry are primarily regulatory, not technical
- Porter's forces shaped by regulation: new entrants face 12+ month authorisation process, supplier power includes compliance technology providers
- Demand classification: likely demand generation (most people don't seek financial advice proactively)
- Macro forces: interest rate environment, pension system changes, intergenerational wealth transfer

**Pass condition:** Regulation is central to the analysis, not a bolt-on section. At least 3 specific regulatory instruments named with dates. Regulatory moat explicitly assessed. Demand classification recognises the advice gap.

---

### Test 4: Market where "do nothing" is the primary substitute

**Input:**
> Analyse the market landscape for pension consolidation platforms.

**Expected:**
- Porter's substitutes analysis: "do nothing" is the dominant substitute, not other platforms
- Demand signals show low awareness but growing interest (pension dashboard programme driving awareness)
- Legislation: Pension Schemes Act 2021, pension dashboards programme timeline, auto-enrolment review
- Market trends: proliferation of small pension pots (job mobility), growing retirement anxiety
- Demand classification: primarily demand generation with some demand capture for "pension transfer" searches
- Community signals: r/UKPersonalFinance discussions reveal confusion and inertia

**Pass condition:** Inertia identified as the primary competitive force. Pension dashboards programme cited with timeline. Demand classification is generation-heavy with evidence. Forum analysis reveals real language people use.

---

### Test 5: Global market requiring geographic scoping

**Input:**
> Analyse the market landscape for e-commerce fulfilment.

**Expected:**
- Market definition includes explicit geographic scoping decision (UK-first per skill default, with global context)
- Porter's forces: high supplier power (logistics infrastructure), high rivalry, Amazon as both competitor and supplier
- Market trends: same-day delivery expectations, sustainability pressure, returns cost challenge
- Macro forces: post-Brexit trade complexity, driver shortages, energy costs
- Market sizing distinguishes 3PL from in-house from marketplace fulfilment
- Demand classification varies by segment: demand capture for established e-commerce, demand generation for D2C brands

**Pass condition:** Geographic scope explicitly stated. Amazon's dual role (competitor + marketplace) addressed. Market sizing distinguishes segments. Brexit implications specific, not generic.

---

## Scorecard (per test run)

| Dimension | Score | Notes |
|---|---|---|
| Process compliance | /11 | One point per check (see Layer 1) |
| Forces specificity | /3 | 3=market-specific, 2=somewhat, 1=textbook |
| Demand signal quality | /3 | 3=evidence-based, 2=partial, 1=asserted |
| Strategic utility | /3 | 3=decision-ready, 2=informative, 1=academic |
| **Total** | **/20** | |

**Target:** ≥16/20 across test cases. Any test below 11/20 warrants immediate skill revision.

---

## Red flags requiring immediate revision

- Porter's Five Forces could apply to any industry — no market-specific evidence
- Legislation section says "regulation is increasing" without naming specific acts
- Demand classification missing entirely
- Market sizing from a single source with no methodology shown
- Google Trends or forum data not attempted (when Chrome is available)
- Market definition too broad (e.g. "the technology market") or undefined
- Macro forces section is generic economic commentary
- Reported and inferred data not distinguished
- Inline citations missing or grouped at section end
- Interview Test not applied — market claims an industry insider would dispute
- "Do nothing" not considered as a substitute when it's clearly the dominant alternative
