# OSINT Collection Methodology

> ANBU OSINT Division 002 — Collection Tradecraft

## Purpose

Defines the governing methodology for all ANBU collection work: how collection is planned, executed, evaluated, and terminated under a single disciplined lifecycle.

## Scope

Applies to every ANBU collection task regardless of source class. It governs sequencing of collection phases, interaction with the source ecosystem, and hand-off into verification and analysis.

## Intelligence objectives

- Standardize collection planning so tasks begin with explicit requirements
- Enforce source evaluation before collection effort is spent
- Integrate collection quality control into the lifecycle rather than treating it as a post-step
- Provide a common vocabulary for collection status, confidence, and gaps

## Core concepts

- The collection lifecycle: requirement definition, planning, discovery, collection, logging, evaluation, gap analysis, termination
- Collection discipline: time-boxed collection windows and defined stopping conditions
- Source lifecycle states: candidate, active, exhausted, archived, rejected
- Requirement-driven collection versus fishing expeditions

## Analytical methodology

ANBU collection follows a seven-phase lifecycle. (1) Requirement definition fixes the question, scope, and success criteria. (2) Planning maps requirement to source classes and effort. (3) Discovery identifies candidate sources and access routes. (4) Collection executes capture with provenance preservation. (5) Logging records every item in the collection log. (6) Evaluation scores source reliability and item relevance. (7) Gap analysis determines whether requirements are met or a follow-on collection cycle is needed.

## Step-by-step workflow

1. Receive analytical requirement or collection tasking
2. Draft requirement definition with success criteria
3. Classify the requirement against source classes and modules
4. Prioritize collection slices under time and access constraints
5. Execute discovery, then targeted collection per source class
6. Record all items in the source collection log with timestamps and access method
7. Run gap analysis; iterate or terminate with documented rationale

## Data requirements

Analytical requirement statement; collection mandate or tasking authority; time window; geographic and entity scope; access constraints; any prior collection log from earlier cycles; relevant legal/ethical boundaries for the jurisdiction involved.

## Approved public sources

- All ANBU source classes: government open data, official statements, press releases, parliamentary records, academic databases, news and media archives, public social media, web archives, satellite and geospatial data, economic and financial databases
- Internal ANBU indexes and prior collection logs
- Collection control registers maintained under this division

## Source verification standards

Every source is evaluated for authority, proximity to the event or subject, currency, and internal consistency before its content is used analytically. Primary sources are preferred over secondary accounts. Where sources conflict, the conflict is preserved and reported rather than silently resolved. Source reliability is rated on the ANBU reliability scale and recorded in the collection log.

## Analytical framework

Requirements are decomposed into discrete collection objectives. Each objective is mapped to source classes by expected yield, access cost, and verification burden. Collection effort is allocated to maximize coverage of high-value objectives under constraints. Every collected item is scored on a relevance matrix before entering verification.

## Evidence requirements

Every analytical claim must be traceable to a logged collection item. Evidence requirements: (1) verbatim quotation or precise paraphrase with page/section reference; (2) source attribution including URL or archive identifier; (3) collection timestamp; (4) access method; (5) confidence grade per the ANBU scale. Claims without logged evidence are marked INSUFFICIENT and excluded from analytical products.

## Confidence assessment

HIGH: multiple independent primary sources, direct documentation, no material contradictions. MODERATE: credible sources with minor gaps or single-source primary documentation. LOW: indirect, derivative, or partially corroborated reporting. INSUFFICIENT: evidence does not support a judgment; collection gap or contested sources prevent assessment.

## Common analytical mistakes

- Collecting before requirements are written, producing volume without direction
- Treating all sources as equal rather than scoring reliability
- Failing to log access method and timestamp, breaking provenance
- Continuing collection after requirements are met, wasting effort and increasing exposure

## Ethical considerations

Collection is limited to information a lawful person could access without deception, credential abuse, or circumvention of technical access controls. Collection never targets private individuals for exposure; it serves analytical questions about public affairs.

## Security boundaries

Collect only from publicly reachable endpoints. No credential guessing, no bypass of paywalls or rate limits, no use of stolen or leaked data, no social engineering. Respect robots directives and platform terms where they reflect public access norms. Do not collect data whose storage or use would violate applicable law.

## Expected output

A completed collection cycle producing: requirement definition, collection log, source inventory with reliability ratings, gap analysis report, and hand-off package to verification/ and analysis divisions.

## Quality checklist

- [ ] Requirement definition exists before collection starts
- [ ] Every item logged with source URL, timestamp, access method
- [ ] Source reliability assessed for every source used
- [ ] Gap analysis completed before termination
- [ ] No restricted or unlawfully obtained material in the collection

## Cross-reference links

- `core/`
- `verification/`
- `legal/`
- `security/`
- `collection_requirement_definition.md`
- `source_collection_log.md`
- `collection_quality_control.md`
- `information_gap_analysis.md`

