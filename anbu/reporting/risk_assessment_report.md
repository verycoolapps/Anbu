# Risk Assessment Report

**Module:** ANBU OSINT — Reporting Division
**File:** reporting/risk_assessment_report.md
**Division:** Reporting · **Product class:** Analytics
**Classification handling:** Apply research data classification rules to all outputs. All stored products must carry an analyst-assigned classification label.

## 1. Purpose

Structured risk analysis: likelihood, impact, exposure, and mitigation-relevant context for a defined subject or portfolio. This template standardizes the product so that any ANBU analyst can produce a consistent, auditable deliverable.

## 2. Scope

In scope: the structure, content requirements, evidence discipline, and quality gate for this product type. Out of scope: the subject-matter tradecraft itself, which lives in the relevant division (`core/`, `analytics/`, `verification/`, `osint/`, `political/`, `military/`, `state/`, `geopolitical/`, `geoint/`, `legal/`, `security/`).

## 3. Intelligence objectives

- Likelihood × impact grading
- Exposure and vulnerability decomposition
- Cascading and correlated risk identification
- Risk-acceptance context (who bears it)

Deliver a graded risk assessment that ranks risks by decision relevance and states assessment confidence.

## 4. Core concepts

This product consumes the ANBU evidence vocabulary defined in [`core/intelligence_framework.md`](../core/intelligence_framework.md): every claim carries exactly one label — FACT, VERIFIED, UNVERIFIED, ASSESSMENT, INFERENCE, HYPOTHESIS, or SPECULATION. Products are hypothesis-driven: alternatives are generated before conclusions, and evidence is sought that discriminates between them.

Risk assessment informs; it does not decide risk appetite — that is the decision-maker's role.

## 5. Analytical methodology

- Triangulate claims across independent source classes before grading
- Apply the evidence vocabulary to every claim
- Generate and test competing hypotheses before drafting conclusions
- Record disconfirming evidence, not only confirming evidence
- Grade confidence at section level, then roll up

## 6. Step-by-step workflow

1. Define the question, decision context, and scope boundaries; record them in RESEARCH OBJECTIVES.
2. Generate candidate hypotheses (minimum two) and map discriminating evidence to each.
3. Collect and label items; record provenance for every source used.
4. Draft VERIFIED FACTS and SOURCE ASSESSMENT sections before writing analysis.
5. Write ANALYSIS against the hypothesis matrix; record rejected alternatives.
6. Build RISK ASSESSMENT, FUTURE SCENARIOS, and INDICATORS TO MONITOR.
7. Fill INFORMATION GAPS and LIMITATIONS honestly; do not paper over them.
8. Assign ANALYTICAL CONFIDENCE per section and for the product as a whole.
9. Assemble in the canonical 20-section order (below); run the quality checklist.
10. Release with classification label, version, date, and reviewer sign-off.

## 7. Data requirements

Risk registers from prior products, incident histories, regulatory filings, audit reports, expert assessments, insurance/actuarial data where public. All data must carry provenance: source identifier, retrieval date, collection method, and handling notes per `core/intelligence_framework.md`.

## 8. Approved public sources

Risk registers from prior products, incident histories, regulatory filings, audit reports, expert assessments, insurance/actuarial data where public. Sources must be permitted under ANBU collection rules; see [`osint/`](../osint/) for collection tradecraft and [`security/safe_public_source_handling.md`](../security/safe_public_source_handling.md) for handling rules.

## 9. Source verification standards

Likelihood estimates anchored to base rates where available; impact assessed separately from probability. Verification outcomes are documented per claim; see [`verification/`](../verification/) and [`source_verification_report.md`](source_verification_report.md).

## 10. Analytical framework

This product uses the ANBU framework in [`core/intelligence_framework.md`](../core/intelligence_framework.md): ACH (Analysis of Competing Hypotheses), capability–intent separation, and explicit falsification conditions. Product-specific application: Risk assessment informs; it does not decide risk appetite — that is the decision-maker's role.

