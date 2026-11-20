# Misinformation Detection

**Division 007 · Verification · ANBU OSINT**

## 1. Purpose

Misinformation is false or misleading content spread without intent to deceive — typically through error, carelessness, or genuine belief. Distinguishing it from disinformation (deliberate deception, see `disinformation_detection.md`) matters analytically but the detection techniques overlap heavily. This file defines how ANBU detects, classifies, and handles misinformation in collected material.

## 2. Scope

Covers inadvertent falsehoods: honest mistakes, outdated information presented as current, misunderstood statistics, satire taken literally, and low-quality aggregation. Also covers "malinformation" — real information presented to mislead — where manipulation is present but intent is ambiguous.

## 3. Intelligence Objectives

- Identify false claims regardless of intent, and record intent assessment separately.
- Detect the structural patterns that produce misinformation (aggregation decay, context collapse).
- Prevent ANBU products from amplifying misinformation while preserving legitimate contested claims.
- Map misinformation ecosystems when they intersect security or political questions.

## 4. Core Concepts

- **Error taxonomy:** factual error, outdated truth, decontextualization, statistical misuse, satirical literalism, aggregation drift.
- **Intent is a separate axis:** detection finds falsity; intent assessment (`disinformation_detection.md`) finds deliberateness. A claim can be verified false while intent remains unclear.
- **Misinformation lifecycle:** creation → amplification → decay/correction. Early-stage detection enables correction before wide spread.
- **Sincere-but-wrong actors:** ordinary users, well-meaning aggregators, and even professionals spread most misinformation. Do not assume bad actors.

## 5. Analytical Methodology

1. **Claim extraction:** isolate the testable assertion from opinion and framing.
2. **Verification:** run `claim_verification.md` workflow; obtain verdict and confidence.
3. **Error classification:** assign the error type; this determines likely cause (honest mistake vs. manipulation pipeline).
4. **Intent assessment:** examine origin, incentives, amplification pattern; document in `disinformation_detection.md` format if deliberate signals exist.
5. **Impact assessment:** estimate reach and consequence for prioritization (`security/` handoff if threat-relevant).
6. **Handling:** flag in products; if publicly debunking, follow `fact_checking_methodology.md`.

## 6. Step-by-Step Workflow

1. Ingest candidate item; snapshot per `tertiary_source_handling.md`.
2. Extract and verify claims per `claim_verification.md`.
3. Classify error type; check for known misinformation patterns (recycled old images, miscaptioned video, manipulated statistics).
4. Assess origin: organic, aggregator, state-adjacent, or unknown; check amplification topology.
5. Record in misinformation register: claim, verdict, error type, intent assessment, spread metrics, handling decision.
6. Escalate to `disinformation_detection.md` if intent evidence emerges; to `security/` if threat-relevant.

## 7. Data Requirements

- Claim card with verdict and evidence manifest.
- Origin and amplification data: earliest instance, propagation path, engagement trajectory.
- Error classification with justification.
- Intent signals documented separately from falsity verdict.

## 8. Approved Public Sources

The open web, public social platforms, fact-checking organization archives (as leads and context), platform transparency reports, academic misinformation research, and media-literacy resources. Debunking decisions use the standard evidence hierarchy.

## 9. Source Verification Standards

Misinformation labels must meet the same evidentiary bar as any verdict: FALSE ratings require affirmative contradictory evidence per `claim_verification.md`; UNVERIFIABLE stays unlabeled rather than falsely flagged. Document the verification trail so labels can be audited.

## 10. Analytical Framework

Use the **Misinformation Profile**: falsity verdict × error type × intent assessment × reach × vulnerability-of-audience. The profile drives handling: correct quietly (low reach), issue public clarification (high reach), or escalate (coordinated/threat-relevant). Distinguish content-level falsehood from source-level unreliability (`source_reliability_assessment.md`).

## 11. Evidence Requirements

Each flagged item requires: the claim, verdict card, error classification rationale, intent signals (or documented absence), earliest-instance record, and reach metrics at flagging time. Claims flagged FALSE without evidence manifests violate doctrine.

## 12. Confidence Assessment

| Level | Criteria |
|---|---|
| HIGH | Claim verified FALSE with primary-anchored contradiction; error type clear |
| MODERATE | FALSE verdict with strong corroboration but ambiguous error mechanism |
| LOW | Suspected misinformation, verification incomplete — flag as candidate only |
| INSUFFICIENT | Cannot determine falsity; item remains unverified, not flagged |

## 13. Common Analytical Mistakes

- Labeling something misinformation because it is false *and* disliked — falsity and offensiveness are independent.
- Assuming intent where only error is proven; keep the axes separate.
- Flagging satire without establishing it is being circulated as literal fact.
- Treating contested scientific or political claims as misinformation when they are merely disputed.
- Ignoring that corrections themselves can be weaponized; verify debunks too.

## 14. Ethical Considerations

False-positive misinformation labels cause real harm (chilling legitimate speech, discrediting honest error). Conservative flagging, published criteria, and correction mechanisms are mandatory. Do not build blacklists of individuals for sharing misinformation — track claims and patterns, not persons, unless threat analysis under `security/` applies.

## 15. Security Boundaries

Misinformation analysis is passive. Do not engage with spreaders, do not create counter-narrative sock-puppets, do not attempt platform manipulation. Threat-relevant cases (election interference, public-safety rumors) hand off to `security/` with evidence packages.

## 16. Expected Output

Misinformation register entries with full profiles; correction recommendations for `reporting/`; escalation packages for `security/`; periodic ecosystem summaries for `analytics/`.

## 17. Quality Checklist

- [ ] Claim verified; verdict and confidence recorded
- [ ] Error type classified with rationale
- [ ] Intent assessed separately from falsity
- [ ] Earliest instance and spread documented
- [ ] Handling decision recorded (correct/de-escalate/escalate)
- [ ] No person-level blacklists created

## 18. Cross-Reference Links

- Verification core: `claim_verification.md`, `fact_checking_methodology.md`, `cross_source_corroboration.md`
- Sibling threat: `disinformation_detection.md`, `propaganda_analysis.md`, `manipulated_media_assessment.md`
- Records: `source_provenance_tracking.md`, `evidence_chain_management.md`, `verification_audit_trail.md`
- Divisions: `security/` (threat cases), `reporting/` (public corrections), `osint/` (collection)
