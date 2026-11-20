# Video Authenticity Assessment

**Division 007 · Verification · ANBU OSINT**

## 1. Purpose

Video is the highest-stakes and hardest-to-verify media type: it carries apparent eyewitness authority while being trivially recontextualized and increasingly synthetic. This file defines the video authenticity workflow — technical integrity, content authenticity, and contextual truth are assessed as three separate questions.

## 2. Scope

Covers user-generated footage, news clips, surveillance/cctv stills and clips, livestreams, screen recordings, and AI-generated video. Audio authenticity and lip-sync are within scope where they affect the verdict.

## 3. Intelligence Objectives

- Determine whether video content is genuine footage, edited, synthetic, or miscontextualized.
- Detect splicing, deepfakes, face-swap, lip-sync manipulation, and metadata anomalies.
- Verify claimed time/place/event independently — the dominant real-world failure is real footage in false context.
- Preserve exhibits forensically.

## 4. Core Concepts

- **Three separate questions:** (1) Is the footage technically manipulated? (2) Is it synthetically generated? (3) Does the claimed context match? A video can pass (1) and (2) yet be deceptive via (3).
- **Frame-level forensics:** manipulation often hides between frames or in short segments; full-resolution frame inspection is mandatory for contested clips.
- **Audio-visual consistency:** lip-sync errors, audio room-tone mismatches, and codec inconsistencies are manipulation indicators.
- **Deepfake indicators (2026 state):** temporal flicker, facial boundary artifacts, eye/blink anomalies, teeth/skin texture uniformity — indicators, never proof.

## 5. Analytical Methodology

1. **Preserve:** hash original file; record acquisition (platform, URL, timestamp, uploader).
2. **Metadata:** container metadata, encoder signatures, creation timestamps vs. claimed date; platform re-encode signatures.
3. **Provenance:** earliest known instance via reverse video search (InVID, platform tools); upload-chain history.
4. **Technical inspection:** frame-by-frame review of contested segments; splice detection (frame discontinuities); clone detection; lighting consistency.
5. **Deepfake screening:** facial-region analysis for synthetic indicators; audio analysis for voice synthesis/cloning artifacts.
6. **Context verification:** geolocation, timestamp cross-checks (sun position, shadows, weather records), event matching per `geoint/` and `publication_date_verification.md`.
7. **Verdict:** per `manipulated_media_assessment.md` matrix; document every check.

## 6. Step-by-Step Workflow

1. Acquire best-quality original; note whether platform compression is the only available version.
2. Extract metadata and keyframes; log anomalies.
3. Reverse-search video and distinctive frames; record earliest instances.
4. Review full clip; extract and inspect frames at 1 fps minimum plus targeted high-rate sampling at cuts/suspect segments.
5. Run splice/deepfake/audio-consistency checks; document methods and results.
6. Geolocate and date-verify the scene independently.
7. Issue verdict card with confidence and evidence manifest.

## 7. Data Requirements

- Original or highest-quality available video file with hash.
- Frame extraction set (documented sampling method).
- Metadata report and platform re-encode notes.
- Reverse-search results.
- Claimed context details for independent verification.

## 8. Approved Public Sources

Reverse video search tools (InVID & WeVerify plugin, platform-native), video forensic tools (documented open-source options), satellite/weather archives for context checks, fact-checker video investigations, deepfake-detection research literature, and platform transparency data on manipulated-media removals.

## 9. Source Verification Standards

No verdict rests on a single automated detector. Every verdict names the checks performed, the indicators observed or absent, and the confidence. UNVERIFIABLE is the honest default for heavily compressed or short clips where checks are inconclusive.

## 10. Analytical Framework

Use the **Video Verdict Matrix**: technical integrity × synthetic-content indicators × provenance consistency × context match → verdict. Manipulation in any layer yields MANIPULATED or RECONTEXTUALIZED as applicable; clean pixels with false context yield RECONTEXTUALIZED, not AUTHENTIC.

## 11. Evidence Requirements

Verdict cards include: file hash, acquisition record, metadata findings, frame-sample documentation, forensic checks named, reverse-search log, context verification results, verdict, confidence. Video exhibits link to `evidence_chain_management.md` with timecode references.

## 12. Confidence Assessment

| Level | Criteria |
|---|---|
| HIGH | Multiple independent manipulation indicators, or provenance/context contradiction documented |
| MODERATE | Strong single-layer evidence (e.g., clear splice boundary + inconsistent audio) |
| LOW | Ambiguous indicators with benign explanations |
| INSUFFICIENT | Compression/length prevents meaningful checks — UNVERIFIABLE |

## 13. Common Analytical Mistakes

- Verifying pixels while ignoring false context (the most common miss).
- Treating "no deepfake detected" as proof of authenticity.
- Relying on a single detector score without manual frame review.
- Ignoring audio — manipulated video often has cloned or mismatched audio.
- Assuming platform labels ("false information") substitute for independent verification.

## 14. Ethical Considerations

Video verdicts can inflame conflicts. Publish only HIGH-confidence verdicts publicly; label others appropriately. Do not redistribute graphic manipulated content; analytical stills are contextualized and minimized.

## 15. Security Boundaries

Passive analysis of provided files and public uploads. No uploading sensitive exhibits to external detection services without `legal/` review. Do not create synthetic media for any purpose.

## 16. Expected Output

Video verdict cards with frame-level evidence, exhibit archive entries, operation profiles when video is part of a deception campaign (`disinformation_detection.md`), and public debunks via `fact_checking_methodology.md`.

## 17. Quality Checklist

- [ ] Best-quality original preserved + hashed
- [ ] Metadata + platform signatures analyzed
- [ ] Reverse-search earliest instance found
- [ ] Frame-level review documented
- [ ] Splice/deepfake/audio checks named and performed
- [ ] Context (geo/date/event) independently verified
- [ ] Verdict + confidence with manifest

## 18. Cross-Reference Links

- Parent: `manipulated_media_assessment.md`, `image_authenticity_assessment.md`
- Context/intent: `disinformation_detection.md`, `misinformation_detection.md`, `propaganda_analysis.md`, `publication_date_verification.md`
- Geolocation: `geoint/` division
- Records: `source_provenance_tracking.md`, `evidence_chain_management.md`, `verification_audit_trail.md`
- Divisions: `security/`, `reporting/`, `legal/`
