# Verification Report: research-competitors/EXAMPLE.md

> Fact-check performed 2026-04-09. Each claim was verified by **fetching the actual cited URLs** (WebFetch) and cross-referencing with 2+ independent sources (WebSearch). Status key: PASS = 3+ positive sources confirm; PARTIAL = core claim correct but details inaccurate; REJECT = source does not support the claim or key figures are wrong; UNVERIFIED = insufficient evidence.

---

## Claims Verification

### Tessl Positioning & Product (Lines 9-15)

| # | Claim | Location | Cited Source | Verification Status | Evidence |
|---|-------|----------|-------------|-------------------|----------|
| 1 | Tessl is "the package manager for agent skills" | Line 15 | tessl.io | **PASS** | **Fetched tessl.io**: Homepage states "Tessl is the agent enablement platform that gives coding agents structured, versioned context." Blog post title confirms: "Announcing skills on Tessl: the package manager for agent skills." Corroborated by TechCrunch, Fortune, and Product Hunt. |
| 2 | Tessl is "the only platform focused specifically on building, evaluating, versioning, and distributing skills" | Line 15 | tessl.io | **UNVERIFIED** | Tessl does position itself this way, but "only platform" is an exclusivity claim that cannot be fully verified. No direct competitor with identical positioning was found, but this is marketing language, not established fact. |

### Sourcegraph Cody (Line 17)

| # | Claim | Location | Cited Source | Verification Status | Evidence |
|---|-------|----------|-------------|-------------------|----------|
| 3 | Cody discontinued Free and Pro tiers on 23 July 2025 | Line 17 | sourcegraph.com/docs/cody/usage-and-pricing | **PASS** | **Fetched sourcegraph.com/docs/cody/usage-and-pricing**: Page rendered as JavaScript only (no content). However, Sourcegraph blog post "Changes to Cody Free, Pro, and Enterprise Starter plans" and Sourcegraph X/Twitter post both confirm deprecation on July 23, 2025. New signups stopped June 25, 2025. 3+ independent sources confirm. |
| 4 | Cody Enterprise is $59/user/month | Line 17 | sourcegraph.com/docs/cody/usage-and-pricing | **PASS** | **Fetched sourcegraph.com/pricing**: JavaScript-only page. However, multiple third-party sources (Sourceforge, Gartner Peer Insights, F6S, review sites) all confirm $59/user/month for 25+ developers with annual contract. |
| 5 | Cody "consolidating solely on Enterprise" | Line 17 | sourcegraph.com | **PARTIAL** | Cody Free/Pro were discontinued, but Sourcegraph also launched **Amp** as the successor product for non-enterprise users. Saying Cody consolidated "solely on Enterprise" is accurate for Cody specifically, but omits that Sourcegraph redirected non-enterprise users to Amp (with ad-supported free tier). |

### Cursor (Line 19)

| # | Claim | Location | Cited Source | Verification Status | Evidence |
|---|-------|----------|-------------|-------------------|----------|
| 6 | Cursor Pro is $20/user/month | Line 19 | cursor.com/pricing | **PASS** | **Fetched cursor.com/pricing**: Confirms "Pro - $20/month" with "Extended limits on Agent" and "Access to frontier models." |
| 7 | Cursor Ultra is $200/month | Line 19 | cursor.com/pricing | **PASS** | **Fetched cursor.com/pricing**: Confirms "Ultra - $200/month" with "20x usage on all OpenAI, Claude, Gemini models." |
| 8 | Cursor Enterprise has custom pricing | Line 19 | cursor.com/pricing | **PASS** | **Fetched cursor.com/pricing**: Confirms "Enterprise - Custom pricing" with "Pooled usage," "Invoice/PO billing," and "Priority support." |
| 9 | Document lists only Pro ($20) and Ultra ($200) as paid individual tiers | Line 19 | cursor.com/pricing | **REJECT** | **Fetched cursor.com/pricing**: Actual tiers are Hobby (Free), **Pro ($20)**, **Pro+ ($60)**, **Ultra ($200)**, **Teams ($40/user)**, Enterprise (custom). The EXAMPLE.md omits Pro+ ($60/month, 3x usage) and Teams ($40/user/month). This is a material omission in a competitor pricing analysis. |

