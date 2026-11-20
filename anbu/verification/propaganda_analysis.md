# Propaganda Analysis

**Division 007 · Verification · ANBU OSINT**

## 1. Purpose

Propaganda is organized communication designed to shape perceptions, emotions, and behavior toward a political objective — typically *openly attributed* to its sponsor, unlike covert disinformation. Analyzing propaganda is analytical work: identifying the message, technique, audience, and intended effect. This file defines ANBU's framework for recognizing and analyzing propaganda without confusing it with ordinary persuasion, opinion, or journalism.

## 2. Scope

Covers state media output, government information campaigns, military information operations (MISO) that are declared or attributable, domestic messaging apparatuses, and influence content from identifiable sponsors. Covert operations belong to `disinformation_detection.md`; this file addresses attributed or attributable persuasion campaigns.

## 3. Intelligence Objectives

- Identify propaganda techniques and classify them consistently.
- Understand what a sponsor is trying to achieve: rally, deter, divide, recruit, demoralize, legitimize.
- Track narrative evolution and audience targeting over time.
- Avoid two failure modes: dismissing propaganda as "just lies" (missing its function) or treating it as truth (missing its purpose).

## 4. Core Concepts

- **Propaganda ≠ lie:** effective propaganda often wraps true facts in selective framing. Analysis targets technique and intent, not only falsity.
- **Technique taxonomy:** appeal to fear/authority/belonging, bandwagon, card-stacking (cherry-picking), glittering generalities, name-calling, transfer, plain-folks, testimonial, fear-then-solution structure.
- **Audience segmentation:** the same sponsor runs different messages to different audiences; analyze per-audience.
- **Counter-propaganda:** responses may themselves be propagandistic; apply the same framework symmetrically.

## 5. Analytical Methodology

1. **Identify sponsor and attribution:** who produces this, and is attribution open, inferred, or contested?
2. **Extract the core message:** the single proposition the content is built to implant.
3. **Inventory techniques:** map each element to the technique taxonomy; note emotional register.
4. **Identify audience and objective:** who is addressed, what behavior is sought.
5. **Assess factual substrate:** which claims are true-but-framed vs. fabricated (route fabrications to `claim_verification.md`).
6. **Track over time:** narrative shifts reveal strategic changes; archive per `source_provenance_tracking.md`.

## 6. Step-by-Step Workflow

1. Collect the propaganda artifact with full provenance.
2. Produce a content breakdown: text/image/audio elements, emotional appeals, CTA.
3. Technique-map the content; score density (techniques per unit).
4. Cross-reference factual claims against verification pipeline; mark TRUE-FRAMED / FALSE / UNVERIFIABLE per element.
5. Infer objective and audience; state inference confidence.
6. Write analysis product section: message, techniques, objective, effectiveness indicators, counterpoints.

## 7. Data Requirements

- Complete artifact captures (all formats, all language versions).
- Sponsor identification with evidence for attribution.
- Audience/distribution channel data where public.
- Claim-level verdicts for embedded factual assertions.
- Temporal series for narrative tracking.

## 8. Approved Public Sources

The propaganda artifacts themselves (state media, official channels, attributed campaigns), academic propaganda studies, platform transparency reports on state media, media-monitoring organization reports, and historical case literature. Analysis cites the artifact and its context — not the sponsor's self-description of its intent.

## 9. Source Verification Standards

Attribution of propaganda to a sponsor requires evidence: official channels, consistent branding, documented distribution, or credible investigative attribution. When attribution is contested, publish the analysis with attribution confidence stated. Never infer sponsorship from content tone alone.

## 10. Analytical Framework

Use the **Propaganda Profile**: sponsor (confidence) × core message × technique inventory × audience × objective × factual substrate verdict × reach. Profiles feed strategic analysis in `geopolitical/` and `political/`; they are descriptive-analytic, not polemical.

## 11. Evidence Requirements

Every propaganda analysis cites: the artifact (provenance record), attribution evidence, technique mapping with quoted examples, claim verdicts for factual elements, and audience/objective inference rationale. Quoted examples must satisfy `quotation_verification.md`.

## 12. Confidence Assessment

| Level | Criteria |
|---|---|
| HIGH | Attribution documented; techniques and objective supported by distribution data |
| MODERATE | Attribution probable; objective inference reasonable but not confirmed |
| LOW | Attribution uncertain or objective speculative — publish as hypothesis |
| INSUFFICIENT | Cannot distinguish propaganda from ordinary advocacy; do not label |

## 13. Common Analytical Mistakes

- Calling everything one disagrees with "propaganda" — the label requires technique + intent + attribution analysis.
- Analyzing only content falsity while ignoring the persuasive architecture.
- Assuming all state media is propaganda (some is dull record; assess actual technique density).
- Ignoring that open democratic governments also run persuasion campaigns; apply the framework symmetrically.
- Treating audience reception as uniform — propaganda often fails with its target.

## 14. Ethical Considerations

Propaganda analysis is dual-use: the same framework could craft propaganda. ANBU publishes technique descriptions at the analytical level, never operational playbooks. Do not assist in producing or amplifying propaganda; analysis is defensive and descriptive.

## 15. Security Boundaries

Passive analysis of public artifacts only. No engagement with propagandists, no amplification of the content under analysis, no collection against private individuals. Sensitive influence-operation findings route to `security/` with `legal/` review.

## 16. Expected Output

Propaganda profiles per artifact or campaign; technique-frequency datasets for `analytics/`; narrative-evolution timelines; integration into `political/` and `geopolitical/` assessments with confidence labels.

## 17. Quality Checklist

- [ ] Sponsor attribution evidenced or confidence stated
- [ ] Core message extracted precisely
- [ ] Techniques mapped with quoted examples
- [ ] Factual substrate claims verified
- [ ] Audience/objective inference documented
- [ ] Temporal tracking initiated for campaigns
- [ ] Symmetric standards applied to all sponsors

## 18. Cross-Reference Links

- Threat siblings: `disinformation_detection.md`, `misinformation_detection.md`, `manipulated_media_assessment.md`
- Claim testing: `claim_verification.md`, `fact_checking_methodology.md`, `cross_source_corroboration.md`
- Quote/media: `quotation_verification.md`, `image_authenticity_assessment.md`, `video_authenticity_assessment.md`
- Divisions: `political/` (domestic messaging), `geopolitical/` (state campaigns), `security/` (operations), `reporting/`
