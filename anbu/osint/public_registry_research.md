# Public Registry Research

> ANBU OSINT Division 002 — Collection Tradecraft

## Purpose

Covers systematic research in public registries: corporate registries, property records, professional registries, vehicle and vessel registries, and licensing databases.

## Scope

National and subnational registries for companies, real estate, professionals, charities, and regulated entities, where access is public or lawfully available.

## Intelligence objectives

- Map ownership, directorship, and registration structures of public-interest entities
- Trace asset holdings and property interests where registries are public
- Verify professional credentials and licenses of public officials and contractors
- Document registration histories and status changes over time

## Core concepts

- Registry hierarchy: national versus subnational competence
- Entity versus beneficial ownership visibility
- Registry update lag and data currency
- Historical versus current registry snapshots

## Analytical methodology

Identify the competent registry for the jurisdiction and entity type. Use official search interfaces; where bulk data is published, prefer it. Record queries, result identifiers, and retrieval dates. For historical reconstruction, use archived registry pages and dated snapshots. Treat registry absence as a finding only after confirming coverage.

## Step-by-step workflow

1. Determine jurisdiction and entity type
2. Locate official registry and its search/bulk options
3. Execute searches by name, identifier, and related parties
4. Record registration numbers, statuses, and officers
5. Check historical snapshots for changes over time
6. Compile findings with registry citations

## Data requirements

Entity names and identifiers; jurisdiction(s); time window; related parties of interest; known registration numbers.

## Approved public sources

- National company registries (e.g., Companies House, national equivalents)
- Property and cadastral registries
- Professional licensing boards
- Charity and NGO registries
- Vessel and aircraft registries
- Sanctions and watchlist registries (see international_dataset_research.md)

## Source verification standards

Every source is evaluated for authority, proximity to the event or subject, currency, and internal consistency before its content is used analytically. Primary sources are preferred over secondary accounts. Where sources conflict, the conflict is preserved and reported rather than silently resolved. Source reliability is rated on the ANBU reliability scale and recorded in the collection log.

## Analytical framework

Registry data is authoritative for registration facts but silent on beneficial ownership unless disclosed. Findings are reported with registry identifier, query date, and caveat about coverage limits. Negative findings require documented search coverage.

## Evidence requirements

Every analytical claim must be traceable to a logged collection item. Evidence requirements: (1) verbatim quotation or precise paraphrase with page/section reference; (2) source attribution including URL or archive identifier; (3) collection timestamp; (4) access method; (5) confidence grade per the ANBU scale. Claims without logged evidence are marked INSUFFICIENT and excluded from analytical products.

## Confidence assessment

HIGH: multiple independent primary sources, direct documentation, no material contradictions. MODERATE: credible sources with minor gaps or single-source primary documentation. LOW: indirect, derivative, or partially corroborated reporting. INSUFFICIENT: evidence does not support a judgment; collection gap or contested sources prevent assessment.

## Common analytical mistakes

- Assuming registry silence means non-existence without checking jurisdiction coverage
- Ignoring name-similarity and transliteration variants
- Treating registered address as physical location
- Failing to record search date, breaking reproducibility

## Ethical considerations

Use registries for lawful public-interest research. Do not use registry data to build targeting packages against private individuals; focus on public-interest entities, officials, and organizations.

## Security boundaries

Do not attempt to bypass registry access controls or payment requirements through technical means. Do not combine registry data with other sources to expose private home addresses.

## Expected output

Registry extract tables with identifiers, statuses, officers, and temporal change notes, fully cited to registry records.

## Quality checklist

- [ ] Registry citations include identifier and retrieval date
- [ ] Negative results documented with search coverage
- [ ] Jurisdiction coverage confirmed
- [ ] No private residential data compiled

## Cross-reference links

- `government_open_data.md`
- `international_dataset_research.md`
- `public_financial_database.md`
- `information_gap_analysis.md`
- `osint_collection_ethics.md`

