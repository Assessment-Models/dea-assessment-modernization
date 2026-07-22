# Self-Assessment Guide — Architecture Modernization Assessment

How to self-administer the modernization assessment without a facilitator.

---

## When to self-assess

- Initial baseline scan
- Annual health check
- Pre-merge gate for new initiatives
- Quarterly trend tracking

Do NOT self-assess for board-level reporting or transformation kick-offs — use a facilitated workshop.

---

## Setup (30 minutes)

1. Pull the latest `instrument.yaml` from this repo
2. Identify one person per dimension (or fewer if dimensions < people):
   - **Strategy** — Modernisation Lead or Sponsor
   - **Pattern Library** — Lead Architect
   - **Execution** — Wave Lead or Engineering Manager
   - **Metrics** — Engineering Manager or Sponsor
   - **People** — People Manager
3. Send instrument to each scorer with the scoring rubric
4. Agree a deadline (typically 1 week)

---

## Scoring (per dimension, ~45 minutes)

For each question in your assigned dimension:

1. Read the question
2. Read the evidence list
3. Score 0–3 based on how many evidence items are present
4. Cite at least one piece of evidence for scores of 2 or 3
5. Record: `[score] — [evidence]`

---

## Aggregation (per domain, ~30 minutes)

For each dimension:

1. Sum all question scores (max = questions × 3)
2. Compute: `(sum / max) × 100` = dimension score (0–100)
3. Mark the band: 0–25, 26–50, 51–75, 76–90, 91–100

For the overall modernization score:

1. Multiply each dimension score by its weight
2. Sum weighted scores
3. Result = modernization score (0–100)

---

## Reconciliation (if multiple scorers per dimension, ~30 minutes)

If two scorers give scores that differ by > 1 point on a question:

1. Surface both scores with evidence
2. Discuss until consensus OR record both
3. Use the lower score when in doubt (more conservative)

---

## Output (1 hour)

Fill in `gap-analysis-template.md` with:

- Scores by dimension
- Top 5 gaps
- Maturity band mapping
- Top 3 quick wins

---

## Follow-up

- **Within 30 days:** publish results internally
- **Within 90 days:** re-run assessment, compare scores
- **If score drops > 10 points:** trigger root-cause review
- **If score increases > 15 points:** promote learnings as case study

---

## Tips for accurate scoring in modernization

1. **Score where you are, not where you want to be.** Aspirational scoring is the most common error in modernisation — teams are optimistic about progress.
2. **Be specific in evidence.** "We have a pattern library" is weak. "12 patterns in git, last reviewed 2026-04-15, used in 3 production migrations" is strong.
3. **Don't skip the people dimension.** Technical maturity without cultural change is brittle.
4. **Compare to last assessment.** Trend is more informative than absolute score.

---

## When to escalate to a facilitated workshop

- Score < 50 (Ad Hoc / Defined) — strategy + foundation work needs broader input
- Significant organisational change (merger, restructure, new leadership)
- Board-level reporting
- Conflict between scorers that can't be resolved

---

## Related

- `gap-analysis-template.md` — output deliverable
- `target-state-template.md` — 12-month roadmap
- `instrument.yaml` — the actual questions