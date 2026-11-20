# Political Communication Analysis

**Module:** political/political_communication_analysis
**Classification:** Public-source OSINT tradecraft — non-partisan
**Audience:** Intelligence analysts, researchers, policy staff

---

## 1. Purpose

Analyse how political actors communicate: official statements, speeches, press conferences, social-media strategy, media relations, narrative construction, and crisis communication. Focuses on public communications only.

## 2. Scope

This module covers Official statements, speeches, press releases, public social-media accounts, media interviews, and public appearances.. It does not cover Private communications, leaked documents, and covert information operations.. All work is limited to publicly available sources, official records, licensed databases, and lawful open-source collection. No classification, tasking authority, or operational access is implied or required.

## 3. Intelligence objectives

- Determine the formal and informal structure of political communication.
- Identify actors, institutions, and mechanisms that shape outcomes.
- Produce evidence-linked assessments with explicit confidence ratings.
- Generate hypotheses that can be tested against additional public reporting.
- Deliver reusable intelligence products for downstream analysis modules.

## 4. Core concepts

- **Actor:** an individual, institution, party, agency, or organized group whose behaviour matters.
- **Mechanism:** a rule, procedure, or informal practice that converts intent into outcome.
- **Signal vs. noise:** distinguishing deliberate information release from routine or accidental exposure.
- **Baseline:** the expected state against which change is measured.
- **Evidence tier:** the reliability of a source and the corroboration level of a claim.

## 5. Analytical methodology

Adopt a structured analytic cycle:

1. **Frame** the question and define what evidence would change the assessment.
2. **Collect** from approved public sources (see Section 9).
3. **Corroborate** each material claim across independent sources.
4. **Analyse** using the framework in Section 11.
5. **Challenge** the assessment via the techniques in Section 15.
6. **Deliver** the product defined in Section 18.

## 6. Step-by-step workflow

1. Receive the collection or analysis requirement; restate it as testable propositions.
2. Inventory available public sources; record access date and retrieval method.
3. Build an actor/institution list; rank by relevance and accessibility.
4. Collect primary documents first (statutes, official records, transcripts, filings).
5. Layer secondary reporting; flag contradictions rather than smoothing them.
6. Apply the Section 11 framework; produce intermediate notes with citations.
7. Run the Section 12 confidence assessment per claim.
8. Draft the Section 18 output; run the Section 19 checklist before release.

## 7. Data requirements

| Requirement | Minimum standard |
|---|---|
| Date stamps | Every source entry carries collection date and publication date |
| Primary-source ratio | At least 40% of material claims trace to primary documents |
| Corroboration | HIGH-confidence claims need two independent sources |
| Provenance | Original URL, document ID, or archive reference preserved |
| Provenance | Original URL, document ID, or archive reference preserved |
| Sensitivity review | Output screened for personal-data and safety exposure |

## 8. Approved public sources
n- **Official gazettes and statute repositories** (see module cross-references).
- **Electoral commissions, parliaments, courts, ministries** — official portals.
- **Company and campaign-finance registers** where public by law.
- **Reputable wire services, major newspapers, academic presses.**
- **Open government datasets, Freedom-of-Information releases.**
- **Social-media and messaging platforms** for public discourse analysis only.

## 9. Source verification standards

- Prefer primary documents over reporting about them.
- Two-source rule for material claims; three for HIGH confidence on contested topics.
- Check for syndication: the same wire story under different headlines is one source.
- Reverse-image and metadata checks on photographs and videos before use.
- Archive URLs where possible; note link-rot risk.
- Record language of source; machine-translated text is flagged as such.
- See ../verification/source_authentication.md and ../verification/chain_of_custody.md for full procedure.

## 10. Analytical framework

Use the staged framework in Section 11: (a) descriptive mapping, (b) relational analysis, (c) explanatory hypotheses, (d) predictive assessment with confidence. Never skip from observation to prediction without documenting the intermediate steps. See ../analytics/analytic_frameworks.md and ../core/collection_plan.md.

## 11. Evidence requirements

- Every claim must be traceable to a numbered source entry.
- Distinguish fact, assessment, and speculation explicitly in the text.
- Quantitative claims require the dataset, method, and date range.
- Absence of evidence is recorded as such — never converted into evidence of absence.

## 12. Confidence assessment

Apply the standard tiers from ../core/confidence_framework.md:

- **HIGH:** multiple independent primary or highly reliable secondary sources; low ambiguity.
- **MODERATE:** credible sources with minor gaps or single-source primary confirmation.
- **LOW:** plausible but under-corroborated; alternative explanations remain open.
- **INSUFFICIENT:** evidence does not support a defensible assessment; state what is missing.

## 13. Common analytical mistakes

