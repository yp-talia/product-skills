# Roadmap Roast v4 — Evaluation Framework & Test Data

## How to evaluate this skill

Five layers of evaluation, in increasing subjectivity.

### Layer 1: Process compliance (mechanical, binary)

| Check | Pass condition |
|---|---|
| Asked for company stage if missing | Yes — single combined question, not two separate |
| Asked self-assessment question before research | Yes — "what feels shakiest?" |
| Ran market research before evaluating | Yes — at least 2 searches, named entities in output |
| Acknowledged self-assessment answer in roast | Yes — validated or reframed what user named |
| Normalisation line present before roast | Yes — in italics |
| Scorecard present | Yes — all 5 dimensions scored |
| Severity triage on all roast points | Yes — every point has 🔴/🟡/🟢 |
| One thing to do this week present | Yes — specific, ≤5 working days |
| Go deeper section present | Yes — contains constraints question AND three follow-up threads |
| Constraints question is single combined prompt | Yes — not multiple separate questions, ≤3 sentences |
| Follow-up threads are roadmap-specific | Yes — each names a specific item or tension from this roast, not generic prompts |

### Layer 2: Specificity (requires human judgement)

For each roast point: could this apply to any roadmap, or is it clearly tied to this specific input?

Generic (bad): "Consider validating your assumptions before building."
Specific (good): "The Salesforce integration is in Q1 but there's no signal of enterprise demand — this looks like a founder assumption, not a customer signal."

Rate each roast point: **Specific / Somewhat specific / Generic**
Pass: 0 generic, ≤1 somewhat specific across all points.

### Layer 3: Fluency calibration (requires human judgement)

Given the fluency signals in the input, does the output use appropriate vocabulary?

Low fluency input receiving high fluency output = fail.
High fluency input receiving dumbed-down output = fail.

Rate: **Well-calibrated / Slightly off / Wrong register**

### Layer 4: Stage calibration (requires human judgement)

Is the critique appropriate for the stated company stage? Would a senior product leader at this stage find it fair?

Rate: **Well-calibrated / Slightly off / Significantly miscalibrated**

### Layer 5: Market research integration (requires human judgement)

Did the market research actually influence the roast, or is the market context section decorative?

Ask: is at least one roast point or craft improvement traceable to something found in research?

Rate: **Integrated / Present but unused / Absent**

---

## What good looks like

A strong output:
- Has a market context section that names something specific and uses it in the critique
- Has a self-assessment acknowledgement that feels responsive, not scripted
- Has a scorecard that tells a coherent story — the roast points match the low scores
- Has a roast where every point makes the user think "I knew this and hadn't said it out loud"
- Has severity triage that creates a clear action order — the user knows what to fix first
- Has a "question worth sitting with" that's still unresolved on Monday
- Has craft improvements that are habits, not projects
- Uses language the user can actually understand given their background
- Has a Go Deeper section with a constraints question that feels natural, not interrogative
- Has three follow-up threads that name specific items or tensions from the roast — not generic invitations

A weak output:
- Has a market section that says nothing specific
- Ignores what the user said was shakiest
- Has roast points that could apply to any roadmap
- Triages everything as 🔴 (no real prioritisation)
- Recommends frameworks instead of behaviours
- Uses jargon a low-fluency user won't understand
- Is so hedged it's useless
- Has generic follow-up threads that could apply to any roadmap
- Asks for constraints as multiple separate questions rather than one combined prompt

---

## Test cases

### Test 1: Missing context — must ask, not guess

**Input:**
> Roast my roadmap:
> - Dark mode
> - API v2
> - Onboarding redesign
> - Salesforce integration
> - Mobile app

