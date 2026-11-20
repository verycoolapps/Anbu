# Translation Verification

**Division 007 · Verification · ANBU OSINT**

## 1. Purpose

Translation is interpretation: every translated claim is twice removed from the source language, and every hop introduces error, bias, or deliberate distortion. This file defines how ANBU verifies translated material — whether ANBU's own translations or third-party translations encountered in sources.

## 2. Scope

Covers translated articles, subtitles, official document translations, social-media translations, machine-translated content, and quotes in translation. Covers both directions: verifying others' translations and certifying ANBU's own.

## 3. Intelligence Objectives

- Detect translation distortion: meaning shifts, tone changes, omitted qualifiers, politically loaded terminology.
- Verify ANBU's own translations meet a defensible standard before publication.
- Recognize when a claim's truth depends on translation choices (e.g., ambiguous source terms).
- Route high-stakes translations to qualified human review.

## 4. Core Concepts

- **Untranslatable residue:** some meaning (register, idiom, political connotation) does not survive translation; flag claims that depend on it.
- **Terminology is politics:** choices like "freedom fighter" vs. "terrorist," "regime" vs. "government" encode interpretation; record contested terms explicitly.
- **Machine translation is a lead, not a verdict:** MT output requires human or expert verification for any material claim.
- **Subtitle/caption translation** is frequently unofficial and error-prone; official subtitles are not guaranteed accurate either.

## 5. Analytical Methodology

1. **Obtain the original-language text:** always verify against the source language, never against another translation.
2. **Produce a careful translation:** for ANBU products, use qualified translation; record translator and method.
3. **Back-translation check:** for high-stakes items, translate back to source and compare meaning (flag divergences).
4. **Terminology audit:** list contested or ambiguous terms; document chosen renderings and alternatives.
5. **Context check:** verify the translation preserves qualifiers, negations, hedges, and attribution ("reportedly," "allegedly").
6. **Verdict:** for third-party translations — ACCURATE / MINOR-DEVIATION / MATERIAL-DISTORTION / UNVERIFIABLE. For ANBU translations — certified with reviewer sign-off.

## 6. Step-by-Step Workflow

1. Capture the original-language source with provenance.
2. If verifying a third-party translation: obtain it, align with original, compare segment by segment.
3. Flag: omissions, additions, negation flips, qualifier loss, terminology shifts, tone changes.
4. Assess materiality: does any deviation change the claim's truth value or implication?
5. For ANBU translations: draft, review by second linguist for high-stakes items, record both.
6. Issue verdict/certification with named checks and confidence.

## 7. Data Requirements

- Original-language source text with provenance record.
- The translation under review (for third-party) or draft + reviewer record (for ANBU).
- Segment-aligned comparison output.
- Terminology decision log.

## 8. Approved Public Sources

Original-language publications (the authoritative text), official translations published by governments/institutions, academic translation studies, professional translator associations for review standards, and language-specific fact-checking organizations.

## 9. Source Verification Standards

Material claims in translation require verification against the original language by a competent reader. ANBU's own published translations of material claims carry translator attribution and, for high-stakes items, second-reviewer sign-off. Machine translation alone never supports a published claim verdict.

## 10. Analytical Framework

Use the **Translation Fidelity Checklist**: fidelity (meaning preserved), completeness (nothing dropped), register (tone/formality), terminology (contested terms documented), pragmatics (speech-act force preserved — a question isn't a statement, a threat isn't a warning). Score each; material failures cap the verdict.

## 11. Evidence Requirements

Translation records include: source text + provenance, translation under review, aligned comparison, deviation log with materiality assessment, terminology decisions, verdict/certification, confidence. ANBU translations additionally record translator identity/qualification and reviewer.

## 12. Confidence Assessment

| Level | Criteria |
|---|---|
| HIGH | Verified against original by competent bilingual reviewer; deviations logged |
| MODERATE | Careful translation with minor unreviewed nuances |
| LOW | Machine translation or single-pass human translation of material claim |
| INSUFFICIENT | No original-language access — claim stays UNVERIFIABLE in translation |

## 13. Common Analytical Mistakes

- Verifying a translation against another translation (error compounding).
- Missing negation flips and qualifier loss — the highest-risk deviations.
- Treating official translations as automatically accurate.
- Ignoring that terminology choices can reverse attribution (who did what to whom).
- Publishing ANBU translations without recording that translation occurred.

## 14. Ethical Considerations

Translations of threatened or dissident speakers carry risk; handle per `legal/` and `security/`. Do not "improve" translations to fit a preferred narrative — fidelity to source is the standard. Credit translators appropriately in products.

## 15. Security Boundaries

Use of translation services on sensitive texts requires `legal/` review (data exposure). Prefer local or vetted tools for sensitive material; document what was sent where.

## 16. Expected Output

Verified-translation records, ANBU translation certifications, terminology glossaries for recurring contested terms, and flags on claims whose truth hinges on translation choices.

## 17. Quality Checklist

- [ ] Original-language source secured
- [ ] Segment-aligned comparison performed
- [ ] Deviations logged with materiality assessment
- [ ] Contested terminology documented
- [ ] Negations/qualifiers/attribution verified
- [ ] Verdict or certification issued with confidence

## 18. Cross-Reference Links

- Claims/media: `claim_verification.md`, `quotation_verification.md`, `manipulated_media_assessment.md`, `document_authenticity_assessment.md`
- Deception: `disinformation_detection.md` (deliberate distortion), `propaganda_analysis.md` (terminology as technique)
- Records: `source_provenance_tracking.md`, `evidence_chain_management.md`, `verification_audit_trail.md`, `source_citation_standards.md`
- Divisions: `osint/` (multilingual collection), `reporting/` (translation standards), `legal/`
