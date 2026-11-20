# Structured Analytic Techniques — SATs

**ANBU Division 008 · Analytics**

---

## Purpose

Structured analytic techniques are explicit, repeatable procedures that force analysts to examine evidence systematically rather than intuitively. This file catalogs the SATs used across ANBU, states when each applies, and defines the minimum rigor expected for each.

## Scope

Covers techniques applicable to OSINT-only evidence: text, imagery metadata, public records, statistics, social-media reporting treated as unverified claims, and geospatial open data. Techniques requiring classified collection or technical access are out of scope.

## Intelligence objectives

- Reduce susceptibility to cognitive bias through procedural discipline.
- Increase the discriminating power of analysis — separating hypotheses the evidence can actually distinguish.
- Produce products whose reasoning can be audited and challenged.
- Make analytic confidence commensurate with the evidence base.

## Core concepts

- **Structure over intuition.** The technique externalizes reasoning into steps another analyst can replicate.
- **Discrimination.** The value of a technique is measured by how much it separates rival explanations.
- **Devil's advocacy.** Deliberately arguing the strongest case against the favored hypothesis.
- **Red teaming.** Subjecting a finished assessment to structured attack before dissemination.
- **Key assumptions check.** Enumerating the beliefs the assessment depends on and testing each.

## Analytical methodology

Every SAT follows the same lifecycle: define the question → state hypotheses → specify the technique → execute per its procedure → record results → challenge the output → attach confidence.

## Step-by-step workflow

1. Select the SAT by matching it to the question type (see matrix below).
2. Write the hypotheses down before examining evidence in detail.
3. Execute the technique mechanically; resist improvising mid-procedure.
4. Document the matrix, argument, or checklist produced.
5. Run `red_team_analytical_review.md` on the result.
6. File the technique output as an annex to the main product.

## SAT selection matrix

| Question type | Primary technique | Supporting technique |
|---|---|---|
| Which explanation is correct? | ACH | Key assumptions check, alternative explanations |
| Is the evidence sufficient? | Key assumptions check | Intelligence gap assessment |
| What is the actor likely to do? | Scenario planning | Indicators and signposts |
| Is this pattern real or noise? | Pattern analysis | Hypothesis testing |
| What could go wrong with this assessment? | Red team review | Devil's advocacy |
| What do we not know? | Intelligence gap assessment | KAC |
| How do actors relate? | Network analysis | Institutional relationship mapping |

## Data requirements

Each technique has its own input needs; common requirements:

- A bounded question and defined decision.
- A hypothesis set developed before deep evidence review.
- Evidence items individually cited and verified per `../verification/`.
- Time and resource budget for the technique — SATs are not free.

## Approved public sources

Same as `analytical_reasoning.md`; plus for ACH and hypothesis testing: primary documents (statutes, budgets, procurement notices, official statements) preferred over commentary.

## Source verification standards

All evidence entering a matrix or argument must carry a verification grade. Unverified items may appear in ACH matrices only as explicitly flagged hypotheses-generators, never as diagnostic evidence.

## Analytical framework — technique profiles

### Analysis of Competing Hypotheses (ACH)

Procedure: list hypotheses → list evidence → matrix of evidence × hypothesis → mark consistent/inconsistent → look for evidence that is diagnostic (supports one, undermines others) → eliminate hypotheses → review. Full detail in `analysis_of_competing_hypotheses.md`. Diagnostic evidence is the scarce resource; non-diagnostic evidence is discarded from the matrix.

### Key Assumptions Check (KAC)

Enumerate every assumption the assessment relies on, rank by fragility (how likely false × impact if false), and test the fragile load-bearing ones first. See `key_assumptions_check.md`.

### Devil's advocacy

Assign the analyst (or a reviewer) to build the strongest honest case against the current judgment, using only legitimate evidence and reasoning. The goal is stress, not demolition.

### Red team analytical review

A fresh-eyes pass that attacks the assessment's structure: evidence sufficiency, hidden assumptions, mirror-imaging, confidence inflation, alternative explanations not considered. See `red_team_analytical_review.md`.

### Scenario planning

Develop 3–4 internally consistent futures driven by key uncertainties, each with signposts that would indicate which scenario is unfolding. See `trend_analysis.md` and `indicators_and_signposts.md`.

## Evidence requirements

- Technique outputs must cite the same evidence base as the main product.
- Matrix cells must be justified; an unmarked cell is a defect.
- Every eliminated hypothesis must state why it failed.

## Confidence assessment

Technique rigor raises the ceiling on achievable confidence but does not guarantee it. A perfectly executed ACH on thin evidence still yields LOW or INSUFFICIENT confidence. Confidence is assigned after technique execution, per `analytical_confidence_language.md`.

## Common analytical mistakes

- Running a technique ceremonially — filling the matrix without letting it change the conclusion.
- Treating diagnostic and non-diagnostic evidence as equally informative.
- Using devil's advocacy as a token gesture with a predetermined outcome.
- Skipping the documentation of technique output, making the analysis unreproducible.
- Applying the wrong technique for the question type.

## Ethical considerations

SATs must be used to improve judgment, not to launder a predetermined conclusion through procedural theater. Analysts must not construct "technique outputs" that misrepresent what the procedure actually found. When a technique contradicts the desired answer, the technique wins or the disagreement is disclosed.

## Security boundaries

Techniques operate only on verified public-source evidence. No technique may justify collection escalation beyond OSINT boundaries. Outputs remain analytical judgments, not targeting products.

## Expected output

For each technique applied: a completed worksheet (matrix, assumption list, scenario set, or review memo) filed as an annex, plus a short note in the main product stating which techniques were run and what they changed.

## Quality checklist

- [ ] Technique matched to question type.
- [ ] Hypotheses written before evidence review.
- [ ] Technique executed per procedure, not improvised.
- [ ] Output documented and annexed.
- [ ] Red team or devil's advocacy pass completed.
- [ ] Confidence reassessed after technique execution.

## Cross-reference links

- [`analysis_of_competing_hypotheses.md`](analysis_of_competing_hypotheses.md) — ACH procedure.
- [`key_assumptions_check.md`](key_assumptions_check.md) — KAC procedure.
- [`red_team_analytical_review.md`](red_team_analytical_review.md) — structured attack on assessments.
- [`hypothesis_testing.md`](hypothesis_testing.md) — probabilistic hypothesis evaluation.
- [`analytical_reasoning.md`](analytical_reasoning.md) — foundational reasoning standard.
- [`cognitive_bias_mitigation.md`](cognitive_bias_mitigation.md) — bias taxonomy and controls.
- [`../core/structured_analytic_techniques.md`](../core/structured_analytic_techniques.md) — division doctrine.
- [`../verification/evidence_grading.md`](../verification/evidence_grading.md) — evidence grades feeding techniques.
- [`../reporting/annex_templates.md`](../reporting/annex_templates.md) — worksheet formats.
