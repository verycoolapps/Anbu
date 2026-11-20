# Cross-Source Corroboration

**Division 007 · Verification · ANBU OSINT**

## 1. Purpose

Corroboration is the process of establishing that independent sources agree on a claim. It is the primary mechanism by which unverified material graduates toward usable confidence. This file defines what counts as *independent* corroboration, how to search for it systematically, and how to avoid the most dangerous verification failure: mistaking echoes for agreement.

## 2. Scope

Applies to any claim with fewer than two independent confirmations. Covers news, official records, datasets, media content, and social posts. Complements `claim_verification.md` (single-claim adjudication) and feeds `evidence_confidence_scoring.md`.

## 3. Intelligence Objectives

- Systematically find independent agreement or disagreement for material claims.
- Map the true origin structure of apparently multi-source claims.
- Detect coordinated amplification masquerading as corroboration.
- Produce an honest corroboration count that survives audit.

## 4. Core Concepts

- **Independence:** two sources are independent only if neither derived its information from the other and they do not share an owner, wire service, or editorial chain.
- **Common-origin collapse:** five outlets rewriting one wire dispatch = one source, not five. Verify origin before counting.
- **Negative corroboration:** independent sources agreeing the claim is *false* is as valuable as agreement it is true.
- **Partial corroboration:** sources may agree on the event but differ on details; score the specific proposition, not the headline.

## 5. Analytical Methodology

1. **Extract the minimal proposition:** strip the claim to its testable core (who, what, when, where).
2. **Search for agreement:** keyword variants, translated equivalents, distinctive details (names, numbers, locations).
3- **For each hit, trace origin:** does it cite a common source? Check wire credits, press-release language, identical phrasing.
4. **Classify each source:** independent / derivative-of-X / unknown-origin.
5. **Count true independents:** only independent sources with compatible claims count.
6. **Record disagreement:** independent contradictions are logged and weighed per `conflicting_evidence_resolution.md`.

## 6. Step-by-Step Workflow

1. Define the proposition precisely; ambiguous claims are split into sub-claims.
2. Run multi-language and multi-platform searches; OSINT claims often corroborate across language boundaries first.
3. For news hits, inspect sourcing: does the article cite documents, officials, or just "reports"?
4. Build the origin map: cluster sources by shared attribution.
5. Assign corroboration level: NONE / SINGLE-INDEPENDENT / MULTI-INDEPENDENT / OFFICIAL-CONFIRMED.
6. Log the search methodology (queries, date, platforms) in the audit trail for reproducibility.

## 7. Data Requirements

- Precise proposition statement.
- Search log: queries, platforms, languages, date executed.
- For each candidate source: URL, timestamp, ownership/affiliation, attribution chain.
- Origin-map output showing clusters and independents.

## 8. Approved Public Sources

All public tiers are valid corroboration targets, weighted by independence and reliability: official records, established outlets, niche specialists, and — with care — authenticated tertiary items. Corroboration across *different tiers* (e.g., official record + independent journalism) is stronger than same-tier repetition.

## 9. Source Verification Standards

A source counts toward corroboration only after its own reliability grade is on file and its independence from other counted sources is established. "Multiple sources" without an origin map is not corroboration — it is a hypothesis about corroboration.

## 10. Analytical Framework

Use the **Corroboration Matrix**: rows = sources, columns = claim elements. Agreement on all elements = strong corroboration; agreement on the core but divergence on details = partial; agreement only on a vague generalization = weak. Score per `source_credibility_scoring.md` input 3.

## 11. Evidence Requirements

Corroboration must be documented with: the proposition, the search log, the origin map, the list of independent agreeing sources (with URLs/timestamps), and the list of disagreeing sources. Undocumented corroboration counts are void.

## 12. Confidence Assessment

| Level | Criteria |
|---|---|
| HIGH | ≥2 truly independent sources, ideally different tiers, no unresolved contradiction |
| MODERATE | 1 independent source plus partial secondary agreement, or independents with minor detail conflicts |
| LOW | Agreement exists but all sources trace to one origin |
| INSUFFICIENT | No corroboration found — treat claim as single-source |

## 13. Common Analytical Mistakes

- Counting a press release and the twenty articles it generated as twenty-one sources.
- Treating translation of the same story as independent corroboration.
- Ignoring that two outlets under common ownership are not independent.
- Stopping the corroboration search after finding agreement — adversarial claims often have a hidden contradicting record.
- Confusing correlation in timing with corroboration of content.

## 14. Ethical Considerations

Corroboration work must not become a tool for manufacturing consensus — e.g., selectively citing agreeing sources while omitting documented contradictions. Symmetric search (looking for both confirmation and refutation) is mandatory for material claims.

## 15. Security Boundaries

Corroboration is passive research. Do not contact sources to confirm claims secondhand, do not create sock-puppet accounts to "test" claims, and do not access private channels. Log all queries for audit.

## 16. Expected Output

A corroboration record per material claim: proposition, origin map, independent-source list, corroboration level, disagreeing sources, search log, and resulting confidence input for the claim card.

## 17. Quality Checklist

- [ ] Proposition stated minimally and precisely
- [ ] Origin map completed before counting sources
- [ ] Independence of each counted source verified
- [ ] Disagreement search performed symmetrically
- [ ] Search methodology logged
- [ ] Corroboration level assigned with justification

## 18. Cross-Reference Links

- Inputs: `primary_source_verification.md`, `secondary_source_verification.md`, `tertiary_source_handling.md`, `source_reliability_assessment.md`
- Conflicts: `conflicting_evidence_resolution.md`
- Downstream: `claim_verification.md`, `source_credibility_scoring.md`, `evidence_confidence_scoring.md`
- Threats: `disinformation_detection.md` (coordinated amplification), `propaganda_analysis.md`
- Divisions: `osint/` (search), `analytics/` (scoring), `reporting/` (presentation)
