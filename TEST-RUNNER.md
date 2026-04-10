# Skill Test Runner

Run evaluation test cases against a skill and score the output.

## How to use

1. Open a new session with the skill installed
2. Paste the test input from the relevant EVAL.md test case
3. Let the skill run to completion
4. Paste the output back into this session (or a scoring session) along with the eval prompt below

## Scoring prompt

Copy everything below the line into a new session with the skill output:

---

You are evaluating the output of a Claude skill. I'll provide:
1. The EVAL.md (evaluation criteria, scorecard, red flags)
2. The test case that was run (input + expected output + pass condition)
3. The actual output the skill produced

Your job:
- Score each Layer from the EVAL.md against the actual output
- Complete the scorecard with scores and brief notes
- Check every pass condition and state pass/fail with evidence
- Check every red flag and state whether it was triggered
- End with: "VERDICT: [PASS/FAIL/BORDERLINE]" and a 2-3 sentence summary

Be rigorous. A pass means every pass condition is met and no red flags are triggered. Borderline means minor issues that don't undermine the output's value. Fail means a pass condition is missed or a red flag is triggered.

---

## Recommended test order

Run one test case per skill to start. Pick the test that exercises the most interesting behaviour:

| Skill | Recommended first test | Why |
|---|---|---|
| research-company | Test 3: amicable (trading name ≠ registered name) | Tests the Companies House verification procedure — the hardest process step |
| research-product | Test 1: Notion | Rich data, tests full portfolio mapping and teardown quality |
| research-competitors | Test 5: PensionBee (inertia as competitor) | Tests whether the skill recognises non-obvious competitive dynamics |
| research-market | Test 3: UK wealth management | Tests regulation-heavy analysis — the most demanding variant |

## Quick smoke test (all four skills, one company)

If you want to test all four skills quickly against the same company:

**Company: Monzo**
- research-company: Test 1
- research-product: Test 2
- research-competitors: Test 3
- research-market: Test 1

This gives you a connected set of outputs for the same company, making it easy to check consistency across skills.