## 11. Evidence requirements

Risk register format: risk statement, drivers, likelihood, impact, confidence, indicators, owner-context. Minimum evidence bar for any ASSESSMENT-grade claim: at least two labeled items, at least one VERIFIED or high-quality FACT, plus a statement of what is missing.

## 12. Confidence assessment

Per-risk confidence; overall confidence is weakest-link per material risk.

## 13. Common analytical mistakes

- Low-probability/high-impact neglect; correlated risks treated as independent; mitigation advice drifting into operations.
- Risk = hazard confusion
- Single-number scores hiding uncertainty
- Ignoring second-order effects
- Unstated risk appetite assumptions
- Section-level omissions disguised as brevity
- Confidence inflation: stating HIGH where the evidence chain has a weak link
- Mixing observation and inference in a single unlabeled sentence

## 14. Ethical considerations

Products in this class handle sensitive subjects. Apply [`legal/ethical_review_checklist.md`](../legal/ethical_review_checklist.md), [`legal/political_neutrality_policy.md`](../legal/political_neutrality_policy.md), and [`security/targeting_and_harm_prevention.md`](../security/targeting_and_harm_prevention.md). Never include material that enables targeting, harassment, or harm; redact personal identifiers per [`security/personal_identifier_protection.md`](../security/personal_identifier_protection.md).

## 15. Security boundaries

- Public sources only; no classified material, no credential misuse, no unauthorized access.
- Evidence handling per [`security/evidence_integrity_management.md`](../security/evidence_integrity_management.md): hash at intake, custody log, working copies only.
- Storage per [`security/secure_document_storage.md`](../security/secure_document_storage.md) with analyst-assigned classification.
- No operational guidance of any kind; analysis stops at posture and trend level.

## 16. Expected output

A graded analytical product in the canonical 20-section structure (template below), with inline `[N]` citations resolving to the Sources and References section, per-section confidence statements, and a release block: classification, version, date, analyst, reviewer.

## 17. Quality checklist

- [ ] All 20 sections present in order (or explicitly marked N/A)
- [ ] Every claim labeled with the evidence vocabulary
- [ ] Every factual claim carries an inline citation
- [ ] Confidence stated per section and overall (HIGH/MODERATE/LOW/INSUFFICIENT)
- [ ] Alternative hypotheses documented with disconfirming evidence
- [ ] Information gaps and limitations stated honestly
- [ ] No operational/targeting content
- [ ] Privacy and defamation guardrails applied
- [ ] Release block complete (classification, version, date, analyst, reviewer)
- [ ] Peer review sign-off recorded

## 18. Canonical 20-Section Report Structure

## ANBU Intelligence Report — Canonical 20-Section Structure

Every ANBU intelligence report follows this fixed section order. Sections may be condensed for short-cycle products, but the order and labels are never changed, and no section is silently omitted — write "No findings" or "Not applicable" where required.

1. EXECUTIVE SUMMARY — the graded bottom line, decision context, and headline confidence.
2. KEY FINDINGS — the discriminating facts and assessments, each with a source label.
3. RESEARCH OBJECTIVES — the questions posed, the decision context, and scope boundaries.
4. BACKGROUND — historical and institutional context needed to read the analysis.
5. VERIFIED FACTS — items graded VERIFIED or high-quality FACT, with citations.
6. SOURCE ASSESSMENT — evaluation of each source class used; strengths, limits, bias indicators.
7. INSTITUTIONAL CONTEXT — the organizations, mandates, and constraints shaping the subject.
8. ANALYSIS — hypothesis-driven reasoning; state alternatives before conclusions.
9. KEY STAKEHOLDERS — actors with interest and influence; roles, not verdicts on persons.
10. HISTORICAL DEVELOPMENT — relevant trajectory; continuity and change.
11. CURRENT SITUATION — dated snapshot of verified state as of reporting.
12. STRATEGIC IMPLICATIONS — what the findings mean for the decision context.
13. RISK ASSESSMENT — graded risks with likelihood, impact, and confidence.
14. ALTERNATIVE HYPOTHESES — competing explanations not selected, with evidence against them.
15. FUTURE SCENARIOS — bounded scenarios with indicators, not predictions.
16. INDICATORS TO MONITOR — observable, checkable early signals per scenario.
17. INFORMATION GAPS — what is unknown, why it matters, and how it could be filled legally.
18. ANALYTICAL CONFIDENCE — source / information / analytical confidence, stated separately.
19. LIMITATIONS — methodological, collection, and ethical limits of this product.
20. SOURCES AND REFERENCES — full citation list in ANBU citation format.

