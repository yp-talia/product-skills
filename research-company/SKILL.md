---
name: research-company
version: "1.0"
description: >
  Research a company's background, financials, culture, growth model, and technology landscape from multiple external perspectives. Trigger whenever the user wants to research a company, understand a company, do due diligence on a company, or learn about a company before an interview, meeting, or partnership discussion. Also trigger when the user says things like 'tell me about [company]', 'research [company]', 'what do we know about [company]', 'dig into [company]', or 'company intel on [company]'.
---

Build a comprehensive intelligence profile of a company from multiple external perspectives. This skill produces a structured output covering what the company does, how it grows, what technology underpins it, its financial health, and what different stakeholders say about it.

## Required Tools

- **WebSearch** — news, press, investor mentions, tech stack signals
- **WebFetch** — company website, blog, specific URLs, Companies House

## Recommended Tools

- **Claude in Chrome** — Glassdoor reviews, Google Reviews, Trustpilot (where login walls or dynamic content block WebFetch). If unavailable, note which perspectives are missing from the output rather than silently degrading.

## Source Rules

Read `references/source-and-triangulation.md` before beginning research. Every factual claim must be cited. Company self-reported information (their website, socials) is treated as true. External claims about the company need triangulation where specified.

### Inline Citation Requirement

**CRITICAL**: Every factual statement in the output MUST have its source placed immediately next to the specific claim — not grouped at the end of a section, paragraph, or profile. The reader must be able to verify any individual statement without hunting for its source.

**Format**: `[Claim text]. [Source: Name, URL, accessed YYYY-MM-DD]`

**Rules**:
1. Every individual factual statement gets its own inline citation
2. If two consecutive facts come from the same source, still cite each one (you can abbreviate: `[Source: same]`)
3. If a claim is your inference rather than a sourced fact, label it: `[Inference based on: ...]`
4. Never write a paragraph of facts and then put a list of sources at the end
5. This rule applies to ALL content — including tables, bullet points, and narrative prose

### Currency

Report all financial figures in their original currency. Do not convert. If a comparison requires normalisation, show both currencies with the exchange rate and date used.

### Source Integrity

Never cite a URL you have not fetched and read in this session. Never invent article titles, author names, or publication dates. If you cannot find a source for a claim, either state the claim is unverified or remove it entirely.

### Review Platform Accuracy

When reporting ratings from Trustpilot, Glassdoor, G2, or similar platforms, fetch the actual page and report the exact numbers shown (overall rating, review count, recommendation percentage). Do not estimate or recall from memory — these numbers change frequently and errors here are immediately visible to anyone who checks.

## Research Steps

### Step 1: Company's Own Voice

Search for and read the company's website. Focus on:
- **About page** — what they do, founding story, team
- **Mission/Values page** — stated purpose and principles
- **Blog** — recent posts, topics they care about, company announcements
- **Careers page** — open roles (signals growth areas and priorities), culture messaging. Check the careers page thoroughly: many companies host job listings on external ATS platforms (Lever, Greenhouse, Workable, Ashby) accessible via a subdomain or separate URL linked from the careers page. Also check LinkedIn Jobs and at least one job board (Indeed, Otta, Welcome to the Jungle) as a cross-reference
- **Social media** — LinkedIn company page, Twitter/X, any other active channels
- **Website footer** — capture the registered company name, company number, and registered address. UK companies are legally required to display this. You will need the company number for Step 6a.

This is Tier 1 information. Treat it as true. Record it faithfully.

### Step 2: News & Press

Search for recent news coverage, prioritising the last 12 months (extend to 24 months if coverage is sparse):
- Funding announcements
- Product launches or pivots
- Leadership changes
- Partnerships or acquisitions
- Industry recognition or awards
- Any negative press (lawsuits, controversies, failures)

### Step 3: Investor Perspective

Search for:
- Funding history — rounds, amounts, investors, valuations where available
- Investor portfolio pages — how the investor describes this company
- Investor commentary — blog posts, interviews, tweets about this company
- Crunchbase profile for structured funding data

### Step 4: Employee Sentiment

Using Chrome (if available), visit Glassdoor (or equivalent) and research:
- Overall rating and trend (improving or declining?)
- Pros and cons patterns across reviews
- Management and leadership feedback
- Work-life balance signals
- Any mentions of product team specifically

Also search LinkedIn for employee posts mentioning the company — both current and former employees.

### Step 5: Customer Sentiment

Search across multiple review platforms:
- **Which?** — if the company operates in a consumer space Which? covers
- **Google Reviews** — via Chrome if available
- **reviews.io** — via WebSearch/WebFetch
- **Trustpilot** — via Chrome or WebSearch
- **G2 / Capterra** — if B2B SaaS
- **App store reviews** — if they have a mobile app
- **Social media mentions** — Twitter/X, Reddit discussions

Look for patterns, not individual reviews. What do customers consistently praise or complain about?

### Step 6: Financial Signals

Research financial health through:
- **Companies House** (if UK company) — see **Step 6a** below for the correct lookup procedure. This is mandatory for UK companies — do not skip it or use a shortcut
- **Crunchbase** — funding data, employee count estimates
- **LinkedIn** — headcount trends (growing, stable, shrinking?)
- **Press** — revenue mentions, growth claims
- **Job postings volume** — lots of hiring = growth; sudden job removal = potential cuts. Check the company's own careers page, LinkedIn Jobs, and at least one external job board. Do not claim "the company is not hiring" based on a single source

Triangulate financial health claims across at least 2 sources.

#### Step 6a: Companies House Lookup (UK Companies — MANDATORY PROCEDURE)

