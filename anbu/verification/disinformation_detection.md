# Disinformation Detection

**Division 007 · Verification · ANBU OSINT**

## 1. Purpose

Disinformation is false or misleading content created and spread *with intent to deceive*. This file defines how ANBU detects deliberate deception operations — distinguishing them from honest error (`misinformation_detection.md`) and from propaganda that is open about its source (`propaganda_analysis.md`). Intent evidence is the defining requirement; this file specifies what that evidence looks like.

## 2. Scope

Covers coordinated inauthentic behavior, fabricated evidence, forged documents, synthetic media deployed deceptively, front-group campaigns, state and non-state influence operations, and engineered narrative laundering. Applies to content, networks, and operations — not merely individual false posts.

## 3. Intelligence Objectives

- Detect deception operations early enough to inform warnings and analysis.
- Identify the operation's structure: creators, amplifiers, narrative, target audience, objective.
- Distinguish disinformation from journalism errors, satire, and opinion.
- Provide `security/` with actionable, evidence-bound packages on influence operations.

## 4. Core Concepts

- **Intent evidence:** fabrication (content that could not exist organically), coordination signatures (synchronized timing, identical phrasing, shared infrastructure), deceptive attribution (false personas, fake think tanks), and strategic consistency (narrative serves a discernible objective).
- **The liar's dividend:** actors may deny authentic content by pointing to demonstrated fakes — detection of fakes enables denial of reals. Record both.
- **Operation vs. content:** a single fake image is content; a fake image seeded through a persona network with a narrative arc is an operation.
- **Attribution humility:** ANBU can identify deception and likely sponsorship without proving state direction; label attribution confidence explicitly.

## 5. Analytical Methodology

1. **Verify falsity** per `claim_verification.md` — disinformation requires falsehood plus intent.
2. **Origin forensics:** earliest instance, account creation patterns, technical fingerprints, reverse-image provenance (`source_provenance_tracking.md`).
3. **Coordination analysis:** temporal clustering, content similarity across accounts, amplification topology (who boosts whom, bot-likeness signals).
4. **Narrative mapping:** what story is being pushed, what counter-narrative is suppressed, who benefits.
5. **Intent synthesis:** weigh fabrication evidence, coordination signatures, and strategic consistency; assign intent confidence.
6. **Package:** produce operation profile for `security/` and/or correction for `fact_checking_methodology.md`.

## 6. Step-by-Step Workflow

1. Ingest candidate; snapshot all material immediately.
2. Verify the underlying claims; document verdicts.
3. Build origin map: earliest instances, first amplifiers, suspected seed accounts.
4. Run coordination checks: posting-time histograms, phrase overlap, network graph of reshares/replies.
5. Check infrastructure: domain registration, hosting, account age distribution, profile reuse.
6. Assess narrative objective and beneficiary; check against known operation patterns (do not over-fit to named campaigns).
7. Assign operation profile: DECEPTION CONFIRMED / STRONG INDICATORS / AMBIGUOUS / NO EVIDENCE; file with audit trail.

## 7. Data Requirements

- Content captures with hashes and earliest-instance records.
- Account metadata snapshots for all actors in the amplification graph.
- Temporal and textual similarity analysis outputs.
- Infrastructure indicators (domains, hosting, toolkit fingerprints).
- Claim verdicts for all embedded assertions.

## 8. Approved Public Sources

Platform transparency reports, public takedown archives, academic disinformation research, fact-checker investigations, open-source intelligence on influence operations, court records on fraud/fabrication, and leaked-platform-data analyses that are lawfully obtained and ethically handled per `legal/`.

## 9. Source Verification Standards

Deception findings require the same rigor as any accusation: document the evidence for fabrication and coordination, state alternative explanations, and grade confidence. Public attribution of operations to states or organizations requires the highest bar — prefer "consistent with" language over definitive claims unless evidence is conclusive.

## 10. Analytical Framework

Use the **Deception Indicator Stack**: (1) content fabrication evidence, (2) coordination signatures, (3) deceptive persona/infrastructure, (4) strategic narrative consistency, (5) beneficiary analysis. No single indicator proves disinformation; convergent stacks do. Score per `evidence_confidence_scoring.md`.

## 11. Evidence Requirements

Operation profiles require: all content captures with provenance, the origin map, coordination analysis outputs, infrastructure indicators, claim verdicts, intent reasoning with alternatives considered, and confidence grade. Profiles lacking the coordination layer are content assessments, not operation findings.

## 12. Confidence Assessment

| Level | Criteria |
|---|---|
| HIGH | Fabricated content + documented coordination + deceptive infrastructure, convergent |
| MODERATE | Strong coordination signatures or fabrication evidence, intent probable |
| LOW | Suspicious patterns with plausible benign explanations — flag as candidate operation |
| INSUFFICIENT | No deception evidence; item may still be false (see misinformation file) |

## 13. Common Analytical Mistakes

- Calling coordinated amplification "grassroots" or "organic" without network analysis.
- Confusing state-aligned voices (which may be sincere) with covert operations.
- Over-attributing to states based on narrative convenience; intent ≠ sponsorship.
- Ignoring that authentic content can be weaponized by inauthentic amplifiers.
- Treating platform enforcement actions as proof of deception without independent review.

## 14. Ethical Considerations

Disinformation findings can be politically explosive. Publish with evidence links, state confidence explicitly, correct promptly, and avoid naming private individuals as operators without documented evidence. Defensive analysis only — ANBU does not conduct influence operations or recommend them.

## 15. Security Boundaries

Strictly defensive and analytical. No engagement with operator infrastructure, no counter-disinformation campaigns, no impersonation, no amplification of the deceptive content. Operation packages to `security/` exclude operational details that could aid the adversary.

## 16. Expected Output

Operation profiles with full evidence chains; threat packages for `security/`; public corrections via `fact_checking_methodology.md` when appropriate; ecosystem trend data for `analytics/`.

## 17. Quality Checklist

- [ ] Falsity verified independently of intent
- [ ] Origin map and earliest instance documented
- [ ] Coordination analysis performed
- [ ] Infrastructure indicators recorded
- [ ] Intent reasoning with alternatives documented
- [ ] Confidence grade assigned
- [ ] Attribution language calibrated to evidence

## 18. Cross-Reference Links

- Verification base: `claim_verification.md`, `misinformation_detection.md`, `propaganda_analysis.md`, `fact_checking_methodology.md`
- Media forensics: `manipulated_media_assessment.md`, `image_authenticity_assessment.md`, `video_authenticity_assessment.md`
- Records: `source_provenance_tracking.md`, `evidence_chain_management.md`, `verification_audit_trail.md`
- Divisions: `security/` (operations), `osint/` (collection), `analytics/` (network analysis), `reporting/`
