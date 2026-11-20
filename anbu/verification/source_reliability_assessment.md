# Source Reliability Assessment

**Division 007 · Verification · ANBU OSINT**

## 1. Purpose

This file defines how ANBU grades the inherent reliability of an information source before any content evaluation occurs. Reliability answers one question: *how consistently does this source provide accurate information under normal conditions?* It is deliberately separated from credibility, which evaluates whether a specific claim is true. A highly reliable source can publish a false claim; a low-reliability source can accidentally publish a true one. Conflating the two is the most common verification failure in OSINT practice.

## 2. Scope

Applies to every source ANBU touches: individuals, publications, institutions, datasets, social accounts, leaked repositories, and automated feeds. The rubric is source-type agnostic; type-specific addenda appear in `primary_source_verification.md`, `secondary_source_verification.md`, and `tertiary_source_handling.md`.

## 3. Intelligence Objectives

- Assign each source a stable, auditable reliability grade (A–F or NATO-style 1–6) with written justification.
- Separate source reliability from content credibility in every analytic product.
- Build a longitudinal reliability record per source so re-use across tasks compounds institutional knowledge.
- Identify sources that are structurally reliable but contextually compromised for a given question.

## 4. Core Concepts

- **Reliability vs. credibility:** reliability is a property of the source; credibility is a property of a claim. See `claim_verification.md`.
- **Base-rate behavior:** a wire service with a 99% historical accuracy rate is still a source, not a guarantee.
- **Structural reliability:** some sources are reliable because of institutional constraints (courts, statistical agencies, peer review). Others are reliable because of track record.
- **Reliability decay:** sources degrade. A defunct outlet's archive remains citable; its live output does not.
- **Adversarial reliability:** a source can be reliably wrong — propaganda outlets are dependable emitters of disinformation. Detect this in `disinformation_detection.md`.

## 5. Analytical Methodology

1. **Classify the source type** (see tier files). Tier determines which rubric columns apply.
2. **Gather reliability evidence:** correction history, retraction record, known fabrication incidents, editorial standards, ownership, funding transparency.
3. **Score five dimensions:** accuracy record, correction behavior, institutional accountability, independence, methodological transparency.
4. **Apply the grade.** Grades: **A** (reliable, minimal verification needed), **B** (usually reliable), **C** (fairly reliable, requires corroboration), **D** (not usually reliable), **F** (unreliable / known fabricator).
5. **Record dissent.** If analysts disagree, note both grades and the disputed evidence in `verification_audit_trail.md`.

## 6. Step-by-Step Workflow

1. Identify the source and assign a persistent identifier (domain, handle, DOI, archive URL).
2. Pull its reliability dossier: about page, masthead, ownership disclosures, correction policy, archive spot-checks.
3. Sample 5–10 past claims against primary records; compute an informal error rate.
4. Assign provisional grade with confidence level.
5. Update `source_provenance_tracking.md` entry; link all downstream citations to the graded record.
6. Re-grade quarterly or on any retraction/fabrication event.

## 7. Data Requirements

- Source identity metadata: canonical URL, owner, jurisdiction, language, format.
- Historical performance sample: minimum 5 verifiable claims.
- Correction/retraction log where available.
- Known external assessments: media-freedom indices, academic citations, fact-checker rulings.

## 8. Approved Public Sources

Reliability grading may cite: Reuters/AP correction archives, ombudsman reports, academic media studies, IFCN signatory lists, ownership databases (e.g., media ownership trackers), court records on defamation/fabrication, and the platform's own transparency reports. Prefer primary records over commentary about the source.

## 9. Source Verification Standards

A source cannot be graded from its self-description alone. At least two independent external signals (ownership data + correction record, or academic study + platform enforcement action) are required for grades A or B. Grade F requires documented fabrication evidence — not reputation.

## 10. Analytical Framework

Use the **Reliability Vector**: plot the source on five axes (accuracy, accountability, independence, transparency, durability). A source strong on accountability but weak on independence is usable with caveats; a source weak on all five is tertiary at best. Feed results into `source_credibility_scoring.md` for claim-level work.

## 11. Evidence Requirements

Every grade must cite: (a) the sampling method used, (b) at least two external corroborating signals, (c) the date of assessment, (d) the analyst. Grades without evidence are void and must be marked INSUFFICIENT in `evidence_confidence_scoring.md`.

## 12. Confidence Assessment

| Level | Criteria |
|---|---|
| HIGH | ≥10 sampled claims, ≥3 external signals, recent assessment (<12 months) |
| MODERATE | 5–9 sampled claims, 2 external signals |
| LOW | Self-report only, single external signal, or stale data |
| INSUFFICIENT | No sampling possible; source ungradeable — treat as unknown reliability |

## 13. Common Analytical Mistakes

- Grading a publication by its best journalism rather than its base rate.
- Treating state media as automatically unreliable — some are precise recorders of official position (see `propaganda_analysis.md` for the distinction).
- Ignoring that a source can be reliable about one beat (court reporting) and fabricated about another (conflict).
- Letting a single viral debunk permanently mark a source F without review of error rate.

## 14. Ethical Considerations

Reliability grades can damage reputations. Grades must be evidence-bound, dated, and correctable. Anonymous analysts must not be targeted; low-reliability designations on individuals require a documented public-interest justification and review. Never grade sources to suppress lawful speech — grade them to calibrate confidence.

## 15. Security Boundaries

Assessment is passive: public records, published archives, official disclosures. No interaction with the source, no test submissions, no social engineering, no impersonation. Do not record personal data of journalists beyond professional-public information already published.

## 16. Expected Output

A `SOURCE_RELIABILITY_RECORD` per source containing: identifier, tier, grade (A–F), five-dimension scores, evidence citations, sample size, assessment date, analyst, confidence level, and review triggers. Records feed `source_citation_standards.md` and `verification_audit_trail.md`.

## 17. Quality Checklist

- [ ] Source type classified before grading
- [ ] ≥2 independent external signals cited
- [ ] Grade justified in writing, not asserted
- [ ] Assessment date and analyst recorded
- [ ] Confidence level stated
- [ ] Cross-linked to credibility scoring and provenance records
- [ ] No personal-data overreach

## 18. Cross-Reference Links

- Upstream: `primary_source_verification.md`, `secondary_source_verification.md`, `tertiary_source_handling.md`
- Parallel: `source_credibility_scoring.md`, `source_provenance_tracking.md`, `source_bias_assessment.md`
- Downstream: `claim_verification.md`, `evidence_confidence_scoring.md`, `source_citation_standards.md`
- Divisions: `osint/` (collection), `analytics/` (confidence models), `legal/` (defamation exposure), `reporting/` (grade presentation)
