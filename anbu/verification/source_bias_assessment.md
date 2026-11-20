# Source Bias Assessment

**Division 007 · Verification · ANBU OSINT**

## 1. Purpose

Bias assessment evaluates systematic tendencies in a source's selection, framing, emphasis, and omission — independent of whether individual claims are true. A truthful source can be systematically biased; a biased source can publish accurate facts. This file defines how ANBU detects, classifies, and records source bias so analysts can calibrate rather than naively trust or dismiss.

## 2. Scope

Covers political, commercial, institutional, national, ideological, and unconscious biases in any source type. Distinct from reliability (accuracy) and credibility (claim-level truth): bias is about systematic slant in what is covered and how.

## 3. Intelligence Objectives

- Identify systematic bias patterns that distort the information environment.
- Adjust confidence and interpretation for known-biased sources without discarding them.
- Detect when apparent corroboration is actually shared bias (sources with the same blind spots).
- Provide consumers with bias context for every significant source.

## 4. Core Concepts

- **Bias types:** selection bias (what stories get covered), framing bias (how they're presented), omission bias (what's left out), confirmation bias (source seeks confirming evidence), institutional bias (funding/ownership incentives), national bias (state-aligned framing).
- **Bias ≠ falsehood:** the goal is calibration, not censorship. A biased source remains usable for what it covers well.
- **Shared-bias detection:** multiple sources can be biased the same way; independence analysis must consider bias correlation (`cross_source_corroboration.md`).
- **Direction vs. magnitude:** record which direction bias leans and how strongly, per topic area — bias is domain-specific.

## 5. Analytical Methodology

1. **Profile the source:** ownership, funding, masthead, stated mission, audience, regulatory environment.
2. **Content sampling:** sample coverage over time; compare story selection against event population; note framing patterns.
3. **Omission analysis:** what significant events does the source not cover, or cover late/thinly?
4. **Language analysis:** loaded terms, passive/active voice choices, headline vs. body divergence.
5. **Compare against baseline:** coverage patterns vs. peer outlets and neutral reference points.
6. **Record bias profile:** direction, domains, magnitude estimate, evidence, confidence — filed per source.

## 6. Step-by-Step Workflow

1. Pull source profile data (ownership, funding, mission).
2. Sample 10–20 recent items across beats; log selection and framing patterns.
3. Identify omissions by comparing against event databases and peer coverage.
4. Classify bias types present; assign direction per domain.
5. Estimate magnitude (LOW/MODERATE/HIGH) with justification.
6. File bias profile; link to source reliability record; update when behavior changes.

## 7. Data Requirements

- Source ownership/funding/mission documentation.
- Content sample with dates and topics.
- Peer-comparison coverage data.
- Omission evidence (significant uncovered events).
- Language/framing examples with quotes.

## 8. Approved Public Sources

Media ownership databases, funding disclosures, regulatory filings, academic media-bias studies (with methodology scrutiny), ombudsman records, platform transparency reports, and the source's own published content. Bias assessments cite observable patterns, not accusations.

## 9. Source Verification Standards

Bias profiles require documented patterns: specific examples, sample sizes, and comparison baselines. "Everyone knows X is biased" is not an assessment. Profiles must be symmetric — apply the same framework to sources across the spectrum, and acknowledge ANBU's own potential biases in methodology notes.

## 10. Analytical Framework

Use the **Bias Vector**: direction (left/right/establishment/industry/national) × domain (domestic/foreign/economic/security) × magnitude × confidence. Vectors inform but do not determine credibility scores; a HIGH-bias source can still carry TRUE claims — flagged, not dismissed.

## 11. Evidence Requirements

Bias profiles include: source profile data, sample description, pattern examples with citations, omission evidence, comparison baseline, vector assignment, confidence. Profiles are dated and revisable.

## 12. Confidence Assessment

| Level | Criteria |
|---|---|
| HIGH | Large sample, multiple bias types documented, peer comparison complete |
| MODERATE | Moderate sample, clear patterns, some comparison |
| LOW | Small sample or single bias type — provisional profile |
| INSUFFICIENT | Insufficient data — no profile; treat as unknown bias |

## 13. Common Analytical Mistakes

- Confusing bias with unreliability — a biased source can be reliable about what it covers.
- Assuming only overtly partisan sources are biased; establishment and commercial biases are equally real.
- Applying uniform bias scores across domains where bias varies.
- Letting bias assessment become a pretext for dismissing accurate reporting.
- Ignoring ANBU's own selection biases in what gets collected and analyzed.

## 14. Ethical Considerations

Bias labels can be weaponized to discredit accurate journalism. Profiles must be evidence-bound, symmetric, and correctable. Do not create bias scores to serve political ends; the framework applies to all sources equally, including those ANBU finds congenial.

## 15. Security Boundaries

Bias assessment uses published content and public records only. No covert monitoring of journalists or outlets; no infiltration of editorial processes.

## 16. Expected Output

Per-source bias profiles linked to reliability records; bias-correlation notes for corroboration analysis; bias context fields in `reporting/` citations.

## 17. Quality Checklist

- [ ] Source profile documented
- [ ] Content sample adequate and described
- [ ] Patterns evidenced with examples
- [ ] Omissions tested against baselines
- [ ] Vector assigned with confidence
- [ ] Symmetric standards applied
- [ ] Profile dated and linked to reliability record

## 18. Cross-Reference Links

- Inputs: `source_reliability_assessment.md`, `cross_source_corroboration.md`, `source_credibility_scoring.md`
- Threat context: `propaganda_analysis.md`, `disinformation_detection.md`, `misinformation_detection.md`
- Claims: `claim_verification.md`, `conflicting_evidence_resolution.md`
- Records: `source_provenance_tracking.md`, `verification_audit_trail.md`, `source_citation_standards.md`
- Divisions: `reporting/` (bias disclosure), `analytics/` (bias-adjusted models), `legal/`