**CRITICAL**: Do NOT search Companies House by company name alone. Trading names frequently differ from registered names (e.g. "amicable" is registered as "E-Negotiation Ltd"). Name-based searches regularly return the wrong entity, producing completely misleading financial and director data. Follow this exact procedure:

**Route 1 — Company number from website (preferred)**:

1. In Step 1, you should have captured the company number from the website footer.
2. If you have a company number, go directly to `https://find-and-update.company-information.service.gov.uk/company/{NUMBER}` — this is the only reliable lookup method.
3. Capture: company status, registered address, filing history, accounts summary, and any recent officer changes.

**Route 2 — No company number found (fallback)**:

1. If the website footer doesn't contain a company number (also check Terms & Conditions, Privacy Policy, and Legal pages), search Companies House by the company's trading name.
2. **You MUST verify any match** before using the data. Navigate to the "People" tab for the entity you found and cross-reference the listed directors/officers against the company's known leadership. If the directors don't match the known leadership, **you have the wrong company** — stop and try alternative names.
3. If you cannot confidently match the entity, state this explicitly: "Could not confidently identify the correct Companies House entity. The trading name differs from the registered name." Do NOT report data from an unverified entity.

**Common pitfalls to avoid**:
- Many companies with similar names exist — always verify via directors
- A registered address in a different city from the company's known HQ is a red flag
- An "active proposal to strike off" flag on an otherwise healthy company is another red flag — verify before reporting

### Step 7: SimilarWeb Traffic Profile

Using Chrome (if available), visit SimilarWeb (similarweb.com) for the company's website. Capture:

- **Total monthly visits** and trend over last 6–12 months
- **Traffic sources breakdown** — direct, organic search, paid search, social, referral, email
- **Top organic keywords** — reveals what customers search for to find them
- **Top referral sources** — partnership and media signals
- **Geographic distribution** — where users are concentrated
- **Bounce rate and pages per visit** — engagement quality signals

If SimilarWeb data is unavailable (common for early-stage startups), note this — it's itself a useful signal about scale.

### Step 8: Growth Model & Distribution

Research how the company acquires customers:
- **Job postings** — are they hiring salespeople, growth engineers, content marketers, partnerships managers? This reveals the go-to-market model
- **Marketing presence** — content marketing, paid advertising signals, SEO footprint, social media strategy
- **Partnerships** — announced distribution partnerships, channel partners
- **Product signals** — referral programmes, freemium tiers, self-serve sign-up (PLG signals)
- **Case studies** — how customers found them, sales cycle evidence

Synthesise into a clear picture: is this company PLG, sales-led, partnership-driven, content-driven, or a hybrid?

### Step 9: Technology Landscape

Research the technical foundation using both passive research and active detection.

#### 9a: BuiltWith / Wappalyzer Detection

Using Chrome (if available), visit **BuiltWith** (builtwith.com) for the company's website. Capture:

- **Frontend frameworks** — React, Angular, Vue, Next.js, etc.
- **Analytics & tracking** — Google Analytics, Mixpanel, Amplitude, Segment, Hotjar, etc.
- **Hosting & CDN** — AWS, GCP, Azure, Cloudflare, Vercel, etc.
- **Payment processing** — Stripe, PayPal, GoCardless, etc.
- **Marketing & CRM tools** — HubSpot, Salesforce, Intercom, Mailchimp, etc.
- **A/B testing & experimentation** — Optimizely, LaunchDarkly, VWO, etc.
- **Error monitoring & performance** — Sentry, Datadog, New Relic, etc.
- **Chat & support** — Intercom, Zendesk, Drift, etc.

If BuiltWith data is sparse, also try **Wappalyzer** (wappalyzer.com) as a cross-reference.

#### 9b: Job Postings & Engineering Signals

Complement the detection data with qualitative research:
- **Job postings** — required tech skills reveal the backend stack
- **Engineering blog** — technical posts, architecture decisions, migration stories
- **GitHub** — open source contributions, public repos
- **StackShare** — self-reported tech stack
- **Conference talks** — engineers speaking about their systems

#### 9c: Technology Assessment

Synthesise into a strategic assessment:

- **Stack modernity** — modern vs legacy signals
- **Experimentation capability** — A/B testing tooling presence or absence
- **Data infrastructure** — analytics and tracking maturity
- **Technical debt signals** — job postings mentioning migrations or re-architecture
- **Build vs buy posture** — third-party services vs custom-built solutions

### Step 10: Synthesise

Write up all findings following the output template in `references/output-templates.md` (Company Intelligence), or adapt to your preferred format. The most important section is the **Multi-Perspective Analysis** — comparing what the company says about itself vs what investors, employees, customers, and press say. Flag misalignments prominently.

### Step 11: Verification Pass

Before writing up, review every claim through two lenses:

1. **The Interview Test**: Imagine someone stating this claim in a meeting with an insider. Could they easily contradict it? If yes, either verify more thoroughly, soften the language, or flag uncertainty.

2. **Negative claim audit**: Scan for any claims about things that don't exist or aren't happening. For each one, confirm you checked at least 3 sources. If not, rephrase as "could not confirm" rather than "does not exist".

### Step 12: Flag Misalignments & Changes Over Time

End the output with:
- Any contradictions between perspectives
- Any significant changes over time (e.g. Glassdoor sentiment declining, or a strategic pivot visible in blog posts)
- Information gaps where you couldn't find data despite trying

### Limitations

- Companies with minimal press coverage or very early stage produce thin results
- Employee sentiment (Glassdoor) requires Chrome for reliable access
- Companies House data only covers UK-registered entities
- SimilarWeb data is unavailable for low-traffic sites
- Financial data for private companies is inherently limited — estimates should be flagged as such

### Conciseness

Target 1,500–2,500 words. Lead with insights that would change how someone thinks about the company. Deprioritise information easily found on page 1 of the company website.