- Mirroring the loudest narrative instead of testing it.
- Treating official statements as ground truth without checking implementation.
- Overweighting a single high-profile source.
- Ignoring base rates and structural constraints.
- Letting political preference shape source weighting.
- Conflating correlation in public data with causation.

## 14. Ethical considerations

- Non-partisan stance: analyse all actors under the same evidentiary standard.
- Protect sources and subjects: publish only what public-source analysis supports; avoid doxxing private individuals.
- Avoid harm amplification: do not produce targeting packages for harassment.
- Respect privacy law and platform terms; public availability is not the same as ethical licence for reuse.
- Clearly label assessments as assessments, not findings of fact.

## 15. Security boundaries

- No attempts to breach systems, access restricted data, or deceive platforms.
- No use of stolen credentials, leaked databases, or intercepted communications.
- No physical surveillance or contact with subjects.
- All collection is passive: reading what is already public.
- See ../security/legal_boundaries.md and ../security/ethics_review.md.

## 16. Indonesia Special Module

**IN:ID-1 — Indonesia political context.**

Indonesia is a presidential constitutional republic. Key institutions for this module:

- **Presidency and cabinet** — President elected directly for a five-year term, maximum two terms; vice-president on the same ticket.
- **DPR (House of Representatives)** — 580 members elected in multi-member constituencies; primary legislative body.
- **DPD (Regional Representative Council)** — 152 members representing provinces; reviews regional and local matters.
- **MPR (People's Consultative Assembly)** — joint sitting of DPR and DPD plus regional representatives; amends constitution, swears in president, and has impeachment power (MK decision, then MPR vote).
- **KPU** — General Elections Commission; administers elections and referendums.
- **MK (Constitutional Court)** — reviews laws against the constitution; resolves election disputes.
- **Parties** — parliamentary threshold historically 4% of national valid votes (raised to 4% then adjusted; verify current law — raised progressively, currently 4% for DPR seats under Law 7/2017 as amended). Major parties: PDI-P, Golkar, Gerindra, PKB, PKS, NasDem, Democratic Party, PAN, PPP, and newer entrants (PSI, Perindo, etc.).
- **Pemilu** — simultaneous legislative and presidential elections held every five years (2014, 2019, 2024, next 2029); pilkada (local elections) held separately every five years offset by ~2.5 years.
- **Regional dynamics** — significant autonomy under regional government law; governors and mayors directly elected since 2005.
- **Military and police** — formally apolitical under the TNI Law and POLRI Law, but civil-military relations remain analytically relevant.
- **Key analytical notes:** coalition fluidity is high; parties often support presidents without joining cabinets formally; KPU results and MK disputes are the authoritative record; English-language coverage varies in quality — use Indonesian-language primary sources (peraturan.go.id, dpr.go.id, mk.go.id, kp.go.id, news outlets like Kompas, Tempo, detik, Tirto).

## 17. Analytical stages detail

1. **Communication inventory** — catalogue official channels: websites, social media, press offices.
2. **Message analysis** — extract key themes, slogans, and policy positions from public statements.
3. **Channel strategy** — assess which channels are used for which audiences and purposes.
4. **Crisis communication** — analyse responses to scandals, disasters, and political crises.
5. **Media relations** — track press access, embargo patterns, and journalist relationships.
6. **Narrative construction** — identify recurring stories, frames, and rhetorical strategies.
7. **Effectiveness assessment** — evaluate public reception through polls and media coverage.

## 18. Expected output

- Structured intelligence brief with executive summary (max 300 words).
- Claims table: claim | source | confidence | date.
- Source register with URLs and collection timestamps.
- Map or network diagram where applicable (described or linked).
- Open questions and collection gaps for follow-up.
- See ../reporting/intelligence_product_standards.md and ../reporting/source_reliability_matrix.md.

## 19. Quality checklist

- [ ] Every material claim has a source and confidence tier.
- [ ] Primary sources preferred; secondary corroboration noted.
- [ ] Indonesia-specific institutions verified against current law.
- [ ] No classified or unlawfully obtained material.
- [ ] No personal-data exposure beyond public figures' official roles.
- [ ] Contradictions reported, not hidden.
- [ ] Output reviewed by second analyst where stakes are high.

## 20. Cross-reference links

- ../core/confidence_framework.md — confidence tier definitions
- ../core/collection_plan.md — collection planning
- ../osint/source_discovery.md — source discovery procedure
- ../verification/source_authentication.md — source authentication
- ../verification/chain_of_custody.md — evidence handling
- ../analytics/analytic_frameworks.md — analytical frameworks
- ../reporting/intelligence_product_standards.md — product standards
- ../security/legal_boundaries.md — legal boundaries
- ../workflows/standard_analysis_workflow.md — standard workflow
- - political_narrative_analysis.md
- political_campaign_public_analysis.md
- public_opinion_analysis.md
- political_leadership_analysis.md
