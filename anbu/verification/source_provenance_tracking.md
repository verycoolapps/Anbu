# Source Provenance Tracking

**Division 007 · Verification · ANBU OSINT**

## 1. Purpose

Provenance tracking answers: *where did this piece of information come from, how did it travel, and can we prove the chain?* Every fact entering an ANBU product must carry a provenance record. This file defines the record format, the chain-of-custody rules, and the handling of broken or adversarial provenance.

## 2. Scope

Applies to all tiers — primary documents, secondary reports, tertiary posts, datasets, media files, and derived analyses. Also covers internal provenance: which analyst handled which item, when, and under what authorization.

## 3. Intelligence Objectives

- Make every claim auditable end-to-end: publication → capture → handling → citation.
- Detect provenance breaks that signal fabrication, laundering, or tampering.
- Support legal defensibility: demonstrate lawful acquisition and handling.
- Enable reuse: provenance records let future analysts re-verify without re-collecting.

## 4. Core Concepts

- **Chain of custody:** the documented sequence of possession from acquisition to analysis. Gaps are findings, not inconveniences.
- **Provenance vs. origin:** origin is where content was created; provenance is the documented path it took to reach ANBU. They can diverge (mirrors, reuploads, translations).
- **Derivative lineage:** every derivative (translation, excerpt, screenshot, AI summary) links to its parent and records what was changed.
- **Temporal provenance:** when each link in the chain occurred; timing anomalies are evidence.

## 5. Analytical Methodology

1. **Register at acquisition:** every item gets a provenance record before analysis begins.
2. **Record the acquisition event:** URL, timestamp (UTC), retrieval method, tool/version, operator.
3. **Link derivatives:** translations (`translation_verification.md`), excerpts, crops, transcriptions each reference the parent record.
4. **Track custody events:** exports, shares, edits, and reformatting are logged with actor and timestamp.
5. **Audit periodically:** sample records and verify links resolve; broken links trigger re-verification per `verification_audit_trail.md`.

## 6. Step-by-Step Workflow

1. Assign each item a persistent ID (e.g., `PROV-YYYYMMDD-NNNN`) at first capture.
2. Populate the provenance record: source URI, capture timestamp/hash, collector, acquisition method, legal basis note.
3. For media, record capture conditions (device, timezone, upload path) relevant to authenticity checks.
4. For documents, record repository, document identifiers, and hash.
5. On any transformation, create a derivative record referencing the parent.
6. On citation into a product, link the product section to the provenance record.

## 7. Data Requirements

- UTC timestamps for every event (capture, transform, cite).
- Cryptographic hashes (SHA-256) for binary files at acquisition.
- Actor identity for every custody event.
- Parent/child links for all derivatives.
- Retention and deletion policy reference per `legal/`.

## 8. Approved Public Sources

Provenance records cite only lawfully acquired public material. Acquisition channels: direct public URLs, licensed databases, archive captures, platform public APIs within terms, lawful FOIA/public-records responses, and consented submissions. The acquisition method is part of the record — "obtained via X" is mandatory.

## 9. Source Verification Standards

A provenance chain is complete when every hop from original publication to ANBU citation is documented with timestamps and actors. Incomplete chains are labeled: `CHAIN-INCOMPLETE` (some hops missing) or `CHAIN-BROKEN` (a hop is contradicted by evidence). Neither label is fatal — it sets the confidence ceiling.

## 10. Analytical Framework

Maintain the **Provenance Graph**: nodes are items and events, edges are custody/derivation relations. Periodically check for: orphaned items (no parent), cycles (impossible lineage), timestamp inversions, and hash mismatches. Anomalies feed `manipulated_media_assessment.md` and fraud analysis.

## 11. Evidence Requirements

A provenance record is itself evidence and must include: record ID, all fields above, the operator's attestation, and links to `evidence_chain_management.md` where the item supports a claim. Records are append-only; corrections create new entries referencing the original.

## 12. Confidence Assessment

| Level | Criteria |
|---|---|
| HIGH | Complete chain, hashes verified, custody unbroken |
| MODERATE | Minor gaps (e.g., mirror hop undocumented) but content authenticated |
| LOW | Chain incomplete or relies on unverifiable intermediaries |
| INSUFFICIENT | No provenance record — item is a lead, not evidence |

## 13. Common Analytical Mistakes

- Recording only the final URL, losing the earlier hops that matter for verification.
- Treating a hash of a screenshot as equivalent to a hash of the original file.
- Forgetting that search-engine caches and aggregators create undocumented derivative hops.
- Letting provenance records become a dumping ground instead of a queryable graph.

## 14. Ethical Considerations

Provenance records may contain personal data of collectors and sources. Apply data-minimization: record role, not unnecessary identity detail. Records must not become a tool for tracking individuals beyond legitimate case needs; access is role-restricted per `security/`.

## 15. Security Boundaries

Provenance infrastructure is access-controlled; integrity is protected (append-only or hash-chained log). No provenance record may be edited after attestation — corrections are superseding entries. Export of provenance data follows `legal/` review for personal-data exposure.

## 16. Expected Output

A provenance register (database or structured files) where every cited item resolves to a complete record; periodic audit reports listing chain anomalies; derivative lineage maps for translated or excerpted material.

## 17. Quality Checklist

- [ ] Every analyzed item has a provenance record
- [ ] Hashes captured for binary content
- [ ] Derivatives linked to parents
- [ ] Custody events complete with actors and timestamps
- [ ] Chain status labeled (COMPLETE / INCOMPLETE / BROKEN)
- [ ] Append-only discipline observed

## 18. Cross-Reference Links

- Core records: `evidence_chain_management.md`, `verification_audit_trail.md`
- Content checks: `image_authenticity_assessment.md`, `video_authenticity_assessment.md`, `document_authenticity_assessment.md`, `translation_verification.md`, `publication_date_verification.md`
- Source tiers: `primary_source_verification.md`, `secondary_source_verification.md`, `tertiary_source_handling.md`
- Divisions: `osint/` (acquisition), `legal/` (retention/privacy), `security/` (access control), `reporting/` (citation)