## Writing Standards and Tone

- **Tone:** calm, precise, evidence-first. No sensationalism, no advocacy, no operational advice.
- **Labels:** every claim carries the evidence vocabulary (FACT, VERIFIED, ASSESSMENT, INFERENCE, HYPOTHESIS, UNVERIFIED, SPECULATION) per `core/intelligence_framework.md`.
- **Citation format:** `[N]` inline markers; full entries in Sources and References with author/organization, title, publication or repository, date, URL or stable identifier, and access date.
- **Confidence:** stated as HIGH / MODERATE / LOW / INSUFFICIENT per the assessment protocol in this file.
- **Separation:** observation, inference, and speculation are never blended in a single sentence.

## Confidence Assessment Protocol

| Level | Standard |
|---|---|
| HIGH | Multiple independent VERIFIED items; hypothesis survives best available alternative explanations; gaps are peripheral. |
| MODERATE | Core claims corroborated; significant secondary elements rest on single or official sources; alternatives remain plausible. |
| LOW | Thin corroboration; key claims UNVERIFIED or single-source; high dependence on inference. |
| INSUFFICIENT | Evidence cannot support the requested assessment; product should report gaps, not conclusions. |


## 19. Citation format

Inline markers `[N]` appear at the claim they support. The Sources and References section lists each source as:

`[N] Author/Organization. "Title." Publication or repository, date. URL or stable identifier. Accessed YYYY-MM-DD.`

Rules: cite the most specific available source; prefer primary over secondary; never cite a source you did not retrieve; archive-unstable pages get an archive reference.

## 20. Cross-references

Sibling products:
- [`executive_intelligence_brief.md`](executive_intelligence_brief.md) · [`strategic_intelligence_report.md`](strategic_intelligence_report.md) · [`political_intelligence_report.md`](political_intelligence_report.md)
- [`military_defense_report.md`](military_defense_report.md) · [`geopolitical_assessment_report.md`](geopolitical_assessment_report.md) · [`government_institution_report.md`](government_institution_report.md)
- [`country_profile_report.md`](country_profile_report.md) · [`country_comparison_report.md`](country_comparison_report.md) · [`conflict_analysis_report.md`](conflict_analysis_report.md)
- [`defense_budget_report.md`](defense_budget_report.md) · [`policy_assessment_report.md`](policy_assessment_report.md) · [`intelligence_gap_report.md`](intelligence_gap_report.md)
- [`source_verification_report.md`](source_verification_report.md) · [`early_warning_report.md`](early_warning_report.md) · [`scenario_analysis_report.md`](scenario_analysis_report.md)
- [`leadership_public_record_profile.md`](leadership_public_record_profile.md) · [`institutional_network_report.md`](institutional_network_report.md) · [`intelligence_dashboard_specification.md`](intelligence_dashboard_specification.md)
- [`reporting_quality_checklist.md`](reporting_quality_checklist.md)

Upstream inputs:
- [`core/intelligence_framework.md`](../core/intelligence_framework.md) — evidence vocabulary and analytic cycle
- [`analytics/`](../analytics/) — tradecraft modules feeding this product
- [`verification/`](../verification/) — authentication and corroboration standards

Quality gate:
- [`reporting_quality_checklist.md`](reporting_quality_checklist.md) — acceptance checklist for all products