**Expected:** Single clarifying question combining stage + success. No roast attempted. No self-assessment question yet (can't ask it before context is established).

**Pass condition:** Response is ≤4 sentences, asks for stage and success definition, nothing else.

---

### Test 2: Low fluency — founder, no product background, minimal input

**Input:**
> Hi — can you look at our roadmap and tell me if it makes sense? We're a 6-month-old startup, just got our first £250K from angels. We make software for restaurant managers to track staff rotas and costs. We want to get to 20 paying restaurants in the next 6 months.
>
> Things we're building:
> - Rota builder (drag and drop)
> - Wage cost calculator
> - WhatsApp notifications for shift changes
> - Staff app (view rotas on phone)
> - Integration with Xero

**Expected:**
- Self-assessment question first
- Market research on restaurant scheduling / workforce management software (Deputy, Rotaready, Planday)
- Plain language throughout — no jargon
- Roast should be gentle but specific — WhatsApp notifications is smart (meets staff where they are), Xero integration is probably premature at this stage
- Craft improvements should be in plain language: "before you build the staff app, ask 5 restaurant managers to show you how their staff currently find out about shift changes"
- Question should be accessible: "If a restaurant manager signed up today and used this for a month, what's the one thing they'd tell their friend it does?"

**Pass condition:** Zero jargon in output without plain-language definition. Roast is warm but specific. Self-assessment question was asked. Market context names at least one competitor.

---

### Test 3: High fluency, Series A, classic output-oriented roadmap (core test case)

**Input:**
> Please roast this. Series A, £4M raised, B2B fintech — we help finance teams automate month-end close. ICP is mid-market CFOs (£50M–£500M revenue). Success in 6 months = hit £1M ARR, reduce average onboarding from 6 weeks to 3.
>
> Q1: Bank reconciliation v2, Bulk transaction import, CSV export improvements, New user onboarding flow, Role-based access control
> Q2: ERP integrations (NetSuite, Sage), Audit trail, Custom reporting, Multi-currency support, Mobile app (view only)
> Q3: AI-powered anomaly detection, Partner API, White-label option

**Expected:**
- Self-assessment question first
- Market context: FloQast, Numeric, BlackLine — ERP integrations already table stakes
- Scorecard: outcome orientation ~2/5, strategic alignment ~3/5, discovery evidence ~1/5, sequencing ~2/5, portfolio ~2/5
- Roast: everything outputs not outcomes; ERP integrations missequenced given ICP; mobile app for mid-market CFOs is questionable; Q3 is a wish list; nothing for existing customer retention
- 🔴 on outcome framing and ERP sequencing; 🟡 on mobile app; 🟢 on Q3 vagueness
- Question: "If you hit £1M ARR in 6 months, which items made the biggest difference to a CFO signing, and can you draw a line from each one to that outcome?"
- Craft improvements: tied to specific items, behavioural

**Pass condition:** Names FloQast/Numeric/BlackLine. Identifies output-vs-outcome gap. Severity correctly triaged. Scorecard scores match roast severity. Full product vocabulary acceptable given high fluency input.

---

### Test 4: Self-assessment reveals sensitive area — must acknowledge

**Input (after self-assessment question):**
> Roast my roadmap please. Series B, £12M raised, HR platform for SMEs. Success in 6 months = £2M ARR and NPS > 50.
>
> Q1: Self-serve onboarding, Document templates v2, Automated contract renewal reminders, Reporting dashboard
> Q2: Payroll integration (Xero, Sage), AI contract review, Mobile app, Multi-entity support
> Q3: Marketplace (partner integrations), White-label offering
>
> [After self-assessment question, user responds:]
> "Honestly the AI contract review — I'm not sure we have the data to do it well and I worry it's been pushed up by the CEO rather than coming from customers."

**Expected:**
- The roast explicitly names AI contract review
- Validates their concern ("you're right to flag this") and deepens it ("the risk is this ships half-baked and erodes trust with CFOs at exactly the moment you need them to renew")
- Does NOT ignore the self-assessment response and give a generic roast
- Acknowledges the "pushed by CEO" political context sensitively — frames it as an alignment issue to address, not a problem to expose

**Pass condition:** AI contract review is named in roast. User's self-assessment is explicitly acknowledged by name. Political sensitivity handled — doesn't make the user feel worse about the CEO dynamic.

---

### Test 5: Genuinely strong roadmap — don't manufacture problems

**Input:**
> Roast this — be honest even if it's good. Series B, £18M raised, consumer health app. Success in 6 months = +40% MAU, improve 30-day retention from 34% to 45%.
>
> Theme 1: Retain (60% capacity): Personalised content recommendations (proven in A/B test), Weekly progress recap (proven retention driver), Push notification optimisation
> Theme 2: Acquire (25% capacity): Referral programme v1, SEO content hub (12-week project)
> Theme 3: Explore (15% capacity): AI therapy companion (6-week research spike, exit criteria: 3 partnership conversations + user willingness to pay signal), B2B employee wellbeing pilot (separate track, 1 PM)

**Expected:**
- Scorecard: outcome orientation ~4/5, strategic alignment ~5/5, discovery evidence ~4/5, sequencing ~4/5, portfolio balance ~5/5
- Genuine praise: explicit outcome framing, evidence of A/B testing, capacity allocation visible, explore track has exit criteria (rare and good), B2B track is correctly isolated
- Roast should be lighter — real issues only: push notification optimisation adjacent to dark pattern territory in mental health (worth flagging); SEO content hub is 12 weeks but the 6-month metric is MAU not SEO traffic (misalignment); referral programme without stated virality assumption is risky
- 🟡 on push notifications and SEO timeline; 🟢 on referral
- Question: "What's the retention driver for users who don't engage with content recommendations — is there anything on this roadmap for the bottom quartile?"
- Should NOT manufacture problems with the outcome framing or capacity allocation

**Pass condition:** Output is noticeably lighter on critique than Tests 2/3. Scorecard reflects genuine quality. Praises exit criteria on explore track explicitly. Does not invent issues with things that are actually good.

---

### Test 6: Constraints provided — must apply them immediately

**Input (two turns):**

Turn 1 (initial roast already delivered for the Series A fintech in Test 3):
> [Go Deeper section asked for constraints]

Turn 2 (user provides constraints):
> "A few things to factor in: the ERP integrations are already committed to two customers for Q2 — we can't move them. We have 6 engineers total and one is leaving end of April. We have a board meeting in 8 weeks and the CEO wants to show progress on ARR. The mobile app was the CEO's idea and politically it's hard to kill."

**Expected:**
- Skill immediately acknowledges the constraints before proceeding
- ERP critique is retracted or reframed — committed customer items come off the table
- Capacity reduction (6 → 5 engineers) changes the sequencing analysis
- Board meeting in 8 weeks creates a near-term framing: what's demonstrable by then?
- Mobile app political sensitivity handled — reframes as "how to redirect" rather than "kill it"
- Does NOT re-ask for constraints already provided
- Does NOT ignore any of the stated constraints

**Pass condition:** All four constraints are explicitly referenced and applied in the response. ERP critique is visibly adjusted. Board timeline shapes the advice. Political sensitivity on mobile app is handled without making the user feel worse about the situation.

---

### Test 7: Debate mode — user pushes back on a roast point

**Input (two turns):**

Turn 1 (initial roast already delivered):
> [Roast flagged ERP integrations as missequenced — table stakes being delayed to Q2]

Turn 2 (user pushes back):
> "Actually the reason ERP is in Q2 isn't laziness — it's because our two EMIS integrations in Q1 are foundational and the ERP work depends on the same data pipeline. We physically can't do ERP before the pipeline is stable. The sequencing is correct."

**Expected:**
- Skill does NOT simply capitulate and agree
- Skill either: (a) holds its position if the pushback doesn't change the underlying concern, or (b) explicitly updates its position and explains what changed
- If updating: names exactly what the new context changed ("if the pipeline dependency is real, the sequencing is correct — what I'd watch instead is whether the pipeline slips and drags ERP with it")
- If holding: presents the original evidence and asks a clarifying question ("that makes sense as a technical dependency — does the pipeline slip risk get communicated to the prospects waiting on ERP?")
- Does NOT repeat the original roast point unchanged as if the user said nothing

**Pass condition:** Response is clearly a direct engagement with the pushback — not a repeat of the original point, not a flat capitulation. Position is either held with evidence or updated with explicit explanation of what changed.

---

### Test 8: Scenario mode — user asks for a reframe

**Input (two turns):**

Turn 1 (initial roast already delivered for Series A fintech):
> [Constraints already shared: 6 engineers, one leaving, board meeting in 8 weeks, ERP committed]

Turn 2 (scenario request):
> "Given all of that — what does this roadmap look like if we stripped it back to only what moves the NRR needle in the next 8 weeks before the board meeting? What stays, what moves, what gets cut?"

**Expected:**
- Skill enters scenario mode explicitly — states it's reframing against the 8-week/NRR constraint
- States assumptions being made (e.g. "assuming NRR improvement comes from reducing early churn, not expansion")
- Shows the reordered roadmap with explicit reasoning for each move: what stays and why, what moves and why, what gets cut and why
- References the constraints already provided (ERP committed so it stays; 5 engineers shapes what's feasible)
- Does NOT just reorder the list without explanation
- Does NOT ignore the constraints already shared
- Output is structured enough to be actionable — the user can take this to their team

**Pass condition:** Scenario is explicitly framed. Assumptions stated. Each item disposition (keep/move/cut) has a one-line reason. Constraints are visibly applied. Output could plausibly be shared with an engineering team as a direction.

---

## Scorecard (per test run)## Scorecard (per test run)

| Dimension | Score | Notes |
|---|---|---|
| Process compliance | /11 | One point per check (see Layer 1) |
| Specificity of roast | /3 | 3=all specific, 2=mostly, 1=generic |
| Fluency calibration | /3 | 3=well calibrated, 2=slightly off, 1=wrong register |
| Stage calibration | /3 | 3=well calibrated, 2=slightly off, 1=wrong |
| Market research integration | /3 | 3=integrated into critique, 2=present not used, 1=absent |
| Self-assessment acknowledged | /3 | 3=responsive and specific, 2=generic nod, 1=ignored |
| Severity triage quality | /3 | 3=differentiated and correct, 2=mostly correct, 1=all same/wrong |
| **Total** | **/29** | |

**Target:** ≥24/29 across all 5 tests. Any test below 17/29 warrants immediate skill revision.

---

## New red flags added in v4

- Go Deeper section absent entirely
- Constraints question is split into multiple separate questions
- Follow-up threads are generic ("want to explore any of these further?" is not a follow-up thread)
- Constraints provided by user are ignored in subsequent responses
- Skill re-asks for constraints already given
- Skill capitulates on a roast point without explaining what changed
- Scenario mode response is a reordered list with no reasoning

## Red flags requiring immediate revision (all versions)

- Skill proceeds to roast without asking for stage context
- Skill skips the self-assessment question entirely
- Self-assessment answer is ignored in the output
- Roast points are generic — none reference specific roadmap items
- Jargon used with a clearly low-fluency user without definition
- All roast points triaged as 🔴 (no real prioritisation)
- Framework recommendations appear (RICE, MoSCoW, OKRs as prescription)
- Market research section is absent or names nothing specific
- Strong roadmap (Test 5) receives equally heavy critique as weak one (Test 3) — failure to calibrate
- "One thing to do this week" is actually a multi-week project