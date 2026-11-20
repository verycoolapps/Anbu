# Red Team Analytical Review

**ANBU Division 008 · Analytics**

---

## Purpose

Red team analytical review subjects a completed assessment to structured adversarial attack before dissemination. The reviewer assumes the assessment is wrong and tries to prove it — not to sabotage, but to find the weaknesses the author missed. This file defines the red-team procedure, the attack categories, and how findings are adjudicated and incorporated.

## Scope

Applied mandatorily to strategic assessments, warning products, and any product supporting high-stakes decisions. Recommended for all assessments above LOW confidence requirements. Can be performed by a separate analyst or a structured self-review with fresh eyes.

## Intelligence objectives

- Find analytical weaknesses before consumers rely on the product.
- Test whether conclusions survive the strongest counterarguments.
- Identify hidden assumptions, evidence gaps, and confidence inflation.
- Improve product quality through constructive adversarial review.
- Prevent dissemination of assessments that would fail under scrutiny.

## Core concepts

- **Adversarial posture.** The reviewer argues against the assessment as if they disbelieve it — not to be hostile, but to test robustness.
- **Attack categories.** Structured dimensions of weakness: evidence, logic, assumptions, alternatives, confidence, completeness, bias.
- **Steelman requirement.** Attacks must use the strongest available counterevidence and reasoning — not strawmen.
- **Finding adjudication.** Each finding is accepted, rejected with reason, or deferred for more collection.
- **Revision trigger.** Certain findings (fatal evidence gaps, logical errors) require revision before dissemination; others are noted as limitations.
- **Independence.** Best practice is reviewer ≠ author; self-review is acceptable for lower-stakes products with documented limitations.

## Analytical methodology

1. Receive the completed assessment and its evidence annex.
2. Read for comprehension before attacking — understand what is claimed.
3. Attack systematically across all categories.
4. For each finding: cite the specific weakness, the evidence or reasoning, and the required fix.
5. Adjudicate findings: accept / reject / defer.
6. Return findings to author for revision.
7. Verify revisions address accepted findings.
8. Document the review: findings, adjudications, revisions made.

## Step-by-step workflow

1. **Preparation.** Reviewer reads the full product, evidence annex, and stated confidence.
2. **Evidence attack.** Are sources verified? Is corroboration real? Are contradictions disclosed? Are single sources load-bearing?
3. **Logic attack.** Does the conclusion follow from the evidence? Are inferential leaps flagged? Is the reasoning chain intact?
4. **Assumption attack.** Run `key_assumptions_check.md` independently — what is assumed but not stated?
5. **Alternative attack.** Run `alternative_explanations.md` — were rival hypotheses genuinely tested?
6. **Confidence attack.** Does the stated confidence match the evidence? Is it inflated or deflated?
7. **Completeness attack.** What evidence was not considered? What questions were not asked? What stakeholders/actors were missed?
8. **Bias attack.** Run `cognitive_bias_mitigation.md` checklist — anchoring, confirmation, mirror-imaging, availability?
9. **Adjudication.** Classify each finding: critical / major / minor / informational.
10. **Revision.** Author revises; reviewer verifies.

## Data requirements

- Complete assessment with evidence annex.
- Access to the same source base for verification.
- Independence from author bias (fresh reviewer preferred).
- Time and authority to require revision.

## Approved public sources

Same as the assessment under review — reviewer must be able to check sources independently. Reviewer's own knowledge and alternative source discovery are encouraged.

## Source verification standards

Reviewer independently verifies load-bearing sources. If reviewer cannot verify a source, the finding is "unverifiable source — requires re-verification or downgrade."

## Analytical framework

Attack categories and questions:

| Category | Key questions |
|---|---|
| Evidence | Are sources verified? Corroborated? Contradictions disclosed? |
| Logic | Does conclusion follow? Leaps flagged? Chain intact? |
| Assumptions | What is assumed? Load-bearing? Tested? |
| Alternatives | Rivals tested? Null hypothesis included? |
| Confidence | Matches evidence? Inflated? Deflated? |
| Completeness | Missing evidence? Unasked questions? Missing actors? |
| Bias | Anchoring? Confirmation? Mirror-imaging? Availability? |
| Communication | Is uncertainty clear? Is estimative language calibrated? |

## Evidence requirements

- Each finding cites specific text, evidence, or reasoning in the assessment.
- Findings include recommended fix.
- Adjudication records reason for acceptance/rejection.
- Revision verification confirms fixes.

## Confidence assessment

The review itself produces a quality verdict:

- **PASS** — no critical findings; assessment sound for dissemination.
- **PASS WITH CONDITIONS** — minor findings; assessment disseminated with noted limitations.
- **REVISE** — major findings; assessment must be revised before dissemination.
- **FAIL** — critical findings; fundamental flaws require major rework or withdrawal.

## Common analytical mistakes

- Rubber-stamp review: going through motions without genuine attack.
- Strawman attacks: attacking weak versions of arguments.
- Reviewing style instead of substance.
- Findings without specific citations.
- Accepting all findings uncritically (reviewer can be wrong too).
- Rejecting valid findings to protect the assessment.
- No revision verification — findings noted but not fixed.
- Reviewer too close to author (shared blind spots).

## Ethical considerations

Red team must strengthen analysis, not undermine it for political purposes. Findings must be honest even when they contradict desired conclusions. Reviewer must not use the process to insert their own analytical biases.

## Security boundaries

Review uses same public-source boundaries as the assessment. Reviewer must not introduce classified or non-public information. Review process itself is internal quality control.

## Expected output

Review memo: findings by category, adjudications, required revisions, final verdict. Filed with the assessment. Main product notes that red-team review was conducted and findings addressed.

## Quality checklist

- [ ] All attack categories systematically applied.
- [ ] Findings cite specific text/evidence.
- [ ] Steelman requirement met — strongest counterarguments used.
- [ ] Adjudication recorded with reasons.
- [ ] Revisions verified.
- [ ] Final verdict stated.
- [ ] Review documented and filed.

## Cross-reference links

- [`cognitive_bias_mitigation.md`](cognitive_bias_mitigation.md) — bias attack checklist.
- [`alternative_explanations.md`](alternative_explanations.md) — alternative attack.
- [`key_assumptions_check.md`](key_assumptions_check.md) — assumption attack.
- [`analytical_quality_control.md`](analytical_quality_control.md) — broader QA framework.
- [`analytical_reasoning.md`](analytical_reasoning.md) — reasoning standard.
- [`structured_analytic_techniques.md`](structured_analytic_techniques.md) — SAT context.
- [`../core/analytical_standards.md`](../core/analytical_standards.md) — doctrine.
- [`../reporting/review_memo_template.md`](../reporting/review_memo_template.md) — output format.
