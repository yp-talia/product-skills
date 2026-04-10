---
name: research-competitors
version: "1.0"
description: >
  Analyse a company's competitive landscape — identify direct, strategic, and adjacent competitors, compare features, pricing, audiences, distribution, and brand perception, and flag underserved segments. Trigger whenever the user wants to understand a company's competition, compare competitors, do a competitive analysis, identify market gaps, or assess competitive positioning.
---

# Research Competitors

Produce a structured competitive analysis: who else operates in this space, how they differentiate, where the gaps are. This skill goes beyond listing competitors — it assesses strategic positioning, audience segmentation, and identifies underserved opportunities.

## Required Tools

- **WebSearch** — competitor identification, feature comparisons, pricing, funding data
- **WebFetch** — competitor websites, pricing pages, feature pages, comparison articles

## Recommended Tools

- **Claude in Chrome** — G2/Capterra comparison pages, competitor product demos, detailed review sites, SimilarWeb traffic analysis, BuiltWith tech stack detection. If unavailable, note which comparisons are based on publicly available data only.

## Source Rules

Read `references/source-and-triangulation.md` before beginning. Revenue/funding claims need triangulation. Feature availability claims should be checked against multiple sources (marketing pages often differ from user reviews). Pricing must note date accessed.

### Inline Citation Requirement

**CRITICAL**: Every factual statement in the output MUST have its source placed immediately next to the specific claim. See `references/source-and-triangulation.md` for full citation rules.

### Currency

Report all financial figures in their original currency. Do not convert. If a comparison requires normalisation, show both currencies with the exchange rate and date used.

### Source Integrity

Never cite a URL you have not fetched and read in this session. Never invent article titles, author names, or publication dates. If you cannot find a source for a claim, either state the claim is unverified or remove it entirely.

### Review Platform Accuracy

When reporting ratings from Trustpilot, Glassdoor, G2, Capterra, or app store reviews, fetch the actual page and report the exact numbers shown. Do not estimate or recall from memory.

## Research Steps

### Step 1: Identify Competitors

Build a comprehensive competitor map across three categories:

**Direct competitors** — same product category, same customer segment:
- Search for "[company name] alternatives" and "[company name] competitors"
- Check G2/Capterra competitor lists
- Look at industry analyst reports
- Check the company's own comparison pages

**Strategic competitors** — different approach to the same underlying problem:
- Think about what job the customer is hiring the product to do
- Who else helps customers accomplish that job, even with a very different product?

**Adjacent competitors** — companies that could expand into this space:
- Large platforms with related capabilities
- Companies in adjacent markets with overlapping customer bases
- Well-funded startups in related spaces

### Step 2: Deep-Dive Direct Competitors

For each direct competitor (top 3–5), research:

- **Product**: Key features, main differentiators, product maturity
- **Pricing**: Model, tiers, price points, enterprise approach
- **Target audience**: Company size, industry, user persona
- **Revenue & scale**: Funding, estimated revenue, employee count, customer count
- **Brand perception**: Strengths and weaknesses per reviews
- **Distribution**: PLG, sales-led, partnerships, content

### Step 3: Feature Comparison Matrix

Build a feature-by-feature comparison table — one of the highest-value outputs.

Guidelines:
- Include only features that matter for differentiation (skip table-stakes)
- Use ✅ / ❌ / 🟡 (partial) where you have clear evidence
- Use ❓ where you couldn't determine availability
- Note your source for each feature claim
- Focus on 8–15 differentiating features

**Verification matters.** For each ✅ or ❌, make sure you have at least one source beyond the company's own marketing page. If you can't verify, use ❓ rather than guessing.

### Step 4: Audience & Segmentation

For each direct competitor, map:
- **Primary audience**: Best customers by company size, industry, geography
- **Use case focus**: What specific use case they optimise for
- **Positioning**: How they describe themselves (taglines, homepage, G2 category)
- **Customer profiles**: What case studies and testimonials reveal

Look for patterns: are all competitors targeting the same segment, or is the market segmented?

### Step 5: SimilarWeb Traffic Analysis

Using Chrome (if available), visit SimilarWeb for the target company and each direct competitor. For each site, capture:

- **Total monthly visits** and trend
- **Traffic sources breakdown** — direct, organic, paid, social, referral, email
- **Top organic keywords** — positioning and demand signals
- **Top referral sources** — partnership signals
- **Geographic distribution**
- **Bounce rate and pages per visit**

Build a comparative traffic table across competitors.

### Step 6: Technology Stack Comparison

Using Chrome (if available), visit **BuiltWith** for each direct competitor. Compare:

- **Frontend framework**
- **Analytics & experimentation**
- **Hosting & infrastructure**
- **Payment processing**
- **Marketing & CRM**

Look for patterns: shared infrastructure (industry standard), experimentation maturity, technology generation, analytics sophistication.

### Step 7: Distribution & Marketing

Compare how competitors reach customers:
- **PLG signals**: Free tier, self-serve sign-up, usage-based pricing
- **Sales-led signals**: "Book a demo" CTAs, enterprise sales teams
- **Content marketing**: Blog quality and frequency, SEO presence
- **Partnerships**: Channel partners, marketplace listings
- **Community**: Developer communities, user forums, events

### Step 8: Brand Perception, Sentiment & Trust Signals

#### Review Volume as Market Signal

Note the **volume** of reviews for each competitor across platforms. This is itself a powerful signal:
- Low review volume across the entire category = likely a demand generation market
- Compare review volume to SimilarWeb traffic — high traffic but few reviews suggests a conversion problem

#### Sentiment Theme Extraction

Using Chrome (if available), read actual review text across Trustpilot, Google Reviews, and relevant platforms. For each competitor, extract:
- **Top 3-5 positive themes**
- **Top 3-5 negative themes**
- **Emotional language patterns** — crisis/urgency language vs planning/proactive language

#### Trust Signals

Research for each competitor:
- Social proof, case studies, industry awards
- Regulatory accreditations, professional qualifications
- Endorsement signals (Which? recommended, partnership badges)

### Step 9: Pricing & Revenue Comparison

Build a comparison table:

| Competitor | Pricing Model | Entry Price | Mid-Tier | Enterprise | Revenue Signals |
|-----------|--------------|------------|---------|-----------|----------------|

Note the date of all pricing research.

### Step 10: Identify Underserved Segments

Based on all research:
- Is there a customer segment no competitor serves well?
- Is there a use case poorly addressed?
- Is there a geographic market underserved?
- Is there a price point gap?
- Are there emerging customer needs no competitor has addressed?

Support each observation with evidence.

### Step 11: Verification Pass

Before writing up:
- Run the Interview Test on feature claims
- Check negative claims about competitors
- Verify pricing data is current

### Step 12: Write Up

Synthesise following the output template in `references/output-templates.md` (Competitor Analysis), or adapt to your preferred format. The comparison matrix and underserved segments sections are the highest-value outputs.

### Limitations

- Feature comparison accuracy depends on source quality; marketing pages often overstate capability
- Pricing changes frequently — always note the access date
- Private company revenue and customer counts are estimates at best
- SimilarWeb and BuiltWith require Chrome for reliable access
- Emerging competitors may not yet appear in analyst reports or comparison sites

### Conciseness

Target 1,500–2,500 words. Keep competitor deep-dives focused on what differentiates them rather than repeating their "About us" page.
