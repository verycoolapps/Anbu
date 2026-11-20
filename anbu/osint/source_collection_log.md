# Source Collection Log

> ANBU OSINT Division 002 — Collection Tradecraft

## Purpose

Defines the standard format and procedures for the source collection log: the central record of all collection activity.

## Scope

All collection activity across all ANBU source classes, providing audit trail and provenance record.

## Intelligence objectives

- Record every collection item with full provenance
- Enable audit and reproducibility
- Track source reliability over time
- Support gap analysis and collection evaluation

## Core concepts

- Collection log as audit trail
- Provenance fields: source, URL, timestamp, access method
- Log entry lifecycle
- Log completeness and quality metrics

## Analytical methodology

Every collected item is logged with: unique ID, source name and URL, collection timestamp, access method, content type, relevance rating, reliability assessment, and notes. Logs are append-only; corrections are new entries, not edits. Logs are reviewed for completeness at collection cycle end.

## Step-by-step workflow

1. Create log entry for each collected item
2. Record all provenance fields
3. Assess relevance and reliability
4. Review log for completeness
5. Archive log with collection cycle
6. Use log for gap analysis and reporting

## Data requirements

Collection items; source information; timestamps; access methods; relevance criteria.

## Approved public sources

- All ANBU source classes
- Collection control registers
- Quality control checklists

## Source verification standards

Every source is evaluated for authority, proximity to the event or subject, currency, and internal consistency before its content is used analytically. Primary sources are preferred over secondary accounts. Where sources conflict, the conflict is preserved and reported rather than silently resolved. Source reliability is rated on the ANBU reliability scale and recorded in the collection log.

## Analytical framework

Log completeness is measured by percentage of items with all required fields. Provenance completeness is critical for verification. Log quality is assessed at cycle end; incomplete logs trigger collection review.

## Evidence requirements

Every analytical claim must be traceable to a logged collection item. Evidence requirements: (1) verbatim quotation or precise paraphrase with page/section reference; (2) source attribution including URL or archive identifier; (3) collection timestamp; (4) access method; (5) confidence grade per the ANBU scale. Claims without logged evidence are marked INSUFFICIENT and excluded from analytical products.

## Confidence assessment

HIGH: multiple independent primary sources, direct documentation, no material contradictions. MODERATE: credible sources with minor gaps or single-source primary documentation. LOW: indirect, derivative, or partially corroborated reporting. INSUFFICIENT: evidence does not support a judgment; collection gap or contested sources prevent assessment.

## Common analytical mistakes

- Incomplete provenance fields
- Editing log entries instead of appending
- Missing access method documentation
- Failing to review log completeness

## Ethical considerations

Logs contain only public-source collection records. No logging of private data or unlawful collection.

## Security boundaries

Logs must not contain credentials, private keys, or sensitive personal data.

## Expected output

Complete collection log with provenance records, reliability assessments, and completeness metrics.

## Quality checklist

- [ ] All fields complete
- [ ] Append-only maintained
- [ ] Completeness reviewed
- [ ] Archived with cycle

## Cross-reference links

- `osint_methodology.md`
- `collection_quality_control.md`
- `information_gap_analysis.md`
- `collection_requirement_definition.md`
- `source_discovery.md`

