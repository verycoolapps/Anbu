# Source Citation Standards

**Division 007 · Verification · ANBU OSINT**

## 1. Purpose

Citations are the interface between analysis and audit: they let consumers verify claims, let reviewers trace reasoning, and let ANBU demonstrate that its products rest on documented evidence. This file defines the mandatory citation format for every ANBU product — covering footnotes, URLs, access dates, and evidence references.

## 2. Scope

Covers all citation types: web sources, documents, datasets, media exhibits, official records, archived captures, and internal evidence records. Applies to every product in `reporting/` and every internal document where claims appear.

## 3. Intelligence Objectives

- Make every factual claim traceable to its source in one step.
- Preserve citability over time: links decay, so captures and identifiers are mandatory where possible.
- Standardize citation so any analyst can produce audit-ready references.
- Support legal defensibility: citations must demonstrate what was relied upon and when.

## 4. Core Concepts

- **Citation ≠ evidence:** a citation points to evidence; the evidence chain (`evidence_chain_management.md`) holds the actual items. Citations must resolve.
- **Link rot:** URLs die; archive captures and persistent identifiers (DOI, document numbers) preserve access.
- **Access dates are mandatory:** web content changes; "accessed YYYY-MM-DD" is required on every URL citation.
- **Tier-aware citation:** primary sources are cited directly; secondary citations note their derivative status and the primary they derive from where known.

## 5. Analytical Methodology

1. **Identify the claim:** every factual assertion gets at least one citation.
2. **Select the best source:** cite the highest-tier source that supports the specific claim (primary > secondary > tertiary).
3. **Format per standard:** apply the citation template with all required fields.
4. **Verify resolution:** confirm the citation resolves at publication time; record archive capture where link rot is likely.
5. **Link internally:** connect citations to evidence IDs and provenance records.
6. **Audit:** review pass confirms every claim has citations and every citation resolves.

## 6. Step-by-Step Workflow

1. Draft product with inline citation markers.
2. For each marker, assemble the full citation: author/institution, title, publication date, URL/identifier, access date, locator (page/timestamp/section).
3. Apply format template (see §10); add archive capture for volatile sources.
4. Resolve-check every URL; replace dead links with archive captures.
5. Cross-link citation to evidence ID in the manifest.
6. Final audit: claim-to-citation coverage check; publish.

## 7. Data Requirements

- Claim inventory for the product.
- Full source metadata for every cited item.
- Access dates for all URLs.
- Archive captures for volatile or likely-to-rot sources.
- Evidence IDs for internal cross-reference.

## 8. Approved Public Sources

Citations reference the standard public-source universe. For citation infrastructure: DOI resolvers, persistent identifiers, Internet Archive captures, and official document repositories are preferred over ephemeral URLs.

## 9. Source Verification Standards

A citation is valid only if: (a) it resolves at publication, (b) it contains all required fields, (c) it supports the specific claim it's attached to (not just the general topic), (d) it reflects the source's actual tier and reliability. Citations meeting these standards are audit-ready.

## 10. Analytical Framework

**Citation template (web):** Author/Institution. "Title." *Publication*, date. URL. Accessed date. [Evidence ID; Tier; Confidence band].

**Citation template (document):** Issuing authority. *Document title*, identifier/number, date. Repository. Locator (page/section). Accessed date. [Evidence ID].

**Citation template (media):** Creator/uploader. "Description." Platform, date. URL/timecode. [Evidence ID; authenticity verdict].

All citations link to `source_provenance_tracking.md` records.

## 11. Evidence Requirements

Citation lists must be complete (every claim covered), resolvable (links/captures work), and honest (tier and confidence stated). Footnote-style citations are acceptable for print formats; evidence-ID linking is mandatory for digital products.

## 12. Confidence Assessment

Citation quality is binary-auditable: VALID (all fields, resolves, supports claim) or DEFICIENT (missing fields, dead link, mismatched support). Products with any DEFICIENT citations in load-bearing claims cannot ship until corrected.

## 13. Common Analytical Mistakes

- Citing the homepage instead of the specific article/page.
- Omitting access dates on web citations.
- Citing a secondary source when the primary was available.
- Using citation as decoration — attaching sources that don't actually support the claim.
- Letting links rot without archive captures.
- Inconsistent formatting across a product.

## 14. Ethical Considerations

Citations must not expose sources to harm: anonymous sources get protective citation practices per `legal/`; sensitive documents are cited by locator without republication. Accurate citation of opponents' sources is required even when inconvenient — citation is not endorsement.

## 15. Security Boundaries

Citation lists may reveal collection methods or sources; security-sensitive products get `security/` review before citation patterns are published. Do not cite non-public or improperly obtained material.

## 16. Expected Output

Complete citation lists per product, inline citations at point of claim, evidence-ID cross-references, archive captures for volatile sources, and citation-audit reports.

## 17. Quality Checklist

- [ ] Every factual claim has ≥1 citation
- [ ] All required fields present per template
- [ ] Access dates on all URLs
- [ ] Links resolve; archive captures for volatile sources
- [ ] Tier and confidence noted where relevant
- [ ] Evidence IDs cross-linked
- [ ] Consistent formatting throughout

## 18. Cross-Reference Links

- Evidence base: `evidence_chain_management.md`, `source_provenance_tracking.md`, `verification_audit_trail.md`
- Source standards: `primary_source_verification.md`, `secondary_source_verification.md`, `tertiary_source_handling.md`, `source_reliability_assessment.md`
- Consumers: `reporting/` (all formats), `legal/` (citation liability), `workflows/` (quality gates)
- Confidence: `evidence_confidence_scoring.md`, `source_credibility_scoring.md`