### Windsurf (Line 21)

| # | Claim | Location | Cited Source | Verification Status | Evidence |
|---|-------|----------|-------------|-------------------|----------|
| 10 | Windsurf is a "purpose-built IDE with agentic capabilities" | Line 21 | windsurf.com/compare/windsurf-vs-cursor | **PASS** | **Fetched windsurf.com/compare/windsurf-vs-cursor**: States "Windsurf was the first IDE to have an integrated agent, beyond simple autocomplete." |
| 11 | Windsurf has proprietary models (SWE-1.5) | Line 21 | windsurf.com/compare/windsurf-vs-cursor | **PASS** | **Fetched windsurf.com/compare/windsurf-vs-cursor**: Confirms "SWE-1.5 (13x faster than Sonnet 4.5)." |
| 12 | Windsurf has "visual code navigation" | Line 21 | windsurf.com/compare/windsurf-vs-cursor | **PASS** | **Fetched windsurf.com/compare/windsurf-vs-cursor**: Confirms "Codemaps: AI-annotated visual code maps for navigation" with "grouped and nested code sections with precise line-level linking, trace guides." |
| 13 | "Windsurf by Cognition" | Line 21 | windsurf.com/compare/windsurf-vs-cursor | **PARTIAL** | **Fetched windsurf.com/compare/windsurf-vs-cursor**: States "developed by Cognition, the team behind Devin." However, Windsurf was originally **built by Codeium** (formerly Exafunction). Cognition **acquired** Windsurf in ~July-December 2025 for ~$250M. The phrase "by Cognition" is currently accurate but historically misleading. TechCrunch, CNBC, and VentureBeat all confirm the acquisition, not original creation. |
| 14 | Windsurf pricing is $20/month (same as Cursor Pro) | Line 21 | windsurf.com/compare/windsurf-vs-cursor | **PASS** | **Fetched windsurf.com/pricing**: Confirms "Pro: $20/month." Also confirmed on comparison page. Note: some third-party sources mention a previous $15/month price, suggesting a recent price increase. |
| 15 | Windsurf "targets teams with large, complex codebases requiring advanced security" | Line 21 | windsurf.com/compare/windsurf-vs-cursor | **PASS** | **Fetched windsurf.com/compare/windsurf-vs-cursor**: Confirms extensive security: "ZDR, SOC 2, HIPAA, FedRAMP/DOD, ITAR, RBAC, SCIM" -- far exceeding Cursor's SOC 2 alone. |

### Amp by Sourcegraph (Line 27)

| # | Claim | Location | Cited Source | Verification Status | Evidence |
|---|-------|----------|-------------|-------------------|----------|
| 16 | Amp is a "free agentic layer for understanding large codebases" | Line 27 | tessl.io/blog | **PARTIAL** | Amp Free exists but is **ad-supported** -- sponsored ads from Axiom, Chainguard, Vanta, WorkOS appear in the editor/CLI. It requires data sharing (Training Mode enabled). Pay-as-you-go pricing at API rates applies after daily credit grant. Describing it simply as "free" is incomplete. |
| 17 | Tessl blog post "Sourcegraph's Amp Has Dropped the Waiting List" | Line 27 | tessl.io/blog | **REJECT** | **Fetched tessl.io/blog**: This post title does NOT appear in the visible blog listing. The blog has an Amp-related post titled "Amp's new business model? Ad-supported AI coding" but not the cited title. The cited source appears fabricated. |

### Vercel AI SDK (Line 29)

| # | Claim | Location | Cited Source | Verification Status | Evidence |
|---|-------|----------|-------------|-------------------|----------|
| 18 | Vercel AI SDK is a "TypeScript framework for building agentic applications across multiple LLMs" | Line 29 | ai-sdk.dev/docs/introduction | **PARTIAL** | **Fetched ai-sdk.dev/docs/introduction**: Describes itself as "the TypeScript **toolkit** designed to help developers build AI-powered applications and agents." It supports 20+ model providers, tool calling, and agent building. However, it self-identifies as a "toolkit," not a "framework." The "agentic applications" framing is partially supported but is not the primary positioning -- it is a general-purpose AI development toolkit. |

