# DEFENSE PROCUREMENT WORKFLOW

## Purpose
Analyze defense procurement programs using public sources: requirements, tendering, contract awards, delivery schedules, industrial participation, offsets, and strategic implications.

## Scope
National defense procurement for any country, including Indonesia's defense modernization (Kementerian Pertahanan, PT Pindad, PT Dirgantara Indonesia, PT PAL, TNI and Polri acquisitions). Focuses on the procurement cycle from announcement to delivery, not classified weapons performance.

## Intelligence objectives
Determine what a country is buying, from whom, at what cost, on what timeline, and what that signals about threat perception, industrial policy, alliance alignment, and budget priorities.

## Core concepts
This workflow operationalizes ANBU's public-source intelligence discipline for its domain. It presumes the 10-step user interaction protocol (`core/user_interaction_protocol.md`), the seven-label evidence vocabulary (`core/intelligence_framework.md`), and the three-dimensional confidence model (`core/confidence_framework.md`). A workflow is a repeatable playbook: given trigger conditions, it sequences division inputs, collection methods, analytical techniques, decision points, quality gates, and the expected product. It never authorizes classified access, operational targeting, or fabricated capability.

## Analytical methodology
End-to-end pipeline: **requirement definition → collection planning → collection → validation → analysis → production → review**. Each phase has explicit entry and exit criteria; work does not advance until the prior phase's quality gate is met. Evidence is labeled at acquisition and re-graded at review. Structured analytic techniques (ACH, key assumptions check, indicator monitoring, scenario analysis) are applied where the domain warrants. All findings are source-linked; inference is always marked.

## Step-by-step workflow
1) **Requirement definition** — decompose the request into intelligence requirements (IRs/PIRs); classify the task per `core/task_classification.md`; assign an analytic confidence target.
2) **Collection planning** — select source classes, languages, and divisions; define collection windows, geographic scope, and the two-source corroboration rule; flag ethical and legal constraints.
3) **Collection** — acquire material; log provenance (URL, timestamp UTC, retrieval method, language) for every item; preserve originals where lawful.
4) **Validation** — run authenticity and provenance checks per `verification/`; grade each item FACT/VERIFIED/UNVERIFIED/ASSESSMENT/INFERENCE/HYPOTHESIS/SPECULATION.
5) **Analysis** — apply the domain analytical framework; generate competing hypotheses; test against evidence; identify key assumptions and disconfirming indicators.
6) **Production** — draft the product per `reporting/` templates and `core/output_standards.md`; assign three-dimensional confidence (source, information, analytical).
7) **Review** — pass all 9 quality gates; conduct red-team/alternative-analysis review where stakes are high; finalize grading and limitations statement.
8) **Variant note** — Indonesia variant: monitor Kemhan (Kementerian Pertahanan), TNI modernization programs, PT Pindad and PT DI production capacity, domestic content requirements, and the influence of defense diplomacy (joint exercises, port visits) on procurement choices.

### Trigger conditions
Activate this workflow when the request concerns: national defense procurement for any country, including indonesia's defense modernization (kementerian pertahanan, pt pindad, pt dirgantara indonesia, pt pal, tni and polri acquisitions). Typical triggers: user questions matching the domain taxonomy in `core/intelligence_taxonomy.md`, recurring monitoring requirements, or event-driven tasks where timeliness matters. If the request is narrower than this workflow's scope, decompose it and run only the relevant phases; if broader, split it across sibling workflows and synthesize in `comprehensive_intelligence_assessment.md`.

### Division activation map
Activates core/, osint/, military/, state/, legal/, geopolitical/, verification/, analytics/, reporting/. Adds security/ for counter-intelligence considerations and geoint/ for industrial geography and infrastructure.

### Decision points
- After requirement definition: if the question cannot be answered from public sources, state the boundary and propose the nearest feasible OSINT answer.
- After validation: if corroboration fails, downgrade confidence and flag contested claims rather than dropping them silently.
- After analysis: if competing hypotheses remain viable, present them with likelihoods instead of forcing a single verdict.
- Before production: if ethical or security boundaries are implicated, consult `legal/ethical_review_checklist.md` and document the decision.

### Phase detail
- **Phase A — Requirements and budget signals** — Identify the strategic driver: threat perception, alliance obligation, industrial policy, or regime security. Trace budget allocations and parliamentary approval debates.
- **Phase B — Tender and award tracking** — Monitor tender announcements, bidder lists, evaluation criteria, and award decisions; compare announced vs. actual contract values and timelines.
- **Phase C — Delivery and capability assessment** — Track delivery schedules, testing, training, and initial operating capability; assess what the delivered system actually changes versus what was announced.
- **Phase D — Strategic interpretation** — Synthesize across programs to judge the direction of military modernization: expeditionary vs. territorial, high-tech vs. mass, indigenous vs. imported.


### Indonesia-specific variant
Indonesia variant: monitor Kemhan (Kementerian Pertahanan), TNI modernization programs, PT Pindad and PT DI production capacity, domestic content requirements, and the influence of defense diplomacy (joint exercises, port visits) on procurement choices.

## Data requirements
Primary: defense ministry and armed forces public statements; secondary corroboration, metadata (timestamp UTC, source, language, retrieval method), and analyst assumptions. Minimum viable dataset: at least two independent source classes for every load-bearing claim; single-source claims must be labeled UNVERIFIED or lower.

## Approved public sources
Defense ministry and armed forces public statements; procurement agency notices and tender documents; parliamentary budget approvals and committee reports; contract award announcements; defense industry reports and corporate disclosures; trade data (SIPRI, IISS, national customs); diplomatic statements; audit reports; defense exhibition and trade press.

