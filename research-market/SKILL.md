---
name: research-market
version: "1.0"
description: >
  Analyse the market landscape around a company using Porter's Five Forces, legislation tracking, trend analysis, and macro forces. Trigger whenever the user wants to understand a market, analyse market dynamics, assess competitive forces, research industry trends, or prepare market context before an interview or strategic decision.
---

# Research Market

Map the forces and trends shaping a company's operating environment. This skill produces a structured analysis of competitive forces (Porter's Five Forces), regulatory landscape, market trends, and macro conditions.

## Required Tools

- **WebSearch** — industry reports, regulatory changes, trend analysis, analyst commentary
- **WebFetch** — specific reports, government/regulatory body pages, industry publications

## Recommended Tools

- **Claude in Chrome** — Google Trends for live search demand data, forum/community research. If unavailable, the analysis will rely on published reports only and miss real-time demand signals — note this limitation in your output.

## Source Rules

Read `references/source-and-triangulation.md` before beginning. Legislation must reference specific acts/regulations with dates. Market trends require triangulation. Market size/growth figures need minimum 2 independent sources.

**Reported vs inferred data**: Be explicit about whether a data point comes from a published source (reported) or from your own reasoning (inferred). "The UK legaltech market is estimated at £1.2bn [Source: ...]" is reported data. "This suggests the family law segment is roughly £200m" is an inference — label it as such.

### Inline Citation Requirement

**CRITICAL**: Every factual statement in the output MUST have its source placed immediately next to the specific claim. See `references/source-and-triangulation.md` for full citation rules.

### Currency

Report all financial figures in their original currency. Do not convert. If a comparison requires normalisation, show both currencies with the exchange rate and date used.

### Source Integrity

Never cite a URL you have not fetched and read in this session. Never invent article titles, author names, or publication dates. If you cannot find a source for a claim, either state the claim is unverified or remove it entirely.

## Research Steps

### Step 1: Define the Market

Before analysing forces, clearly define what market you're analysing. The same company can be framed in different markets depending on the lens:
- What industry does this company operate in?
- What specific segment within that industry?
- What adjacent markets overlap or compete?

Get this right first — it frames everything that follows.

### Step 2: Porter's Five Forces

For each force, research the specific dynamics in this company's market. Avoid generic analysis — every point should be evidenced.

**Threat of New Entrants**
- Barriers to entry (capital, regulatory, technical, network effects, brand loyalty)
- Significant new entrants in the last 2 years
- Are barriers rising or falling?

**Bargaining Power of Suppliers**
- Key suppliers (technology providers, data sources, talent pools)
- Concentration and switching costs
- Have any suppliers made moves to compete directly?

**Bargaining Power of Buyers**
- Concentration, switching costs, price sensitivity
- Do buyers have alternatives? How easy to find?
- Are buyers becoming more sophisticated?

**Threat of Substitutes**
- Alternative approaches to the same problem (not just direct competitors)
- Are any substitutes gaining traction?
- What would cause a switch?

**Competitive Rivalry**
- Number of competitors, market concentration
- Growing (positive-sum) or stagnant (zero-sum)?
- How differentiated are offerings?
- Recent exits, mergers, or consolidation?

### Step 3: Legislation & Regulation

Research with a UK-first lens, then EU/global where relevant:

- **Recent changes** (last 12 months)
- **Upcoming changes** — proposed legislation, consultations, expected dates
- **Regulatory bodies** — who regulates, what are their current priorities?
- **Compliance requirements** — what must companies do to operate?
- **Regulatory moats** — does regulation benefit incumbents?

For each piece of regulation, note: the specific act/regulation name, implementation date, impact on companies, and whether it creates opportunities or threats.

### Step 4: Market Trends

**Technology trends**
- What technologies are changing how products in this space work?
- Are there technology inflection points approaching?

**Customer/user expectation shifts**
- Self-serve vs high-touch expectations
- Mobile-first, real-time, personalisation
- Privacy and data ownership concerns

**Distribution model changes**
- PLG replacing sales-led, marketplace dynamics, embedded finance/tech

**Market structure trends**
- Consolidation vs fragmentation
- Vertical integration vs specialisation

For each trend, triangulate: a trend reported by one blogger is a hypothesis; a trend reported by multiple authoritative sources is a trend.

### Step 5: Demand Signal Analysis

Gather live demand data — not from cached results, but from tools that show current search behaviour and public discussion.

#### 5a: Google Trends (trends.google.co.uk)

Using Chrome (if available):
- **Core product terms** — interest over time (12 months and 5 years), geographic breakdown, related rising queries
- **Comparative term analysis** — compare related terms (up to 5). Relative volumes matter more than absolute
- **Seasonal patterns** — demand spikes at certain times?
- **Category context** — compare against broader category terms

#### 5b: Content Landscape Analysis

Search Google for key product terms and analyse:
- **Page 1 composition** — legal firms (established market), informational articles (education-stage), comparison sites (mature with alternatives), government guidance (regulatory-driven)
- **Content volume and quality** — content gap = opportunity; crowded = validates demand
- **Paid advertising presence** — confirms commercial intent

#### 5c: Forum and Community Signals

Search Reddit, Mumsnet, and relevant forums:
- **Discussion volume and recency** — are real people asking about this?
- **Question patterns** — awareness gap vs discovery problem vs comparison shopping
- **Sentiment and barriers** — what stops people from acting?
- **Language people actually use** — often differs from formal terms

#### 5d: Demand Classification

Synthesise into a classification:

- **Demand capture** — significant search volume, people actively looking. GTM: SEO, paid search, comparison sites
- **Demand generation** — people have the need but don't know the solution exists. GTM: content, partnerships, PR
- **Latent demand** — people don't yet recognise the problem. GTM: behaviour change, regulatory catalysts

This classification is one of the most strategically important outputs of the entire research process.

### Step 6: Macro Forces

- **Economic conditions** — how does the current economy affect demand?
- **Investment climate** — are investors bullish or bearish on this sector?
- **Talent market** — easy or hard to hire?
- **Geopolitical factors** — trade policy, cross-border data regulations

### Step 7: Verification Pass

Before writing up:
- Run the Interview Test on key claims
- Check negative claims
- Ensure every quantitative claim shows methodology and source
- Distinguish clearly between reported data and inferences

### Step 8: Write Up

Synthesise following the output template in `references/output-templates.md` (Market Landscape), or adapt to your preferred format. For each force and trend: state the finding, provide evidence, assess the implication, and note confidence level.

### Limitations

- Google Trends and forum analysis require Chrome for the richest signals
- Regulation tracking is UK-focused by default; other jurisdictions need explicit scoping
- Market sizing for nascent or niche markets often produces wide ranges — show your methodology
- Demand classification is a judgement call, not a binary — present the evidence and let the reader calibrate

### Conciseness

Target 1,500–2,500 words. Porter's Five Forces should be specific to this market, not generic textbook answers. If a force isn't particularly interesting, keep it to 1–2 sentences rather than padding.
