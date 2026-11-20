# Manipulated Media Assessment

**Division 007 · Verification · ANBU OSINT**

## 1. Purpose

Manipulated media — doctored images, recontextualized video, synthetic audio, spliced documents — is the most virulent vector for modern deception. This file is the umbrella procedure for detecting media manipulation of any kind, routing specific media types to their dedicated assessments (`image_authenticity_assessment.md`, `video_authenticity_assessment.md`, `document_authenticity_assessment.md`) and synthetic content to `disinformation_detection.md` where intent is at issue.

## 2. Scope

Covers all media types: still images, video, audio, documents, screenshots, maps, and composite content. This file defines the general triage framework; type-specific technical checks live in the dedicated files.

## 3. Intelligence Objectives

- Triage media items quickly: authentic / manipulated / unverifiable.
- Route items to the correct specialist assessment without duplication.
- Detect manipulation even when the media is real but the context is fabricated (the most common and hardest case).
- Preserve media evidence with forensic integrity for potential `legal/` proceedings.

## 4. Core Concepts

- **Content authenticity vs. context authenticity:** a real photo with a false caption is manipulation of meaning, not pixels. Both must be checked.
- **The manipulation ladder:** recontextualization (easiest, most common) → editing/splicing → deep synthesis. Difficulty of detection decreases down the ladder; real-world frequency increases up it.
- **Provenance-first:** before pixel analysis, check whether the media's documented origin supports the claimed context. Provenance failures often resolve the question faster than forensics.
- **The liar's dividend caveat:** demonstrating that *some* media is fake does not prove *this* media is fake; verdicts are per-item.

## 5. Analytical Methodology

1. **Snapshot and hash** the media immediately; preserve original file and metadata.
2. **Context check:** does the claimed time/place/event match the media's provenance? Apply `publication_date_verification.md` and geolocation per `geoint/`.
3. **Type routing:** image → `image_authenticity_assessment.md`; video → `video_authenticity_assessment.md`; document → `document_authenticity_assessment.md`; audio → transcription/provenance checks.
4. **Manipulation forensics:** apply the type-specific technical checks; record indicators found or absent.
5. **Synthesis check:** for suspected synthetic content, apply deepfake indicators and AI-generation signals.
6. **Verdict:** AUTHENTIC / MANIPULATED / UNVERIFIABLE with evidence manifest; file in audit trail.

## 6. Step-by-Step Workflow

1. Acquire media: original file preferred; if only screenshot/screen-recording exists, record that limitation.
2. Extract metadata (EXIF, container metadata, encoder signatures); flag stripping anomalies.
3. Reverse-search the image/video (per image assessment file) for earlier instances.
4. Frame-by-frame or detail inspection for video; error-level analysis for images where tools permit.
5. Check compression artifacts, lighting consistency, shadow geometry, edge anomalies, audio-visual sync.
6. Assess context claims independently of pixels: caption, location, date, event.
7. Issue verdict card with confidence and full evidence manifest.

## 7. Data Requirements

- Original media file with SHA-256 hash; acquisition provenance.
- Metadata extraction output.
- Reverse-search results with timestamps.
- Frame captures for video analysis.
- Context claims being tested (caption, location, date, event).

## 8. Approved Public Sources

The media itself, reverse-image search engines, platform content-credentials/C2PA data where present, fact-checker media investigations, academic media-forensics literature, and open-source detection tooling documentation. No paid "deepfake detection" services are assumed; methodology must be documented regardless of tools used.

## 9. Source Verification Standards

A media verdict requires documented checks, not tool output alone: name the methods applied, the indicators observed, and the confidence. "A detector said fake" is not evidence — detectors have false-positive rates and are easily evaded. Verdicts state which checks were performed.

## 10. Analytical Framework

Use the **Media Verdict Matrix**: provenance status × technical findings × context match → verdict. AUTHENTIC requires no manipulation indicators AND consistent provenance/context. MANIPULATED requires affirmative manipulation evidence. UNVERIFIABLE covers everything else — including real media in false context pending geolocation/verification.

## 11. Evidence Requirements

Verdict cards for media include: file hash, acquisition record, metadata findings, reverse-search results, forensic checks performed (named), indicators observed, context verification status, verdict, and confidence. All media exhibits link to `evidence_chain_management.md`.

## 12. Confidence Assessment

| Level | Criteria |
|---|---|
| HIGH | Multiple independent manipulation indicators OR authenticated provenance contradicting claim |
| MODERATE | Strong single-indicator evidence or consistent anomaly pattern |
| LOW | Ambiguous indicators; plausible benign explanations exist |
| INSUFFICIENT | Cannot perform meaningful checks; verdict UNVERIFIABLE |

## 13. Common Analytical Mistakes

- Declaring media fake because it "looks AI-generated" — visual style is not evidence.
- Declaring media real because no manipulation was found — absence of evidence is not evidence of authenticity.
- Confusing recontextualization with pixel manipulation and missing the actual deception.
- Trusting a single automated detector without corroborating indicators.
- Publishing media verdicts without preserving the original file and hash.

## 14. Ethical Considerations

Media verdicts affect reputations and public discourse. Publish only verdicts meeting the HIGH bar of documented checks; label UNVERIFIABLE honestly rather than implying innocence or guilt. Never use manipulated media in ANBU products outside clearly-labeled analytical context.

## 15. Security Boundaries

Forensic work on provided files is in-scope; active collection of media from targets is governed by `osint/` and `legal/`. Do not distribute manipulated media even for debunking without watermarking/context; do not create manipulated media under any circumstances.

## 16. Expected Output

Media verdict cards with evidence manifests; exhibit archives preserving originals with hashes; integration into `disinformation_detection.md` profiles when deception operations are involved; corrections via `fact_checking_methodology.md` when public verdicts are issued.

## 17. Quality Checklist

- [ ] Original file hashed and preserved
- [ ] Metadata extracted and anomalies noted
- [ ] Reverse-search performed
- [ ] Type-appropriate forensic checks named and performed
- [ ] Context claims verified independently
- [ ] Verdict + confidence issued with manifest
- [ ] Exhibit archived per chain management

## 18. Cross-Reference Links

- Type specialists: `image_authenticity_assessment.md`, `video_authenticity_assessment.md`, `document_authenticity_assessment.md`, `quotation_verification.md`
- Intent/context: `disinformation_detection.md`, `misinformation_detection.md`, `propaganda_analysis.md`, `publication_date_verification.md`, `translation_verification.md`
- Records: `source_provenance_tracking.md`, `evidence_chain_management.md`, `verification_audit_trail.md`
- Divisions: `geoint/` (geolocation), `security/` (threat media), `reporting/` (exhibit presentation), `legal/`
