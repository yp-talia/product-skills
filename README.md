# PM Prompts

A collection of Claude skills, prompts, and LLM tools built for product managers working on real products.

Not tutorials. Not demos. Things I actually use.

---

## What's here

### 🔥 Roadmap Roast

A Claude skill that evaluates a product roadmap before you present it. It researches your competitive landscape, asks what you already know isn't working, then gives you a structured critique — what's strong, what's missequenced, what's a growth bet with no evidence behind it, and the one question the roadmap can't answer that it should be able to.

Built for the moment the night before you stand in front of people and commit to a direction publicly. It has no social pressure to be coy.

**Install:** Download `roadmap-roast.skill` and install it in Claude.

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

After the initial roast, you can push back, provide constraints, or ask it to reframe the roadmap for a specific scenario. It holds positions with evidence or updates them with explicit reasoning, it doesn't just agree.

**Evals:** `roadmap-roast/evals/evals.json` — 8 test cases, 93 expectations. Run against `roadmap-roast/SKILL.md` using the Claude Code eval prompt in `roadmap-roast/eval-prompt.md`.

---



## Contributing

If you've built something in the same spirit — a prompt, a skill, a Claude Code hook, an eval harness — open a PR. The bar is: would you actually use this on a real product?

---

## Author

Yiannis Pelekanos — product leader, [LinkedIn](https://www.linkedin.com/in/yiannispelekanos/)).