## Source verification standards
Two-source rule where feasible; document chain of custody; flag single-source claims; record retrieval timestamps (UTC); preserve originals where lawful; distinguish primary from secondary sources; treat social-media and messaging-app material as leads until corroborated; verify geolocation and imagery metadata per `verification/` and `geoint/geospatial_source_verification.md`.

## Analytical framework
Structured matrix linking observations to sources, dates, locations, and confidence levels; competing-hypotheses generation; key-assumptions check; indicator-based monitoring for ongoing developments; scenario analysis where futures are at stake; explicit separation of FACT/VERIFIED/UNVERIFIED/ASSESSMENT/INFERENCE/HYPOTHESIS/SPECULATION per `core/intelligence_framework.md`.

## Evidence requirements
Every claim must cite a source, date, and method; inferences must be labeled as such; forecasts must state assumptions and uncertainty ranges; contested claims must present both sides with their evidence; absence of evidence must be stated as such, not filled with plausible narrative; quantitative claims must state the dataset and its limitations.

## Confidence assessment
- **HIGH** — multiple independent corroborations across source classes; strong provenance; convergent analysis.
- **MODERATE** — two or more sources with minor gaps; partial corroboration; some contested elements.
- **LOW** — single source or weak corroboration; significant gaps; high dependence on inference.
- **INSUFFICIENT** — cannot be assessed from public sources; evidence base absent, inaccessible, or irretrievably contested.
Report all three dimensions (source, information, analytical) per `core/confidence_framework.md`; a product may legitimately carry HIGH source confidence with LOW analytical confidence.

## Common analytical mistakes
Conflating announced programs with delivered capability; treating contract value as procurement cost (ignoring offsets and in-kind transfers); ignoring domestic industrial politics; assuming all purchases are for external threats (some are for regime security); failing to track delivery delays and cancellation rates; ignoring the role of corruption in procurement.

## Ethical considerations
Do not publish information that could reveal operational vulnerabilities or assist adversaries in targeting; avoid naming individual soldiers or contractors in sensitive contexts; respect export-control restrictions; do not speculate on classified capabilities beyond public evidence. All products pass `legal/ethical_review_checklist.md`; personal data is minimized per `legal/personal_data_minimization.md`; political neutrality is maintained per `legal/political_neutrality_policy.md`.

## Security boundaries
Public sources only — no classified access is claimed or simulated. Never attempt to bypass access controls, decrypt restricted feeds, use stolen credentials, or facilitate operational harm. Do not publish information that could endanger individuals, critical infrastructure, or ongoing negotiations. Comply with `legal/lawful_osint_boundaries.md`, `legal/classified_information_exclusion.md`, and `legal/sovereignty_and_jurisdiction.md`.

## Expected output
Structured findings with confidence ratings, source appendix, explicit limitations, and a decision-relevant bottom line per `core/output_standards.md` and `reporting/` templates. Deliverables: executive summary, graded findings, source appendix, uncertainty statement, and indicator watchlist where applicable.

## Quality checklist
- [ ] Sources documented with provenance and timestamps
- [ ] Evidence labels applied to every claim
- [ ] Three-dimensional confidence reported
- [ ] Competing hypotheses considered
- [ ] Limitations and uncertainties stated
- [ ] Ethical and security boundaries respected
- [ ] All 9 quality gates passed
- [ ] Cross-references to sibling workflows and divisions complete

## Cross-reference links

**Sibling workflows:**
- [`country_intelligence_workflow`](country_intelligence_workflow.md)
- [`political_crisis_workflow`](political_crisis_workflow.md)
- [`government_transition_workflow`](government_transition_workflow.md)
- [`election_monitoring_workflow`](election_monitoring_workflow.md)
- [`military_modernization_workflow`](military_modernization_workflow.md)
- [`geopolitical_crisis_workflow`](geopolitical_crisis_workflow.md)
- [`international_conflict_workflow`](international_conflict_workflow.md)
- [`diplomatic_development_workflow`](diplomatic_development_workflow.md)
- [`public_policy_investigation_workflow`](public_policy_investigation_workflow.md)
- [`corruption_public_record_workflow`](corruption_public_record_workflow.md)
- [`strategic_infrastructure_workflow`](strategic_infrastructure_workflow.md)
- [`international_sanctions_workflow`](international_sanctions_workflow.md)
- [`national_security_policy_workflow`](national_security_policy_workflow.md)
- [`public_disinformation_investigation`](public_disinformation_investigation.md)
- [`strategic_forecasting_workflow`](strategic_forecasting_workflow.md)
- [`multi_country_comparison_workflow`](multi_country_comparison_workflow.md)
- [`comprehensive_intelligence_assessment`](comprehensive_intelligence_assessment.md)

**Division references:**
- `core/` — core doctrine, protocols, confidence, QA
- `osint/` — collection tradecraft, source classes
- `political/` — elections, parties, elites, public opinion
- `military/` — force posture, procurement, doctrine
- `state/` — governance, bureaucracy, institutions
- `geopolitical/` — alliances, conflicts, sanctions
- `verification/` — authenticity, provenance, corroboration
- `analytics/` — indicators, forecasting, structured techniques
- `geoint/` — geospatial analysis, imagery, terrain
- `legal/` — law, regulation, treaties, accountability
- `security/` — threats, risks, protective intelligence
- `reporting/` — formats, templates, dissemination

**Core protocols:** `../core/user_interaction_protocol.md`, `../core/task_classification.md`, `../core/intelligence_framework.md`, `../core/confidence_framework.md`, `../core/output_standards.md`