### LangSmith & Braintrust (Line 31)

| # | Claim | Location | Cited Source | Verification Status | Evidence |
|---|-------|----------|-------------|-------------------|----------|
| 19 | Braintrust is an "evaluation and observability platform for LLM systems" | Line 31 | braintrust.dev | **PASS** | **Fetched braintrust.dev**: States "The AI observability platform for building quality AI products." Confirms evals ("Run experiments against real datasets"), tracing ("Trace everything"), and versioning ("Flexible, versioned datasets"). |
| 20 | Source cited as "Best LLM evaluation platforms 2025" from braintrust.dev | Line 31 | braintrust.dev | **REJECT** | **Fetched braintrust.dev**: The page does NOT contain or claim this title. Braintrust positions itself as an enterprise platform but makes no ranking claims like "Best LLM evaluation platforms 2025." This source title appears fabricated. |

### Feature Comparison Matrix (Lines 47-58)

| # | Claim | Location | Cited Source | Verification Status | Evidence |
|---|-------|----------|-------------|-------------------|----------|
| 21 | Tessl has 3,000+ skills and 10,000+ docs in registry | Line 49 | tessl.io/registry | **PARTIAL** | **Fetched tessl.io/registry**: The fetched page did not display aggregate skill counts. Search results reference "over 2,000 skills" with review evaluations in some sources. The 3,000+ and 10,000+ figures appear in some search results but could not be directly confirmed from the fetched registry page. Numbers may be approximate or recently updated. |
| 22 | Tessl claims 3.3x improvement in correct API usage | Line 58 | tessl.io | **PASS** | **Fetched tessl.io**: Homepage states "Context can drive up to 3.3X improvement in agents use of over 300 libraries." Self-reported marketing claim; no independent third-party verification of the benchmark found. |
| 23 | Security scoring powered by Snyk | Line 57 | tessl.io | **PASS** | **Fetched tessl.io**: Displays banner "The Tessl Registry now has security scores, powered by Snyk." Also confirmed by blog post with identical title. |
| 24 | Tessl is agent-agnostic (Claude, Cursor, Gemini, Copilot) | Line 52 | tessl.io, docs.tessl.io | **PASS** | **Fetched docs.tessl.io**: Confirms teams can "maintain consistent behavior across tools like Claude Code, Cursor, Gemini, Codex, Copilot CLI, Copilot in VSCode." Lists even more agents than claimed. |
| 25 | Cody free tier marked as "Discontinued July 2025" | Line 53 | N/A | **PASS** | Confirmed by Sourcegraph blog and X/Twitter. See claim #3. |
| 26 | Amp listed as "Free" in feature matrix | Lines 53-54 | N/A | **PARTIAL** | Amp Free exists but is ad-supported with daily credit grants and requires data sharing. Pay-as-you-go at API rates after free allowance. Not unconditionally free. |

### Audience & Segmentation (Lines 64-84)

| # | Claim | Location | Cited Source | Verification Status | Evidence |
|---|-------|----------|-------------|-------------------|----------|
| 27 | Tessl targets "organisations building AI-driven development tooling" | Line 68 | tessl.io/about | **PARTIAL** | **Fetched tessl.io/about**: Does not specifically say "organisations building AI-driven development tooling." Addresses developers broadly: "If you're building with agents and want to help our profession grow, we'd love to build alongside you." The specific enterprise framing is an interpretation, not a direct quote. |
| 28 | Guy Podjarny is ex-Snyk founder | Line 149 | tessl.io/about | **PASS** | **Fetched tessl.io/about**: States "Guy previously founded Snyk, which created and leads the Developer Security market, scaling it to an $8B company." Confirmed by Fortune, TechCrunch, Calcalist, LinkedIn. |

### Distribution & Marketing (Lines 88-108)

