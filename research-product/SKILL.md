---
name: research-product
version: "1.0"
description: >
  Analyse a company's product — what it is, who it serves, value chain, unit economics, market sizing, and a hands-on experience teardown. Also covers partnerships and ecosystem. Trigger whenever the user wants to understand a product, analyse a product, do a product teardown, assess a product's market, or evaluate a product before an interview, investment, or strategic decision.
---

# Research Product

Produce a deep analysis of a company's product: what it is, who it serves, how value flows, the economics behind it, how big the market is, and what the actual experience of using it is like. This skill goes beyond surface-level feature lists — it assesses the product as a business and as a user experience.

## Required Tools

- **WebSearch** — product information, reviews, case studies, market data
- **WebFetch** — product pages, pricing pages, documentation, industry reports

## Recommended Tools

- **Claude in Chrome** — product walkthroughs, G2/Capterra detailed reviews, interactive product pages. If unavailable, note which sections are based on inference rather than first-hand observation.

## Source Rules

Read `references/source-and-triangulation.md` before beginning. Company's own product pages and pricing are Tier 1 (treated as true). Market sizing requires minimum 2 independent sources or methodologies. Unit economics estimates must state all assumptions.

### Inline Citation Requirement

**CRITICAL**: Every factual statement in the output MUST have its source placed immediately next to the specific claim — not grouped at the end of a section, paragraph, or profile. The reader must be able to verify any individual statement without hunting for its source.

**Format**: `[Claim text]. [Source: Name, URL, accessed YYYY-MM-DD]`

**Rules**:
1. Every individual factual statement gets its own inline citation
2. If two consecutive facts come from the same source, still cite each one
3. If a claim is your inference rather than a sourced fact, label it: `[Inference based on: ...]`
4. Never write a paragraph of facts and then put a list of sources at the end

### Currency

Report all financial figures in their original currency. Do not convert. If a comparison requires normalisation, show both currencies with the exchange rate and date used.

### Source Integrity

Never cite a URL you have not fetched and read in this session. Never invent article titles, author names, or publication dates. If you cannot find a source for a claim, either state the claim is unverified or remove it entirely.

### Review Platform Accuracy

When reporting ratings from Trustpilot, Glassdoor, G2, Capterra, or app store reviews, fetch the actual page and report the exact numbers shown. Do not estimate or recall from memory — these numbers change frequently and errors here are immediately visible to anyone who checks.

## Research Steps

### Step 1: Product Overview

Research what the product does:
- **Product website** — features, use cases, how it works
- **Documentation / help centre** — depth of product, complexity signals
- **Demo videos / product tours** — if publicly available
- **Product Hunt / launch announcements** — positioning at launch vs now

Capture: core value proposition, key features, how it works at a high level.

### Step 2: Existing Product Line Analysis

Map everything the company offers — not just the headline product:

#### 2a: Map the Full Product Portfolio

- **All products and services** — check main navigation, footer links, pricing page, help centre
- **Product line structure** — how does the company organise its offerings? By customer segment, life event, service type?
- **Revenue significance** — which product lines appear to drive most revenue?
- **Maturity per line** — the company may have a mature flagship alongside a nascent new line
- **Launch timeline** — when was each product introduced? Blog posts, press releases, Product Hunt, Wayback Machine

#### 2b: Deep-Dive the Core Product(s)

- **User journey mapping** — walk through the core product end-to-end (via Chrome if accessible, or reconstruct from demos/reviews/help docs)
- **Pricing and packaging** — tiers, ACV signals
- **Customer reviews specific to the core product** — what do users love and hate?
- **Operational model** — purely digital, or involves human professionals?
- **Technology and infrastructure signals** — shared capabilities across product lines

#### 2c: Analyse What Can Be Leveraged

Assess reusable assets across product lines:
- **Reusable infrastructure** — shared technical components
- **Existing user base as a channel** — cross-sell potential
- **Brand and trust transfer** — does the brand credibly extend?
- **Operational capabilities** — existing professional relationships
- **Design patterns and UX conventions** — interaction patterns users expect
- **Pricing model precedent** — what the existing model signals about willingness to pay
- **Data assets** — data accumulated that could inform new products

#### 2d: Assess the Strategic Gap

