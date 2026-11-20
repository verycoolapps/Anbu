# Secondary Source Verification

**Division 007 · Verification · ANBU OSINT**

## 1. Purpose

Secondary sources interpret, report on, or summarize events documented elsewhere: journalism, think-tank analysis, academic papers, expert commentary, and reference works. They are essential for discovery and context but must never stand alone as evidence for a factual claim. This file defines how ANBU verifies secondary material before letting it shape analysis.

## 2. Scope

Covers: news reporting, investigative journalism, think-tank and NGO reports, academic secondary literature, encyclopedias, fact-check articles (which are themselves secondary assessments), and expert opinion. Distinct from primary records (`primary_source_verification.md`) and from unvetted user-generated content (`tertiary_source_handling.md`).

## 3. Intelligence Objectives

- Extract leads and hypotheses from secondary material without inheriting its errors.
- Trace each secondary claim back toward primary evidence or mark it unverifiable.
- Evaluate the secondary source's own reliability grade and incentive structure.
- Detect when "consensus" reporting is actually one wire story multiplied.

## 4. Core Concepts

- **Derivative risk:** most secondary errors are inherited from an earlier unverified claim, not originated.
- **Attribution laundering:** "experts say," "reports suggest" — phrases that hide the actual source. Strip them during extraction.
- **Echo-chamber corroboration:** apparent multi-source agreement that traces to a single origin. See `cross_source_corroboration.md`.
- **Secondary as map, not territory:** journalism tells you where to dig; the primary record tells you what is there.

## 5. Analytical Methodology

1. **Classify** the secondary source: reported journalism, analysis, opinion, reference, or advocacy.
2. **Extract testable claims** and strip unattributed attributions.
3. **Grade source reliability** per `source_reliability_assessment.md`.
4. **Trace to primary:** for each material claim, attempt to locate the underlying primary record.
5. **Score credibility** per `source_credibility_scoring.md`; record which claims remain unanchored.
6. **Log derivatives:** note which other outlets carry the same claim, and whether they share an origin.

## 6. Step-by-Step Workflow

1. Capture the secondary item: URL, publication, author, timestamp, access date.
2. Identify the claim(s) it contributes to the dossier; quote exactly.
3. Check whether the outlet grades A–C; if D/F, downgrade all its claims by one band unless independently corroborated.
4. Follow the attribution chain: who does the article cite? Is that source primary, secondary, or unnamed?
5. Search for the primary record per `primary_source_verification.md`; record found/not-found.
6. File a claim card noting secondary status and corroboration state.

## 7. Data Requirements

- Full citation metadata for the secondary item.
- Author identity and beat expertise where published.
- Outbound attribution list (whom the piece cites).
- Inbound derivative map: who else published the same claim (reverse-search the distinctive phrasing).

## 8. Approved Public Sources

Established news organizations, peer-reviewed journals, university presses, major wire services, reputable think tanks (with methodology disclosure), government statistical publications, and recognized fact-checking organizations. Advocacy outlets are usable as sources *about their own position*, never as neutral evidence.

## 9. Source Verification Standards

Secondary sources must clear three gates before their claims enter analysis: (1) source reliability grade assigned, (2) primary-source trace attempted and result logged, (3) derivative/origin analysis completed for corroboration purposes. Skipping any gate leaves claims in a provisional state.

## 10. Analytical Framework

Apply the **Attribution Trace**: claim → article → cited source → primary record. Each hop is logged with reliability. A claim that dies at an unnamed hop is scored on its weakest verified ancestor, not on the polish of the final write-up.

## 11. Evidence Requirements

For every secondary citation: exact quote, publication timestamp, author, outlet reliability grade, the primary-source search result (found URL or documented failure), and the derivative map summary. "Verified by secondary consensus" is not an acceptable evidence statement.

## 12. Confidence Assessment

| Level | Criteria |
|---|---|
| HIGH | Secondary claim traced to authenticated primary record |
| MODERATE | Multiple independent secondaries agree, primary trace incomplete |
| LOW | Single secondary, or secondaries sharing a common origin |
| INSUFFICIENT | Secondary claim with no traceable origin and no corroboration — lead only |

## 13. Common Analytical Mistakes

- Citing a news report of a leaked document without examining the document.
- Counting syndicated content across outlets as independent corroboration.
- Trusting a prestigious outlet's analysis of a domain it does not cover.
- Letting a well-written secondary claim outrank a poorly formatted but authentic primary record.

## 14. Ethical Considerations

Journalists and researchers deserve accurate characterization. Record errors precisely; do not imply fabrication when the actual failure was sloppy attribution. Criticism of outlets should cite documented standards violations, not political disagreement.

## 15. Security Boundaries

Read-only review of published material. No contacting journalists as a pretext for verification, no pre-publication review demands, no use of leaked credentials or paywall bypass where lawful access exists.

## 16. Expected Output

Verified secondary citations with trace results, a derivative/origin map for corroborated claims, and a list of unanchored secondary claims flagged as leads for `osint/` collection tasks.

## 17. Quality Checklist

- [ ] Outlet graded for reliability
- [ ] Claims extracted verbatim, attributions stripped
- [ ] Primary trace attempted and logged
- [ ] Derivative map completed before counting corroboration
- [ ] Confidence band assigned per claim
- [ ] Unanchored claims marked as leads, not facts

## 18. Cross-Reference Links

- Feeds from: `osint/` collection, `tertiary_source_handling.md`
- Relies on: `primary_source_verification.md`, `source_reliability_assessment.md`, `source_credibility_scoring.md`
- Feeds into: `cross_source_corroboration.md`, `claim_verification.md`, `fact_checking_methodology.md`
- Divisions: `reporting/` (secondary citation norms), `legal/` (defamation), `analytics/` (confidence)
