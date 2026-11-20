# Document Authenticity Assessment

**Division 007 · Verification · ANBU OSINT**

## 1. Purpose

Documents — PDFs, scans, spreadsheets, official forms, leaked files — are primary-source material when authentic and fabrication vectors when not. This file defines the workflow for assessing whether a document is genuine, altered, fabricated, or misattributed, and for establishing its provenance.

## 2. Scope

Covers digital documents (PDF, DOCX, XLSX, images of documents), scanned paper records, official publications, and leaked document sets. Email authenticity checks (headers, authentication results) are covered where they bear on document claims.

## 3. Intelligence Objectives

- Determine document status: GENUINE / ALTERED / FABRICATED / UNVERIFIABLE / MISATTRIBUTED.
- Authenticate official documents against issuing-authority records.
- Detect anachronisms: fonts, software artifacts, metadata, and content that postdate the claimed creation.
- Establish chain of custody for leaked or sensitive documents.

## 4. Core Concepts

- **Metadata forensics:** PDF producer/creator fields, software version anachronisms, font embedding inconsistencies, incremental-update history, and creation/modification timestamp analysis.
- **Content forensics:** formatting inconsistencies (font changes mid-document, alignment drift), language/register anomalies, numerical impossibilities, and knowledge anachronisms (references to events after the claimed date).
- **Provenance authentication:** does the document exist in an official repository, or does its claimed source corroborate it? A document matching an official record is authenticated regardless of file-level forensics.
- **Fabricated documents are designed to be plausible:** modern fabrications use genuine templates and correct formatting; detection relies on anomalies a fabricator missed.

## 5. Analytical Methodology

1. **Preserve:** hash file; record acquisition source and path.
2. **Extract metadata:** full PDF/DOCX metadata, embedded files, incremental updates, producer chains.
3. **Content inspection:** formatting consistency, anachronistic references, numerical/date coherence, signature/seal plausibility.
4. **Repository check:** search official sources for the document or its identifiers (publication number, form number, docket reference).
5. **Provenance verification:** for leaked docs, establish custody chain; for official docs, verify against issuing authority.
6. **Expert escalation:** where stakes are high and capability is exceeded, flag for external expert review rather than guessing.
7. **Verdict:** per matrix below with named checks and confidence.

## 6. Step-by-Step Workflow

1. Receive document; hash and snapshot; record acquisition provenance.
2. Run metadata extraction; log all fields, especially software versions vs. claimed date.
3. Inspect content: fonts, formatting, page geometry, language, internal references, dates.
4. Check for anachronisms: software that didn't exist, fonts released later, events referenced before they occurred.
5. Repository verification: does an official copy exist? Does the claimed issuing authority confirm?
6. For scans: check paper texture, print artifacts, handwriting consistency where relevant.
7. Issue verdict card; file in audit trail; preserve exhibit.

## 7. Data Requirements

- Original file with hash + acquisition record.
- Full metadata extraction output.
- Claimed provenance (issuing authority, date, context).
- Repository search results.
- Anachronism analysis notes.

## 8. Approved Public Sources

Official repositories and gazettes, standards bodies (for form templates), software release histories (for anachronism checks), font foundries (release dates), archive.org captures, court record systems, and academic document-forensics literature. For leaked materials, public leak archives with documented custody.

## 9. Source Verification Standards

GENUINE requires either official-repository confirmation or forensic cleanliness across all checks with consistent provenance. ALTERED requires affirmative evidence of modification post-creation. FABRICATED requires evidence the document could not exist as claimed (anachronisms, template mismatch, provenance impossibility). When checks conflict, the verdict is the more conservative status with dissent documented.

## 10. Analytical Framework

Use the **Document Verdict Matrix**: provenance status × metadata findings × content forensics × repository match → verdict. Documents authenticating to official repositories are GENUINE even with odd file metadata (re-saves happen); documents with clean metadata but failed provenance are UNVERIFIABLE at best.

## 11. Evidence Requirements

Verdict cards include: file hash, acquisition record, metadata report, forensic check list (named), anachronism findings, repository search results, verdict, confidence. Documents supporting claims link via `evidence_chain_management.md` with page/section locators.

## 12. Confidence Assessment

| Level | Criteria |
|---|---|
| HIGH | Official-repository match OR multiple convergent forensic indicators |
| MODERATE | Forensic-clean document with plausible but unconfirmed provenance |
| LOW | Ambiguous findings; benign explanations exist |
| INSUFFICIENT | Document too degraded or checks inapplicable — UNVERIFIABLE |

## 13. Common Analytical Mistakes

- Assuming official-looking formatting equals authenticity.
- Treating missing metadata as suspicious (many legitimate producers strip it).
- Ignoring anachronisms in content (the strongest fabrication signal).
- Declaring fabrication on a single anomaly without considering re-save/edit history.
- Failing to check whether the document's identifiers exist in official indexes.

## 14. Ethical Considerations

Document verdicts can accuse individuals of forgery — a serious claim. Publish only HIGH-confidence verdicts publicly; preserve originals; minimize exposure of sensitive personal data in exhibits; follow `legal/` for leaked-material handling.

## 15. Security Boundaries

Assessment of provided files only. Do not open documents with active content (macros, embedded executables); extract text/metadata statically. Do not distribute leaked documents beyond the analysis need-to-know.

## 16. Expected Output

Document verdict cards, exhibit archive entries, authentication certificates for official documents, and integration into `claim_verification.md` for document-supported claims.

## 17. Quality Checklist

- [ ] Original hashed and preserved
- [ ] Metadata fully extracted and analyzed
- [ ] Content forensics performed (fonts, formatting, anachronisms)
- [ ] Repository verification attempted
- [ ] Provenance chain documented
- [ ] Verdict + confidence with named checks

## 18. Cross-Reference Links

- Parent: `manipulated_media_assessment.md`, `primary_source_verification.md`
- Related: `publication_date_verification.md`, `translation_verification.md`, `quotation_verification.md`
- Intent: `disinformation_detection.md` (forged documents in operations)
- Records: `source_provenance_tracking.md`, `evidence_chain_management.md`, `verification_audit_trail.md`
- Divisions: `legal/` (document handling), `security/` (sensitive materials), `reporting/`
