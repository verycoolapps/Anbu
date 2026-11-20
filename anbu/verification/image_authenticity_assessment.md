# Image Authenticity Assessment

**Division 007 · Verification · ANBU OSINT**

## 1. Purpose

This file defines the technical and contextual workflow for assessing whether a still image is authentic, manipulated, synthetic, or miscontextualized. It is the specialist procedure invoked by `manipulated_media_assessment.md` for all still-image exhibits.

## 2. Scope

Covers photographs, screenshots, scans, memes with photographic content, satellite/aerial imagery stills, and document images. Video frames are handled under `video_authenticity_assessment.md`; this file covers the still-image pipeline including frame captures used as exhibits.

## 3. Intelligence Objectives

- Determine image authenticity status: AUTHENTIC / EDITED / SYNTHETIC / RECONTEXTUALIZED / UNVERIFIABLE.
- Detect common manipulation types: splicing, clone-stamp, inpainting, generative fill, metadata stripping, AI generation.
- Verify contextual claims (location, date, event) independently of pixel content.
- Preserve exhibits with forensic integrity.

## 4. Core Concepts

- **Metadata first:** EXIF/XMP data, encoder signatures, and thumbnail consistency are quick wins — but metadata absence is normal for social-media images and proves nothing by itself.
- **Error-level analysis (ELA):** compression-error patterns reveal spliced or recompressed regions; requires care — ELA is suggestive, not conclusive.
- **Clone detection:** duplicated regions indicate copy-move manipulation.
- **Lighting/shadow geometry:** inconsistent shadow direction, impossible reflections, and mismatched lighting indicate compositing.
- **Recontextualization:** the dominant real-world manipulation — genuine photo, false caption, wrong date/place. Pixel analysis will not catch it; provenance and geolocation will.

## 5. Analytical Methodology

1. **Preserve:** hash the file; record acquisition path; retain original untouched copy.
2. **Metadata extraction:** EXIF, XMP, IPTC, PNG text chunks, C2PA/Content Credentials; record presence, absence, and anomalies.
3. **Provenance check:** earliest known instance via reverse search; compare metadata across instances.
4. **Technical inspection:** resolution consistency, compression artifacts, edge halos, noise-pattern discontinuities, clone regions, lighting/shadow consistency.
5. **AI-generation indicators:** check for known synthetic signatures (unrealistic text, hand/finger anomalies, texture uniformity) — treat as weak indicators only.
6. **Context verification:** match claimed location/date/event against `geoint/` records and `publication_date_verification.md`.
7. **Verdict:** issue per `manipulated_media_assessment.md` matrix with named checks.

## 6. Step-by-Step Workflow

1. Receive image; verify file integrity and hash.
2. Extract all metadata; log fields and anomalies.
3. Reverse-search: Google Lens, TinEye, Yandex, platform-native search; record earliest results.
4. Visual inspection at full resolution: edges, text, hands, reflections, shadows, background consistency.
5. Apply ELA and clone-stamp checks where tooling permits; document method and result.
6. Geolocation: match claimed location to visual evidence per `geoint/`; verify date consistency.
7. Issue verdict card: status, checks performed, indicators, confidence, manifest.

## 7. Data Requirements

- Original image file (not screenshot of image) with hash.
- Metadata extraction report.
- Reverse-search result set with dates.
- Claimed context (caption, location, date, event) being tested.
- Tool/method log for reproducibility.

## 8. Approved Public Sources

Reverse-image search engines, EXIF viewers, C2PA/content-credential readers, open-source forensic tools (documented versions), satellite imagery archives for geolocation cross-check (`geoint/`), fact-checker image investigations, and academic image-forensics literature.

## 9. Source Verification Standards

Verdicts name every check performed. A verdict of EDITED requires affirmative manipulation evidence (splicing boundary, clone region, metadata contradiction). A verdict of AUTHENTIC requires no indicators found across all applicable checks AND consistent provenance — "looks normal" is not a verdict.

## 10. Analytical Framework

Use the **Image Assessment Record**: file hash → metadata findings → provenance results → technical findings (each named) → context match → verdict. Scores feed `evidence_confidence_scoring.md`; verdicts feed `claim_verification.md` when the image supports a claim.

## 11. Evidence Requirements

Every image assessment retains: original file + hash, metadata report, reverse-search log, forensic check outputs, context verification results, verdict, and confidence. Excerpts or crops used in products link back to the exhibit record.

## 12. Confidence Assessment

| Level | Criteria |
|---|---|
| HIGH | Multiple independent manipulation indicators or provenance contradiction |
| MODERATE | Strong single indicator or consistent anomaly set |
| LOW | Ambiguous findings with benign explanations |
| INSUFFICIENT | File too degraded or checks inapplicable — UNVERIFIABLE |

## 13. Common Analytical Mistakes

- Treating metadata absence as proof of manipulation (social platforms strip it routinely).
- Declaring AI generation from visual style alone.
- Ignoring recontextualization because pixels are clean.
- Using ELA on already-compressed social-media images and over-reading noise.
- Publishing verdicts without preserving the original file.

## 14. Ethical Considerations

Image verdicts affect real people. Publish only documented verdicts; label uncertainty honestly. Do not enhance or distribute manipulated images; analytical exhibits are watermarked and context-labeled.

## 15. Security Boundaries

Assessment is on provided files. No active scraping of image sources beyond public reverse-search; no uploading sensitive exhibits to third-party services without `legal/` review.

## 16. Expected Output

Image verdict cards, exhibit archive entries, and — for public-facing work — debunk packages per `fact_checking_methodology.md`.

## 17. Quality Checklist

- [ ] Original preserved + hashed
- [ ] Metadata extracted, anomalies logged
- [ ] Reverse-search earliest instance found
- [ ] Technical checks named and performed
- [ ] Context (geo/date/event) verified
- [ ] Verdict + confidence with manifest

## 18. Cross-Reference Links

- Parent: `manipulated_media_assessment.md`, `disinformation_detection.md`
- Context: `publication_date_verification.md`, `translation_verification.md`, `geoint/` (directory)
- Records: `source_provenance_tracking.md`, `evidence_chain_management.md`, `verification_audit_trail.md`
- Divisions: `geoint/`, `security/`, `reporting/`, `legal/`