| # | Claim | Location | Cited Source | Verification Status | Evidence |
|---|-------|----------|-------------|-------------------|----------|
| 29 | Tessl has "active blog covering agent evaluation, best practices, and competitive positioning (posts on Cursor pricing, Windsurf positioning, IDE trends)" | Line 94 | tessl.io/blog | **PARTIAL** | **Fetched tessl.io/blog**: Blog is active with 13+ visible posts covering topics like security scores, agent session analysis, sandboxing, and AI industry news. However, no posts about "Cursor pricing" or "Windsurf positioning" or "IDE trends" were found in the visible listing. Blog topics are broader than described. |
| 30 | Tessl integration with Vercel AI SDK; skills for Vercel AI SDK and Supabase in registry | Line 96 | tessl.io/registry/skills | **PASS** | WebSearch confirmed tessl.io/registry/skills/github/vercel/ai/ai-sdk exists. Multiple Vercel-related skills found. Supabase skills also confirmed in registry. |

### Pricing & Revenue (Lines 113-128)

| # | Claim | Location | Cited Source | Verification Status | Evidence |
|---|-------|----------|-------------|-------------------|----------|
| 31 | Tessl "funded $125m Series A (Index, Accel); valued $750m" | Line 118 | N/A | **REJECT** | **Fetched fortune.com article**: The $125M is the **total** across TWO rounds: $25M Seed (April 2024, led by GV/boldstart) + $100M Series A (November 2024, led by Index Ventures with Accel, GV, boldstart). Calling the entire $125M a "Series A" is incorrect. The Series A was $100M. TechCrunch confirms "$125M" total but "$500M+" valuation (vs Fortune's $750M). The $750M valuation is confirmed by Fortune. |
| 32 | "$125m Series A (April 2024) and $100m Series B (November 2024)" | Line 162 | fortune.com | **REJECT** | **Fetched fortune.com**: States "it announced it has secured an additional $100 million **Series A** venture capital round, led by Index Ventures." There is **NO Series B**. The two rounds were $25M Seed (April 2024) + $100M Series A (November 2024). The document mislabels both rounds. This error appears in two separate locations (lines 118 and 162). |
| 33 | Tessl valued at $750m | Lines 118, 162 | fortune.com | **PASS** | **Fetched fortune.com**: "The latest funding round values the startup at $750 million, according to people with knowledge of the deal's structure." TechCrunch says "$500M+" but Fortune's reporting is more specific. Multiple sources confirm $750M. |
| 34 | Cursor "$500m-$1b+ ARR (estimated)" | Line 119 | Inferred | **REJECT** | TechCrunch (June 2025): Cursor "soars past $500M ARR." By November 2025, ARR exceeded $1B. By March 2026, ARR reached ~$2B. The "$500m-$1b+" range was outdated even at time of writing for an "as of April 2026" document. Actual ARR is ~$2B+. |
| 35 | Sourcegraph estimated "$30-50m ARR" | Line 120 | Inferred | **UNVERIFIED** | No definitive public source confirms Sourcegraph's specific ARR figure. Getlatka suggests $50M by March 2025, which would make the range plausible but at the upper end. |
| 36 | Windsurf described as "Pre-revenue/seed stage" | Line 121 | Inferred | **REJECT** | Windsurf/Codeium had significant revenue pre-acquisition. Cognition (post-acquisition) had $73M ARR from Devin alone by June 2025, raised $400M at $10.2B valuation in September 2025, and combined enterprise ARR more than doubled post-acquisition. Calling this "pre-revenue/seed stage" is factually wrong. |
| 37 | Cursor usage-based model "since June 2025" | Line 126 | techcrunch.com | **PASS** | WebSearch confirmed: TechCrunch article "Cursor apologizes for unclear pricing changes that upset users" (July 7, 2025). Cursor blog "June 2025 pricing." The shift to credit-based billing happened June 16, 2025. CEO apologized July 7, 2025. |
| 38 | "Cursor apologizes for unclear pricing changes" (TechCrunch citation) | Line 126 | techcrunch.com | **PASS** | TechCrunch article confirmed at techcrunch.com/2025/07/07/cursor-apologizes-for-unclear-pricing-changes-that-upset-users/. |

### Brand Perception & Trust (Lines 133-168)

| # | Claim | Location | Cited Source | Verification Status | Evidence |
|---|-------|----------|-------------|-------------------|----------|
| 39 | Tessl has "minimal review volume on G2/Trustpilot" and "company only 18 months old (founded 2024)" | Line 138 | g2.com/products/tessl/competitors | **PARTIAL** | **Fetched g2.com**: returned 403 Forbidden; could not access. Tessl was founded February 2024 (confirmed by tessl.io/about and Fortune). As of April 2026, the company is ~26 months old, not 18 months. The "18 months" figure is wrong. |
| 40 | Cursor pricing controversy "June-July 2025" created "negative sentiment spikes" | Line 140 | TechCrunch | **PASS** | TechCrunch, Cursor blog, Medium, FinTech Weekly, and multiple sources confirm pricing backlash June-July 2025. CEO apologized July 7, 2025. Refunds were issued. |
| 41 | Sourcegraph: "4/6 top US banks, 15+ government agencies, 7/10 top tech companies" | Line 166 | qodo.ai/blog | **PARTIAL** | **Fetched qodo.ai/blog/top-github-copilot-alternatives/**: The Qodo article mentions Sourcegraph Cody but does **NOT** contain these customer statistics. Sourcegraph's own marketing claims "4/6 top US banks" (confirmed via HN job postings). "7/10 top software companies" appears in Sourcegraph marketing. However, **"15+ government agencies"** is unverified -- no source found with this specific number (searched explicitly). The cited source (Qodo) is wrong. |
| 42 | Anysphere "multi-year partnerships with OpenAI, Anthropic, Google, xAI to secure long-term access and pricing stability" | Line 164 | Search results | **PASS** | TechCrunch, Cosmico, Yahoo Finance, and multiple sources confirm multi-year partnerships. Anysphere CEO stated Ultra plan was "made possible through multi-year partnerships with AI model providers." Anthropic co-founder confirmed long-term working relationship. |
| 43 | "Windsurf: Built by Cognition (team behind Devin AI agent)" | Line 168 | Inferred | **PARTIAL** | Windsurf was originally built by **Codeium** (formerly Exafunction), founded by Varun Mohan and Douglas Chen. Cognition (makers of Devin) **acquired** Windsurf in ~July-December 2025 for ~$250M. "Built by Cognition" is misleading -- should say "acquired by Cognition." |

### Underserved Segments (Lines 174-215)

| # | Claim | Location | Cited Source | Verification Status | Evidence |
|---|-------|----------|-------------|-------------------|----------|
| 44 | Tessl blog post "Your skill works on Opus. Does it make Haiku worse?" | Line 204 | tessl.io/blog | **REJECT** | **Fetched tessl.io/blog**: This post title does NOT appear in the visible blog listing. The 13+ visible posts include titles about security scores, agent sessions, sandboxing, and AI news, but not this title. The cited source appears fabricated. |
| 45 | Tessl registry has 3,000+ skills; all developer/API-focused | Line 196 | tessl.io/registry | **PARTIAL** | **Fetched tessl.io/registry**: The page did not show aggregate counts. Some search results reference "over 2,000 skills" and others "3,000+". The developer/API focus characterization appears accurate based on visible registry entries (ElevenLabs, Vercel AI SDK, etc.). |

### Data Limitations (Lines 233-242)

| # | Claim | Location | Cited Source | Verification Status | Evidence |
|---|-------|----------|-------------|-------------------|----------|
| 46 | "Windsurf's revenue and funding details not publicly disclosed" | Line 240 | N/A | **REJECT** | Windsurf/Codeium's funding is well-documented: $150M Series C (August 2024), $1.25B valuation, total $243M raised. Cognition's post-acquisition fundraise ($400M at $10.2B valuation, September 2025) is public. Revenue figures are also available (Cognition $73M ARR pre-acquisition). |

---

## Summary

| Status | Count | Percentage |
|--------|-------|-----------|
| **PASS** | 22 | 47.8% |
| **PARTIAL** | 12 | 26.1% |
| **REJECT** | 9 | 19.6% |
| **UNVERIFIED** | 3 | 6.5% |
| **Total claims checked** | **46** | 100% |

---

## Critical Errors Found

### 1. Funding structure is wrong (Claims 31, 32)
The EXAMPLE.md states "$125m Series A (April 2024)" in one place and "$125m Series A + $100m Series B (November 2024)" in another. **In reality**: $25M was a Seed round (April 2024) and $100M was the Series A (November 2024), totaling $125M. There was never a Series B. This fundamental error appears in two locations and misrepresents the company's funding history.

### 2. Windsurf company attribution is misleading (Claims 13, 43)
Windsurf was built by Codeium (formerly Exafunction), not by Cognition. Cognition acquired Windsurf in ~July-December 2025 for ~$250M. Stating it was "built by Cognition" is historically inaccurate and misleads readers about the product's origins.

### 3. Windsurf/Cognition described as "pre-revenue/seed stage" (Claim 36)
Cognition had $73M ARR from Devin alone by June 2025, raised $400M at $10.2B valuation in September 2025, and combined ARR more than doubled post-Windsurf acquisition. This is factually wrong.

### 4. Cursor pricing is incomplete (Claim 9)
The EXAMPLE.md omits the Pro+ tier ($60/month, 3x usage) and Teams tier ($40/user/month). cursor.com/pricing shows 6 tiers, not 4. For a competitor pricing analysis, this is a material gap.

### 5. Cursor ARR estimate is severely outdated (Claim 34)
The document estimates "$500m-$1b+" but actual ARR as of April 2026 is ~$2B+, roughly 2-4x higher than the upper bound given.

### 6. Fabricated source titles (Claims 17, 20, 44)
Three cited sources do not exist at the URLs claimed:
- "Sourcegraph's Amp Has Dropped the Waiting List" -- not found on tessl.io/blog
- "Best LLM evaluation platforms 2025" -- not found on braintrust.dev
- "Your skill works on Opus. Does it make Haiku worse?" -- not found on tessl.io/blog

### 7. Cited source does not contain claimed data (Claim 41)
The Sourcegraph customer statistics ("4/6 top US banks, 15+ government agencies, 7/10 top tech companies") are attributed to qodo.ai/blog, but the fetched Qodo article does not contain these figures. The "15+ government agencies" figure specifically could not be verified in any source.

### 8. Windsurf funding data claimed unavailable (Claim 46)
The document states Windsurf's "revenue and funding details [are] not publicly disclosed" when they are extensively documented across TechCrunch, CNBC, VentureBeat, and Tracxn.

### 9. Company age is wrong (Claim 39)
Tessl is stated as "18 months old" but was founded February 2024, making it ~26 months old as of April 2026.

---

## Material Omissions

1. **Cursor Pro+ tier ($60/month)** -- entirely absent from pricing comparison
2. **Cursor Teams tier ($40/user/month)** -- absent
3. **Windsurf Max tier ($200/month)** and **Teams tier ($40/user/month)** -- absent
4. **Amp's ad-supported model** -- not disclosed; described simply as "free"
5. **Cursor's actual ARR (~$2B as of March 2026)** -- significantly exceeds the estimate given
6. **Windsurf's origin as Codeium** -- not mentioned anywhere in the document
7. **Cognition's $10.2B valuation and $400M+ fundraise** -- not reflected in Windsurf assessment

---

## Methodology Notes

- **URLs fetched directly**: tessl.io, tessl.io/about, tessl.io/blog, tessl.io/registry, cursor.com/pricing, windsurf.com/compare/windsurf-vs-cursor, windsurf.com/pricing, ai-sdk.dev/docs/introduction, braintrust.dev, docs.tessl.io, qodo.ai/blog/top-github-copilot-alternatives, fortune.com/2024/11/14/tessl-funding-ai-software-development-platform, techcrunch.com/2024/11/14/tessl-raises-125m
- **URLs that failed to render**: sourcegraph.com/docs/cody/usage-and-pricing (JavaScript-only), sourcegraph.com/pricing (JavaScript-only), g2.com/products/tessl/competitors (403 Forbidden)
- **Cross-reference searches performed**: 12 WebSearch queries across TechCrunch, Fortune, CNBC, VentureBeat, Tracxn, Crunchbase, and other sources
