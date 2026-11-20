# Primary Source Verification

**Division 007 · Verification · ANBU OSINT**

## 1. Purpose

Primary sources are the evidentiary bedrock of OSINT: documents, datasets, recordings, official statements, and direct observations created at the time and place of the event by a participant or witness. This file defines how ANBU locates, authenticates, and extracts claims from primary material before any secondary reporting is trusted.

## 2. Scope

Covers: government gazettes and budgets, court records, legislative transcripts, procurement and tender notices, corporate filings, academic datasets, satellite imagery metadata, original video/audio, leaked document caches (handled per `legal/` constraints), and firsthand testimony captured contemporaneously. Does not cover journalism about events (secondary) or commentary about sources (tertiary).

## 3. Intelligence Objectives

- Establish what actually happened, not what was reported to have happened.
- Anchor every major claim to at least one primary record wherever one exists.
- Detect when official primary records contradict each other (a high-value analytical signal in itself).
- Build provenance chains that survive adversarial scrutiny.

## 4. Core Concepts

- **Contemporaneity:** primary value degrades when the record was created after the fact for a different purpose (e.g., a memoir written years later).
- **Custody:** a document is only as good as the chain showing it was not altered. Track per `evidence_chain_management.md`.
- **Provenance ≠ authenticity:** a real leaked document can be misattributed; an authentic-sounding PDF can be fabricated. Both checks required.
- **Primary is not neutral:** budgets, indictments, and statements are authored with purpose. Verify content *and* motive via `source_bias_assessment.md`.

## 5. Analytical Methodology

1. **Identify candidate primary records** for the claim (who would have produced one?).
2. **Locate the record** in an official repository or archive; prefer canonical URLs over mirrors.
3. **Authenticate** using the checks in `document_authenticity_assessment.md` and `publication_date_verification.md`.
4. **Extract the relevant passage** verbatim; preserve page/section identifiers.
5. **Compare against secondary accounts**; log agreements and contradictions.
6. **Grade** the record (see `evidence_confidence_scoring.md`) and file.

## 6. Step-by-Step Workflow

1. From the claim, enumerate expected primary artifacts (order, invoice, minutes, dataset, footage).
2. Search official sources first: agency sites, gazette portals, court dockets, procurement registries, statistical offices.
3. If not found officially, check archival repositories (Internet Archive, national libraries, document caches) and record retrieval path.
4. Capture: URL, access date, file hash where available, page references, verbatim excerpt.
5. Cross-check document metadata (creation tools, fonts, formatting anomalies) per `document_authenticity_assessment.md`.
6. Record in `source_provenance_tracking.md`; mark whether the record is original, mirror, or derivative.

## 7. Data Requirements

- Canonical repository URL and retrieval timestamp.
- Document identifiers: publication number, docket ID, ISBN/DOI, dataset DOI, recording timestamp.
- For digital files: SHA-256 hash at acquisition.
- Page/line/section locator for every excerpt cited.

## 8. Approved Public Sources

Government portals and gazettes, national statistical offices, central banks, electoral commissions, court systems, legislative records, procurement/tender portals, academic repositories (arXiv, SSRN, institutional repositories), open government data portals, and established archival institutions. Social-media posts by verified officials count as *statements* (primary for what was said) but not as proof of underlying facts.

## 9. Source Verification Standards

A primary source must be (a) located at an authoritative repository or (b) accompanied by documented provenance for the copy used. Screenshots of documents are leads, not evidence — obtain the underlying file or an official confirmation. Wayback Machine captures are acceptable with capture timestamp recorded.

## 10. Analytical Framework

Use the **Primary-Record Ladder**: official record > contemporaneous official statement > contemporaneous participant account > later official account > later participant account > none. Each rung down reduces confidence by one band. Record which rung supports each claim in the claim card.

## 11. Evidence Requirements

Every primary citation requires: exact title/identifier, issuing authority, publication or event date, repository URL, access date, locator (page/section/timecode), verbatim excerpt, and hash if a file. Anything less is a lead, not evidence.

## 12. Confidence Assessment

| Level | Criteria |
|---|---|
| HIGH | Official repository record, authenticated, directly on point |
| MODERATE | Primary record via reputable archive/mirror, minor custody gaps |
| LOW | Contemporaneous participant account, unverified document, or partial record |
| INSUFFICIENT | Lead only — no primary record located; claim remains unanchored |

## 13. Common Analytical Mistakes

- Treating an official *statement about* a record as the record itself.
- Citing a PDF from an unofficial mirror without checking it against the canonical version.
- Assuming an official document is true — primary authenticates origin, not content (see `propaganda_analysis.md`).
- Ignroring negative primary evidence because it contradicts the working hypothesis.

## 14. Ethical Considerations

Some primary records contain personal data, sealed-case references, or doxxing material. Cite the minimum excerpt needed. Do not republish full documents containing third-party personal data; reference locators instead. Leaked materials are handled per `legal/` rules — possession and citation are not endorsement.

## 15. Security Boundaries

Retrieval is passive HTTP access to public repositories. No credential use against non-public systems, no exploitation of repository vulnerabilities, no scraping that violates terms where a lawful alternative exists. Document any access that required bypassing paywalls or bot controls.

## 16. Expected Output

For each material claim: a primary-source citation block (per `source_citation_standards.md`), an authenticity note, a provenance record in `source_provenance_tracking.md`, and a confidence band. Contradictions between primary records are escalated as analytical findings, not silently resolved.

## 17. Quality Checklist

- [ ] Primary record located or documented absence recorded
- [ ] Repository is authoritative or provenance documented
- [ ] Excerpt verbatim with locator
- [ ] Authentication checks performed
- [ ] Hash/access date captured
- [ ] Contradictions logged, not smoothed over

## 18. Cross-Reference Links

- Complements: `secondary_source_verification.md`, `tertiary_source_handling.md`, `document_authenticity_assessment.md`, `publication_date_verification.md`
- Feeds: `claim_verification.md`, `cross_source_corroboration.md`, `evidence_chain_management.md`
- Divisions: `osint/` (collection), `legal/` (leaked-doc rules), `reporting/` (citation format), `analytics/` (confidence)
