# Public Timeline Collection

> ANBU OSINT Division 002 — Collection Tradecraft

## Purpose

Defines methods for building chronological timelines from public sources: event sequences, policy timelines, and organizational histories.

## Scope

Timeline construction across all OSINT source classes for events, policies, and organizational activities.

## Intelligence objectives

- Build accurate chronological sequences
- Standardize timestamp handling across sources
- Identify temporal patterns and correlations
- Support event reconstruction and trend analysis

## Core concepts

- Timestamp standardization
- Relative versus absolute time
- Timeline granularity
- Source timestamp reliability
- Timeline visualization

## Analytical methodology

Collect timestamped items from all sources. Standardize to UTC where possible; note original timezones. Record source publication time versus event time. Build master timeline. Identify temporal clusters and gaps. Visualize for analysis. Grade timestamp reliability per source.

## Step-by-step workflow

1. Define timeline scope
2. Collect timestamped items
3. Standardize timestamps
4. Build master timeline
5. Identify patterns and gaps
6. Produce timeline with confidence grading

## Data requirements

Timeline scope; time period; source types; timezone handling requirements.

## Approved public sources

- All OSINT source classes with timestamps
- Official records with dates
- News reports with publication times
- Social media posts with timestamps
- Archive snapshots with capture dates

## Source verification standards

Every source is evaluated for authority, proximity to the event or subject, currency, and internal consistency before its content is used analytically. Primary sources are preferred over secondary accounts. Where sources conflict, the conflict is preserved and reported rather than silently resolved. Source reliability is rated on the ANBU reliability scale and recorded in the collection log.

## Analytical framework

Timelines grade timestamp reliability by source type. Publication time is distinguished from event time. Gaps are documented as potential collection gaps or genuine lulls. Temporal patterns are flagged for analysis.

## Evidence requirements

Every analytical claim must be traceable to a logged collection item. Evidence requirements: (1) verbatim quotation or precise paraphrase with page/section reference; (2) source attribution including URL or archive identifier; (3) collection timestamp; (4) access method; (5) confidence grade per the ANBU scale. Claims without logged evidence are marked INSUFFICIENT and excluded from analytical products.

## Confidence assessment

HIGH: multiple independent primary sources, direct documentation, no material contradictions. MODERATE: credible sources with minor gaps or single-source primary documentation. LOW: indirect, derivative, or partially corroborated reporting. INSUFFICIENT: evidence does not support a judgment; collection gap or contested sources prevent assessment.

## Common analytical mistakes

- Mixing publication time with event time
- Ignoring timezone differences
- Missing timestamp precision variations
- Treating timeline gaps as meaningful without checking collection coverage

## Ethical considerations

Build timelines from public sources. Do not create timelines targeting private individuals.

## Security boundaries

No timeline construction for stalking or targeting.

## Expected output

Timeline report with standardized timestamps, event nodes, confidence grading, and visualization.

## Quality checklist

- [ ] Timestamps standardized
- [ ] Event vs publication time distinguished
- [ ] Gaps documented
- [ ] Confidence graded

## Cross-reference links

- `public_event_reconstruction.md`
- `source_collection_log.md`
- `news_media_monitoring.md`
- `osint_methodology.md`
- `collection_quality_control.md`

