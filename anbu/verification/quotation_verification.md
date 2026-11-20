# Quotation Verification

**Division 007 · Verification · ANBU OSINT**

## 1. Purpose

Quotations carry outsized rhetorical weight and are among the most frequently manipulated elements in public discourse: clipped out of context, paraphrased into quotation marks, translated loosely, or fabricated entirely. This file defines how ANBU verifies that a quotation is accurate, complete-in-context, and correctly attributed.

## 2. Scope

Covers direct quotes, partial quotes, translated quotes, quotes from speeches/documents/testimony, and quotes circulating on social media. Distinguishes verbatim accuracy from contextual fairness — both must be checked.

## 3. Intelligence Objectives

- Verify verbatim accuracy: does the source text actually contain these words?
- Verify attribution: did this person say/write this, in this venue, at this time?
- Verify context integrity: does surrounding context change the meaning?
- Detect fabricated, stitched, or AI-generated quotations.

## 4. Core Concepts

- **Verbatim vs. gist:** quotation marks claim verbatim accuracy; [brackets] and ellipses signal editorial alteration — check whether alterations change meaning.
- **Context is part of the quote:** a verbatim sentence embedded in a false narrative is still a misquote in effect. Verify the surrounding paragraph/speech segment.
- **Translation is interpretation:** "translated quotes" are twice removed from source; verify against the original-language text, not another translation.
- **Audio/video quotes:** verify against the recording, including what was actually said vs. subtitles/captions (which are frequently wrong).

## 5. Analytical Methodology

1. **Capture the quote claim:** exact quoted text, attributed speaker, venue, date, outlet carrying the quote.
2. **Locate the original:** transcript, video, document, or audio recording of the original utterance.
3. **Verbatim comparison:** word-for-word check; note every deviation including punctuation and filler words.
4. **Context extraction:** pull the surrounding 2–3 paragraphs/minutes; assess whether context supports or reverses the quoted meaning.
5. **Attribution check:** confirm speaker identity, venue, and date via `publication_date_verification.md` and provenance.
6. **Translation check:** if translated, verify against original language per `translation_verification.md`.
7. **Verdict:** VERBATIM-ACCURATE / MINOR-DEVIATION / CONTEXT-MISLEADING / FABRICATED / UNVERIFIABLE.

## 6. Step-by-Step Workflow

1. Record the quote exactly as published, with the publishing outlet and timestamp.
2. Identify the claimed original source (speech, interview, document, post).
3. Retrieve the original: official transcript preferred; video/audio frame-and-audio verification; document page.
4. Compare verbatim; log every deviation with location.
5. Extract and review context; document whether context alters meaning.
6. Verify speaker/venue/date independently.
7. Issue verdict card with the original-source citation per `source_citation_standards.md`.

## 7. Data Requirements

- Published quote text + carrier citation.
- Original source location (URL, timestamp, page).
- Verbatim comparison output (diff).
- Context extract.
- Attribution/date verification results.

## 8. Approved Public Sources

Official transcripts (government, court, legislative), full video/audio recordings, reputable transcript services (as leads — verify against recording), document repositories, platform-native post archives, and archived page captures. Subtitles and captions are leads, never the final authority.

## 9. Source Verification Standards

VERBATIM-ACCURATE requires word-for-word match against the original recording or official transcript. Quotes from memory, notes, or secondary reports cannot receive this rating. CONTEXT-MISLEADING is assigned when verbatim text is accurate but surrounding context reverses or materially alters the meaning.

## 10. Analytical Framework

Use the **Quote Verdict Matrix**: verbatim accuracy × attribution validity × context fairness → verdict. The matrix prevents the common failure of rating a quote TRUE while ignoring that it was clipped from a meaning-reversing context.

## 11. Evidence Requirements

Quote verdict cards include: published quote, carrier citation, original-source citation with locator (timestamp/page), verbatim diff, context extract, attribution evidence, verdict, confidence. Original recordings/transcripts link to provenance records.

## 12. Confidence Assessment

| Level | Criteria |
|---|---|
| HIGH | Original recording/official transcript located; verbatim comparison complete |
| MODERATE | Reliable transcript located, no recording available |
| LOW | Only secondary reports of the quote; original unlocated |
| INSUFFICIENT | No original source found — UNVERIFIABLE |

## 13. Common Analytical Mistakes

- Checking the quote against another article quoting it (circular verification).
- Trusting subtitles/captions over the actual audio.
- Approving ellipsis edits without checking whether removed text changes meaning.
- Verifying words but ignoring context — the highest-frequency error.
- Treating translated quotes as verified against English intermediaries.

## 14. Ethical Considerations

Quote verdicts about public figures require the same symmetric rigor as any claim. Avoid publishing quotes out of context in ANBU's own products — model the standard. Respect `legal/` for quotes from sealed proceedings or private communications.

## 15. Security Boundaries

Retrieval of public recordings and transcripts only. No access to non-public recordings or leaked private communications without `legal/` authorization.

## 16. Expected Output

Quote verdict cards, corrected-quote citations for products, and integration with `fact_checking_methodology.md` for public-facing quote checks.

## 17. Quality Checklist

- [ ] Published quote captured exactly
- [ ] Original source located (recording/transcript/document)
- [ ] Verbatim comparison completed with deviations logged
- [ ] Context reviewed for meaning impact
- [ ] Attribution/date independently verified
- [ ] Translations checked against original language
- [ ] Verdict + confidence issued

## 18. Cross-Reference Links

- Parent: `claim_verification.md`, `manipulated_media_assessment.md`
- Related: `translation_verification.md`, `publication_date_verification.md`, `video_authenticity_assessment.md`
- Deception: `misinformation_detection.md`, `disinformation_detection.md`, `propaganda_analysis.md`
- Records: `source_provenance_tracking.md`, `evidence_chain_management.md`, `verification_audit_trail.md`, `source_citation_standards.md`
- Divisions: `reporting/`, `legal/`