Articulate what's missing — the gap between what exists and what the market needs:
- What customer need does the gap address?
- Is this a natural adjacency or a strategic leap?
- What evidence exists for demand?
- What's the implied go-to-market?

### Step 3: Users, Buyers & Beneficiaries

These are often different people. Map them:
- **Users** — who interacts with the product daily?
- **Buyers** — who makes the purchase decision?
- **Beneficiaries** — who benefits from the product's output?

Sources: case studies, testimonials, job postings that mention the tool, G2 reviewer profiles.

### Step 4: Value Chain

Map how value flows:
- What input does the product take?
- What transformation does it perform?
- What output does it deliver?
- How does the output reach the beneficiary?
- Where is value created vs where is value captured (pricing)?

### Step 5: Pricing & Revenue Model

Research from the company's pricing page (Tier 1):
- Pricing model (subscription, usage-based, per-seat, freemium, transaction fee)
- Price points and tiers
- What's included at each tier
- Enterprise pricing signals
- Any recent pricing changes

### Step 6: Unit Economics Assessment

Based on available data, estimate or infer:

**Customer Acquisition Cost (CAC) signals:**
- Marketing team size and spend signals
- Sales team size
- Self-serve vs sales-assisted conversion

**Lifetime Value (LTV) signals:**
- Pricing × estimated contract length
- Churn indicators from reviews
- Upsell/expansion signals

**Gross Margin indicators:**
- Software vs services mix
- Infrastructure intensity
- People intensity

**State every assumption explicitly.** If data is insufficient to estimate, say so. Be especially careful about precision that exceeds your evidence.

### Step 7: Product Maturity

Assess where the product sits:
- **0→1** — recently launched, finding product-market fit
- **Scaling** — PMF established, growing customer base
- **Optimising** — mature product, focus on retention and efficiency

Evidence: product age, feature breadth, customer testimonials, competitive positioning, team size.

### Step 8: Market Sizing

Estimate TAM, SAM, SOM:

**Show your methodology.** Use at least two approaches:
1. **Top-down**: industry reports, analyst estimates
2. **Bottom-up**: number of potential customers × average revenue per customer

Triangulate: if approaches produce wildly different numbers, investigate why.

### Step 9: Growth vs Capture

Assess:
- **Market expansion** — growing the overall market?
- **Market capture** — taking share from competitors?
- **Adjacent expansion** — moving into new segments or geographies?

### Step 10: Product Experience Teardown

**If the product is publicly accessible** (via Chrome):
1. Visit the product website
2. Sign up or start a free trial if available
3. Walk through the onboarding flow
4. Experience the core workflow
5. Note: UX quality, load times, mobile responsiveness, error handling, onboarding friction, empty states

**Produce 3–5 specific observations**, each with:
- What you observed
- Why it matters
- An improvement hypothesis

**If the product is NOT publicly accessible:**
- Map the journey from demos, screenshots, case studies, and user reviews
- Note what you can't assess and why
- Still produce observations, but flag them as inferred

### Step 11: Partnerships & Ecosystem

Research:
- **Integrations** — what does the product connect to?
- **Channel partners** — who resells or recommends this product?
- **Technology partners** — whose infrastructure do they depend on?
- **Strategic alliances** — co-marketing, co-development, data sharing

Assess: what can they build vs what must they integrate? Do partnerships constrain the roadmap? Where does the ecosystem create leverage?

### Step 12: Verification Pass

Before writing up, run the Interview Test on every key claim. Pay special attention to:
- Unit economics estimates — could an insider easily refute your numbers?
- Product maturity assessment — does it match signals from job postings?
- Market sizing — are your numbers defensible if challenged?
- Any negative claims — have you checked enough sources?

### Step 13: Write Up

Synthesise all findings following the output template in `references/output-templates.md` (Product Analysis), or adapt to your preferred format. Ensure every factual claim is cited, every estimate shows its methodology, and every assumption is stated.

### Limitations

- Product teardowns require Chrome for the richest observations; without it, assessments are inferred from public materials
- Unit economics for private companies are inherently estimates — flag confidence levels
- Market sizing varies significantly by methodology; always show your working
- Products behind login walls or enterprise paywalls can only be assessed from external signals

### Conciseness

Target 1,500–2,500 words for a standard product analysis. The product teardown and market sizing are the highest-value sections. Trim generic product descriptions in favour of opinionated observations.
