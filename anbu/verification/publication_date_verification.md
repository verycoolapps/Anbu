# Publication Date Verification

**Division 007 · Verification · ANBU OSINT**

## 1. Purpose

The claimed publication date of content is a load-bearing fact: it determines whether information was available when decisions were made, whether images predate events they are said to depict, and whether "news" is recycled material. This file defines how ANBU establishes when content was actually published, created, or first appeared.

## 2. Scope

Covers articles, posts, images, videos, documents, dataset releases, and archived pages. Distinguishes three different dates that are routinely conflated: content creation date, first-publication date, and the date a copy was accessed or re-shared.

## 3. Intelligence Objectives

- Establish first-publication dates for viral and evidentiary content.
- Detect recycled content presented as new — a primary disinformation and engagement-farming technique.
- Verify that content existed (or did not) at decision-relevant times.
- Detect backdated or forward-dated material, including manipulated timestamps.

## 4. Core Concepts

- **Three dates:** creation (EXIF/metadata), first-publication (earliest discoverable posting), and access/copy date. Only the first two bear on authenticity claims; the third is custody.
- **Timestamp laundering:** platforms allow edits and reposts that obscure original dates; earliest-instance search is the corrective.
- **Metadata dates lie:** EXIF dates are trivially edited; treat as claims, corroborate with archive captures.
- **The Wayback problem:** archive captures prove existence *by* a date, not *since* a date; absence of early captures is weak negative evidence.

## 5. Analytical Methodology

1. **Capture now:** record current timestamp and content hash immediately.
2. **Extract claimed dates:** metadata, on-page dates, URL patterns, platform timestamps.
3. **Earliest-instance search:** reverse-search content, search distinctive phrases with date filters, check platform post IDs/timestamps, query archives (Wayback, archive.today).
4. **Corroborate:** multiple independent date signals (archive capture + platform timestamp + metadata) establish a date range.
5. **Flag anomalies:** dates that postdate events the content depicts, future dates, inconsistent internal timestamps.
6. **Verdict:** ESTABLISHED (narrow range) / RANGE (bounded) / UNRESOLVED / ANOMALOUS.

## 6. Step-by-Step Workflow

1. Record item with hash and current UTC time.
2. Collect all claimed dates from metadata and page content.
3. Run earliest-instance searches across web archives, search engines with `before:` filters, platform-native history.
4. Check for edit history where platforms expose it.
5. Cross-check internal consistency: does the content reference events that fix a latest-possible date? Does metadata predate claimed publication implausibly?
6. Record date verdict with evidence; feed into `claim_verification.md` and media assessments.

## 7. Data Requirements

- Content hash and capture timestamp.
- All claimed date fields extracted.
- Archive query results (Wayback CDX, archive.today).
- Platform timestamp evidence.
- Content-internal date constraints (referenced events).

## 8. Approved Public Sources

Internet Archive/Wayback Machine and CDX API, archive.today, search engines with date operators, platform public timestamps and edit histories, news-archive services, DNS/whois historical records for domains, certificate transparency logs (for site existence dating), and EXIF/metadata fields (as claims requiring corroboration).

## 9. Source Verification Standards

A publication date is ESTABLISHED only with ≥2 independent date signals converging, or one authoritative signal (e.g., platform timestamp from the original poster) plus absence of earlier instances in thorough search. Single metadata dates are never sufficient.

## 10. Analytical Framework

Use the **Date Confidence Bands**: same-day certainty (multiple signals), narrow range (days), bounded range (weeks/months), unresolved. Record which signals support the band. Date verdicts attach to claim cards as an evidentiary input.

## 11. Evidence Requirements

Date verification records include: item hash, all claimed dates, search methodology and queries, archive capture URLs with timestamps, platform evidence, internal-consistency analysis, verdict, and confidence.

## 12. Confidence Assessment

| Level | Criteria |
|---|---|
| HIGH | Multiple convergent independent signals; earliest instance identified |
| MODERATE | One authoritative signal plus supporting evidence |
| LOW | Single weak signal or conflicting signals unresolved |
| INSUFFICIENT | No reliable date evidence — treat as undated |

## 13. Common Analytical Mistakes

- Treating "date on the page" as publication date — CMS dates are often modified dates.
- Assuming no archive capture means recent publication.
- Ignoring timezone differences in timestamp comparison.
- Letting a recycled image's original EXIF date be cited as the repost date.
- Using date uncertainty to avoid a verdict — report the range honestly.

## 14. Ethical Considerations

Date verification can be used to "debunk" by claiming content is older than claimed when the truth is merely uncertain. Publish date verdicts with the same evidentiary rigor as content verdicts; UNRESOLVED is a legitimate finding.

## 15. Security Boundaries

Passive archive and search queries only. Respect archive rate limits; document bulk access. No attempts to access non-public platform data for timestamps.

## 16. Expected Output

Date-verification records attached to items in provenance; date verdicts as inputs to claim cards, media assessments, and timeline construction in `analytics/`.

## 17. Quality Checklist

- [ ] Item hashed and captured immediately
- [ ] All claimed dates extracted
- [ ] Earliest-instance search executed and logged
- [ ] Independent signals converged or divergence documented
- [ ] Internal-consistency check performed
- [ ] Date verdict + confidence recorded

## 18. Cross-Reference Links

- Content integrity: `manipulated_media_assessment.md`, `image_authenticity_assessment.md`, `video_authenticity_assessment.md`, `document_authenticity_assessment.md`
- Claims: `claim_verification.md`, `quotation_verification.md`, `translation_verification.md`
- Records: `source_provenance_tracking.md`, `evidence_chain_management.md`, `verification_audit_trail.md`
- Divisions: `osint/` (archival collection), `analytics/` (timelines), `reporting/`
