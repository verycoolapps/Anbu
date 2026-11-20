# Fact-Checking Methodology

**Division 007 · Verification · ANBU OSINT**

## 1. Purpose

Fact-checking is the applied, public-facing form of claim verification: systematically testing assertions in public discourse against evidence and publishing the result. This file defines ANBU's internal fact-checking workflow — the standard to which ANBU's own published verdicts and any fact-check products must adhere.

## 2. Scope

Covers claims circulating in public discourse: political statements, viral posts, news assertions, official claims, and advertising/marketing assertions. Distinct from internal claim verification in that results are formatted for public consumption and must meet higher evidentiary and impartiality bars.

## 3. Intelligence Objectives

- Publish verdicts that are correct, impartial, and audit-proof.
- Apply consistent methodology so verdicts are comparable across claims and analysts.
- Maintain IFCN-style standards: nonpartisanship, transparency of sources, open methodology.
- Correct the record promptly when ANBU's own checks err.

## 4. Core Concepts

- **Claim selection:** checkability, virality, harm potential, and source prominence drive priorities — not political convenience.
- **Symmetric standard:** the same evidentiary bar applies regardless of the claimant's identity or ideology.
- **Rating transparency:** publish the rating scale and what each rating requires *before* verdicts.
- **Right of reply:** documented effort to obtain the claimant's response is part of the methodology for public verdicts.

## 5. Analytical Methodology

1. **Select and scope:** define the exact claim, its context, and the date of the assertion.
2. **Verify per `claim_verification.md`:** decompose, evidence-hunt, corroborate, score.
3. **Apply rating scale:** e.g., TRUE / MOSTLY TRUE / MIXED / MOSTLY FALSE / FALSE / UNVERIFIABLE with published definitions.
4. **Document everything:** evidence manifest, search log, corroboration map, dissent.
5. **Draft verdict:** plain-language explanation with evidence links; avoid partisan framing.
6. **Editorial review:** independent analyst re-checks methodology and wording (`reporting/` standards).
7. **Publish with corrections policy:** every verdict carries methodology link, evidence links, date, and author.

## 6. Step-by-Step Workflow

1. Log the claim with provenance (`source_provenance_tracking.md`).
2. Run full claim-verification workflow; produce verdict card.
3. If verdict is contested or confidence < MODERATE, escalate to senior review before publication.
4. Attempt claimant response where feasible; document attempts.
5. Publish verdict with rating, evidence manifest, methodology statement.
6. Monitor for new evidence; re-open the check if material evidence emerges; publish updates transparently.
7. File all materials in the audit trail; corrections get their own dated entries.

## 7. Data Requirements

- Full claim provenance and context capture.
- Evidence manifest meeting chain-management standards.
- Rating-scale definitions document (versioned).
- Response-attempt log.
- Corrections log.

## 8. Approved Public Sources

Same evidence universe as claim verification, with stricter weighting toward primary records and away from partisan secondary sources. For political claims, official records (votes, budgets, statutes, transcripts) outrank commentary. Fact-checks may cite other fact-checkers only as discovery leads, not as evidence.

## 9. Source Verification Standards

Public fact-checks meet the highest verification bar in the system: every verdict requires either authenticated primary evidence or robust multi-tier corroboration; every evidence link must resolve at publication; every rating must map to published criteria. Verdicts that cannot meet the bar are published as UNVERIFIABLE with the search documented.

## 10. Analytical Framework

Use the **Check Package**: claim card + evidence manifest + rating justification + response log + methodology statement. The package is self-contained — a reader should be able to re-run the check from the package alone. This is the standard `reporting/` templates implement.

## 11. Evidence Requirements

Each published verdict links: the claim (with timestamp), every evidence item (with provenance), the corroboration map, the rating rationale, the response attempt, and the methodology version. Broken evidence links discovered post-publication trigger immediate correction review.

## 12. Confidence Assessment

Public verdicts publish confidence alongside rating: HIGH = primary-anchored; MODERATE = strong corroboration; LOW = limited evidence (usually forces UNVERIFIABLE); INSUFFICIENT = cannot responsibly publish a rating — internal note only.

## 13. Common Analytical Mistakes

- Rating the interpretation instead of the literal claim (or vice versa) — state which was checked.
- Cherry-picking the narrowest reading to earn a technically-true rating.
- Publishing verdicts on claims too ambiguous to test fairly.
- Failing to check the claim's original context (e.g., a quote clipped from a longer statement).
- Letting the claimant's prominence lower the evidentiary bar.

## 14. Ethical Considerations

Fact-checking is powerful and easily weaponized. Strict nonpartisanship, published methodology, symmetric standards, prompt corrections, and transparency about uncertainty are mandatory. Never fact-check to advance a preferred political outcome; the check serves the claim, not the checker.

## 15. Security Boundaries

No private-data exposure in published verdicts. Evidence involving minors, victims, or sensitive sources gets `legal/` review. Do not publish verdicts that would identify anonymous sources or compromise ongoing security matters — refer to `security/` and `legal/`.

## 16. Expected Output

Published verdicts in `reporting/` format with full check packages; an internal corrections log; periodic methodology reviews; an archive of verdicts machine-readable for analytics.

## 17. Quality Checklist

- [ ] Claim scoped precisely with context and date
- [ ] Full verification workflow executed
- [ ] Rating justified against published scale
- [ ] Evidence manifest complete and links resolve
- [ ] Response attempt documented
- [ ] Independent editorial review passed
- [ ] Confidence published alongside rating
- [ ] Corrections policy acknowledged

## 18. Cross-Reference Links

- Core method: `claim_verification.md`, `cross_source_corroboration.md`, `source_credibility_scoring.md`
- Claim integrity: `quotation_verification.md`, `publication_date_verification.md`, `translation_verification.md`
- Manipulation context: `misinformation_detection.md`, `disinformation_detection.md`, `propaganda_analysis.md`, `manipulated_media_assessment.md`
- Standards: `source_citation_standards.md`, `verification_audit_trail.md`
- Divisions: `reporting/` (verdict format), `legal/` (publication liability), `analytics/` (verdict datasets)
