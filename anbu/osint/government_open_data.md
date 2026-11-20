# Government Open Data

> ANBU OSINT Division 002 — Collection Tradecraft

## Purpose

Defines procedures for collecting and analyzing data published by government open data portals at national, subnational, and municipal levels.

## Scope

Covers national open data portals (data.gov, data.gov.uk, EU data portals), ministry datasets, municipal open data, and government statistical releases.

## Intelligence objectives

- Identify authoritative government datasets relevant to requirements
- Understand portal structures, update cadences, and API access
- Assess dataset quality, licensing, and methodology notes
- Correlate government data with other source classes

## Core concepts

- Open data licensing (CC-BY, OGL, national variants)
- Dataset versus release versus API
- Statistical methodology notes and revision policies
- Proactive versus reactive government publication

## Analytical methodology

Locate the portal through official government domains. Enumerate datasets by category, publisher, and update frequency. Prefer bulk downloads and documented APIs over manual scraping. Record dataset identifiers, versions, and retrieval dates. Check methodology and changelog documents before analysis.

## Step-by-step workflow

1. Identify relevant government level and agencies
2. Locate portal and dataset catalog
3. Filter by category, geography, and update frequency
4. Download dataset or document API access terms
5. Record version, retrieval timestamp, license
6. Cross-check methodology notes before analytical use

## Data requirements

Target government level and jurisdictions; statistical or administrative domains; time series requirements; acceptable licenses.

## Approved public sources

- National open data portals (data.gov, data.gov.uk, data.europa.eu, national equivalents)
- Ministry and agency publication pages
- Municipal open data portals
- Government statistical offices and census bureaus
- Official gazettes and legal databases

## Source verification standards

Every source is evaluated for authority, proximity to the event or subject, currency, and internal consistency before its content is used analytically. Primary sources are preferred over secondary accounts. Where sources conflict, the conflict is preserved and reported rather than silently resolved. Source reliability is rated on the ANBU reliability scale and recorded in the collection log.

## Analytical framework

Government data is treated as authoritative for what it measures, but methodology notes govern interpretation. Figures are cross-checked across releases and, where possible, independent sources. Dataset versions are pinned for reproducibility.

## Evidence requirements

Every analytical claim must be traceable to a logged collection item. Evidence requirements: (1) verbatim quotation or precise paraphrase with page/section reference; (2) source attribution including URL or archive identifier; (3) collection timestamp; (4) access method; (5) confidence grade per the ANBU scale. Claims without logged evidence are marked INSUFFICIENT and excluded from analytical products.

## Confidence assessment

HIGH: multiple independent primary sources, direct documentation, no material contradictions. MODERATE: credible sources with minor gaps or single-source primary documentation. LOW: indirect, derivative, or partially corroborated reporting. INSUFFICIENT: evidence does not support a judgment; collection gap or contested sources prevent assessment.

## Common analytical mistakes

- Using preliminary figures without noting revision risk
- Ignoring license terms on redistribution
- Comparing datasets with different methodologies or geographies
- Failing to record which dataset version was used

## Ethical considerations

Use only data published under open licenses or public access provisions. Respect license attribution requirements. Do not use government portals to probe non-public systems.

## Security boundaries

No scraping behind government authentication walls. No attempts to access classified or restricted government networks. Respect robots and API rate limits.

## Expected output

Dataset inventory with versions, licenses, coverage notes, and integration into analysis datasets.

## Quality checklist

- [ ] Dataset version and retrieval date recorded
- [ ] License terms documented
- [ ] Methodology notes reviewed
- [ ] Figures cross-checked where material

## Cross-reference links

- `public_registry_research.md`
- `parliamentary_document_research.md`
- `official_statement_collection.md`
- `international_dataset_research.md`
- `public_economic_database.md`

