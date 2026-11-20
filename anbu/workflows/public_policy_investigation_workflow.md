# PUBLIC POLICY INVESTIGATION WORKFLOW

## Purpose
Investigate public policy development and implementation: agenda-setting, formulation, adoption, implementation, and evaluation, using public sources to assess effectiveness, equity, and unintended consequences.

## Scope
Domestic public policy in any country, including Indonesia's policy landscape (economic, social, environmental, digital, health). Focuses on the policy cycle and its outcomes, not classified policy options.

## Intelligence objectives
Determine how a policy was developed, who influenced it, what it aims to achieve, how it is implemented, and what its actual effects are on different groups.

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
8) **Variant note** — Indonesia variant: incorporate Bappenas (National Development Planning Agency), ministry policy documents, BPK audit findings, and the role of regional governments (pemda) and village-level implementation in policy delivery.

### Trigger conditions
Activate this workflow when the request concerns: domestic public policy in any country, including indonesia's policy landscape (economic, social, environmental, digital, health). Typical triggers: user questions matching the domain taxonomy in `core/intelligence_taxonomy.md`, recurring monitoring requirements, or event-driven tasks where timeliness matters. If the request is narrower than this workflow's scope, decompose it and run only the relevant phases; if broader, split it across sibling workflows and synthesize in `comprehensive_intelligence_assessment.md`.

### Division activation map
Activates core/, osint/, state/, legal/, political/, analytics/, verification/, reporting/. Adds security/ for national security policy and geoint/ for spatial policy impacts.

### Decision points
- After requirement definition: if the question cannot be answered from public sources, state the boundary and propose the nearest feasible OSINT answer.
- After validation: if corroboration fails, downgrade confidence and flag contested claims rather than dropping them silently.
- After analysis: if competing hypotheses remain viable, present them with likelihoods instead of forcing a single verdict.
- Before production: if ethical or security boundaries are implicated, consult `legal/ethical_review_checklist.md` and document the decision.

### Phase detail
- **Phase A — Policy genealogy** — Trace the policy from agenda-setting through formulation, adoption, implementation, and evaluation; identify the key actors, institutions, and ideas at each stage.
- **Phase B — Design and intent analysis** — Analyze the policy's stated objectives, instruments, targeting, and theory of change; identify assumptions and implicit trade-offs.
- **Phase C — Implementation and outcome assessment** — Compare design with actual implementation and outcomes; use budget data, statistics, and field-level reporting; assess distributional effects across regions and groups.
- **Phase D — Effectiveness and reform assessment** — Judge whether the policy achieves its objectives, at what cost, and with what unintended consequences; identify reform options implied by the evidence.


### Indonesia-specific variant
Indonesia variant: incorporate Bappenas (National Development Planning Agency), ministry policy documents, BPK audit findings, and the role of regional governments (pemda) and village-level implementation in policy delivery.

## Data requirements
Primary: government policy documents and white papers; secondary corroboration, metadata (timestamp UTC, source, language, retrieval method), and analyst assumptions. Minimum viable dataset: at least two independent source classes for every load-bearing claim; single-source claims must be labeled UNVERIFIED or lower.

## Approved public sources
Government policy documents and white papers; legislative records and committee reports; budget allocations and expenditure data; regulatory agency publications; impact assessments; academic and think-tank evaluations; media coverage; stakeholder interviews (where public); freedom-of-information responses where lawful.

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
Treating policy announcements as policy outcomes; ignoring implementation gaps; failing to account for distributional effects; conflating correlation with causation; assuming policy coherence across government; neglecting the role of informal institutions and corruption; evaluating only intended objectives, not actual effects.

## Ethical considerations
Protect the privacy of individuals affected by policy; avoid publishing information that could endanger vulnerable groups; respect the confidentiality of whistleblowers; maintain neutrality between policy alternatives; do not advocate for specific policy outcomes. All products pass `legal/ethical_review_checklist.md`; personal data is minimized per `legal/personal_data_minimization.md`; political neutrality is maintained per `legal/political_neutrality_policy.md`.

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
- [`defense_procurement_workflow`](defense_procurement_workflow.md)
- [`military_modernization_workflow`](military_modernization_workflow.md)
- [`geopolitical_crisis_workflow`](geopolitical_crisis_workflow.md)
- [`international_conflict_workflow`](international_conflict_workflow.md)
- [`diplomatic_development_workflow`](diplomatic_development_workflow.md)
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
