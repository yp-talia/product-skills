# Product Skills

A collection of Claude skills built for product managers working on real products.

Not tutorials. Not demos. Things I actually use.

---

## What's a Claude skill?

A Claude skill is a reusable prompt — with structure, evaluation criteria, and often a multi-step workflow — that runs inside [Claude Code](https://docs.anthropic.com/en/docs/claude-code) or [Cowork](https://claude.ai/cowork). Think of it as a senior colleague you can invoke on demand: it has a point of view, it does research, and it produces structured output you can act on. Skills can use web search, browser automation, and external tools — they're not just prompt templates.

---

## What's here

### Roadmap Roast

A Claude skill that evaluates a product roadmap before you present it. It researches your competitive landscape, asks what you already know isn't working, then gives you a structured critique — what's strong, what's missequenced, what's a growth bet with no evidence behind it, and the one question the roadmap can't answer that it should be able to.

Built for the moment the night before you stand in front of people and commit to a direction publicly. It has no social pressure to be coy.

**Install:** Download `roadmap-roast/roadmap-roast.skill` and install it in Claude.

**What it takes as input:**
- A flat list of roadmap items (minimum — names only is fine)
- Horizon-bucketed items with brief rationale
- A full context block with stage, Ideal Customer Profile, validation, success definition, and itemised roadmap (maximum)

**What it produces:**
- Market context (researched, not assumed)
- What's actually working
- A scorecard across five dimensions
- A severity-triaged roast (🔴/🟡/🟢)
- The question worth sitting with
- Three craft improvements
- One thing to do this week
- Follow-up threads and a constraints question to go deeper

After the initial roast, you can push back, provide constraints, or ask it to reframe the roadmap for a specific scenario. It holds positions with evidence or updates them with explicit reasoning — it doesn't just agree.

**Evals:** `roadmap-roast/evals/evals.json` — 8 test cases, 93 expectations. Run against `roadmap-roast/SKILL.md` using the Claude Code eval prompt in `roadmap-roast/eval-prompt.md`.

**Example output:** [`roadmap-roast/EXAMPLE.md`](roadmap-roast/EXAMPLE.md) — a Series A consumer legaltech roadmap with severity-triaged critique, competitive blind spots, and a discovery gap on the biggest growth bet.

---

### Research Skills

A set of four research skills for product managers doing company intelligence, product analysis, competitive landscaping, and market mapping. Each skill runs a structured, multi-step research workflow using web search and browser tools, producing cited, opinionated output.

Each skill works independently for any due diligence, strategic planning, or "I need to understand this company/market fast" moment. They can also be used together "research {company name} company, product, market and competitors".

| Skill | What it does |
|---|---|
| **research-company** | Company background, financials, culture, growth model, technology landscape. Multi-perspective analysis comparing what the company says about itself vs what investors, employees, customers, and press say. [`Example →`](research-company/EXAMPLE.md) |
| **research-product** | Product teardown — what it is, who it serves, value chain, unit economics, market sizing, and a hands-on experience walkthrough. [`Example →`](research-product/EXAMPLE.md) |
| **research-competitors** | Competitive landscape — direct, strategic, and adjacent competitors. Feature comparison matrix, pricing analysis, audience segmentation, and underserved segments. [`Example →`](research-competitors/EXAMPLE.md) |
| **research-market** | Porter's Five Forces applied to a specific market. Legislation tracking, trend analysis, demand signal classification, and macro forces. [`Example →`](research-market/EXAMPLE.md) |

All four skills follow the citation and triangulation rules in `references/source-and-triangulation.md`.

**Install:** Download the `.skill` file from any skill folder and install it in Claude.

---

## Shared references

| File | Purpose |
|---|---|
| `references/source-and-triangulation.md` | Citation format, source quality tiers, triangulation rules, and verification checks. Used by all research skills. |
| `references/output-templates.md` | Suggested output structures for each research skill. Use these directly or adapt to your own format. |

---

## Repo topics

`product-management` · `claude` · `llm-tools` · `ai-tools` · `product-strategy` · `competitive-analysis` · `market-research`

---

## Contributing

If you've built something in the same spirit — a prompt, a skill, a Claude Code hook, an eval harness — open a PR. The bar is: would you actually use this on a real product? Is it additive to what exists without adding undue complexity or context, have you evaluated your change?
---

## Author

[Yiannis Pelekanos](https://www.linkedin.com/in/yiannispelekanos/) — product leader. Also building [Moments in Vine](https://momentsinvine.com), a consumer SaaS for wine collectors.
