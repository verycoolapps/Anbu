# Source Credibility Scoring

**Division 007 · Verification · ANBU OSINT**

## 1. Purpose

Credibility scoring evaluates whether a *specific claim* from a source is believable, given what is known about the source, the claim's content, and its evidentiary support. This file operationalizes the second half of the reliability/credibility separation defined in `source_reliability_assessment.md`.

## 2. Scope

Applies to individual claims, assertions, figures, quotes, and attributed statements. Not for grading whole outlets (that is reliability) and not for scoring the final analytic judgment (that is `evidence_confidence_scoring.md`).

## 3. Intelligence Objectives

- Produce a transparent, numeric or ordinal credibility score for each material claim.
- Make scoring reproducible: another analyst given the same evidence must reach a similar score.
- Expose which inputs drive the score so consumers can audit rather than trust.
- Prevent false precision: scores are ordinal bands, not probabilities of truth.

## 4. Core Concepts

- **Claim-level vs. source-level:** a Grade-A wire can carry a Grade-D claim; a Grade-D blog can carry a claim later proven true. Score the claim.
- **Evidentiary support:** the score rises with primary-source confirmation, not with the plausibility of the story.
- **Motivated reasoning risk:** official sources may be accurate but motivated; motivated accuracy is still accuracy, but flag it in `source_bias_assessment.md`.
- **Score stability:** a claim's score may move as corroboration arrives; every change is logged in `verification_audit_trail.md`.

## 5. Analytical Methodology

Score each claim on five inputs, each 0–2 points (max 10):

1. **Source reliability grade** — from `source_reliability_assessment.md`.
2. **Evidentiary support** — primary record > official statement > corroborated secondary > lone secondary > unattributed.
3. **Corroboration** — independent sources agreeing (see `cross_source_corroboration.md`): 0 = none, 1 = partial, 2 = strong.
4. **Internal consistency** — does the claim fit the source's own record, documents, and known behavior?
5. **Adversarial context** — is the claim in a domain where this source has a documented fabrication history?

Map totals: 9–10 HIGH, 6–8 MODERATE-HIGH, 4–5 MODERATE, 2–3 LOW, 0–1 INSUFFICIENT.

## 6. Step-by-Step Workflow

1. Restate the claim in one sentence with all qualifiers preserved.
2. Pull the source's reliability record; note its grade.
3. Hunt for the best available evidentiary support; classify it on the support ladder.
4. Run corroboration check per `cross_source_corroboration.md`; count independent agree/disagree sources.
5. Score the five inputs; compute total; assign band.
6. Document the score rationale; file in `verification_audit_trail.md`.

## 7. Data Requirements

- The claim text exactly as published, with URL and access date.
- Source reliability record (must exist; create one first if absent).
- Corroboration set: list of independent sources found agreeing or disagreeing.
- Best available primary evidence or documented reason none exists.

## 8. Approved Public Sources

For scoring inputs: official records (gazettes, budgets, court filings, procurement notices), wire services, established fact-checkers (IFCN members), academic literature, and platform transparency data. For corroboration, prefer sources with no shared ownership or wire dependency — see `cross_source_corroboration.md`.

## 9. Source Verification Standards

A score is only as good as its weakest input. If the reliability grade is INSUFFICIENT, the claim score cannot exceed LOW regardless of other inputs — record this ceiling explicitly rather than hiding it.

## 10. Analytical Framework

Present scores as **claim cards**: claim text, source, reliability grade, evidentiary support class, corroboration count, total score, band, dissent notes. Cards are the atomic unit exchanged between verification and reporting divisions (`reporting/`).

## 11. Evidence Requirements

Each scored claim must retain: verbatim claim text, publication timestamp, source identifier, the five input scores with one-line justifications, corroboration source list, and access dates for every URL cited.

## 12. Confidence Assessment

The score itself carries a confidence: HIGH when all five inputs are populated with dated evidence; MODERATE when corroboration is partial; LOW when the claim rests on a single source of unknown reliability; INSUFFICIENT when the claim cannot be restated unambiguously (ambiguous claims are scored on their strongest reading and flagged).

## 13. Common Analytical Mistakes

- Scoring plausibility instead of evidence — a likely claim is not a credible claim.
- Counting three outlets that all rewrote the same wire dispatch as three corroborations.
- Averaging away a decisive negative (e.g., official denial) with positive vibes.
- Treating "no evidence found" as evidence of falsehood; absence of evidence is scored as missing corroboration, not disproof.

## 14. Ethical Considerations

Scores influence publication decisions. A LOW score is not a verdict of falsehood — it is a statement about current evidence. Report wording must preserve this distinction to avoid defaming individuals or institutions on thin evidence.

## 15. Security Boundaries

Scoring uses only already-collected public material. Do not contact sources to "verify" claims, do not submit test claims to platforms, and do not use private channels. Preserve chain of custody per `evidence_chain_management.md`.

## 16. Expected Output

A scored claim card per material assertion, plus an aggregate credibility summary when claims cluster (e.g., "8 of 12 claims in this dossier score ≤3"). Cards link to `source_citation_standards.md` format.

## 17. Quality Checklist

- [ ] Claim restated verbatim with qualifiers intact
- [ ] Source reliability record exists and is current
- [ ] All five inputs scored with justification
- [ ] Corroboration independence verified
- [ ] Band assigned and confidence stated
- [ ] Audit-trail entry filed

## 18. Cross-Reference Links

- Inputs: `source_reliability_assessment.md`, `cross_source_corroboration.md`, `primary_source_verification.md`
- Peers: `evidence_confidence_scoring.md`, `source_bias_assessment.md`, `source_provenance_tracking.md`
- Outputs: `claim_verification.md`, `fact_checking_methodology.md`, `reporting/`
- Divisions: `osint/` (claim harvesting), `analytics/` (scoring models), `legal/` (publication risk)
