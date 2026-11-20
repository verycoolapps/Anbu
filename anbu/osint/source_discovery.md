# Source Discovery

> ANBU OSINT Division 002 — Collection Tradecraft

## Purpose

Provides systematic procedures for discovering publicly accessible sources relevant to an analytical requirement, before any collection effort is committed.

## Scope

Covers discovery across all source classes: institutional portals, search engines, archives, registries, social platforms, and geospatial repositories.

## Intelligence objectives

- Find authoritative and primary sources before secondary aggregators
- Map the source ecosystem for a given topic, entity, or jurisdiction
- Identify access constraints (authentication, paywall, geographic restriction) early
- Build a candidate source inventory for prioritization

## Core concepts

- Source discovery versus source collection: discovery finds where information lives; collection retrieves it
- Primary, secondary, and tertiary source hierarchy
- Institutional versus individual source classes
- Access taxonomy: open, registered, paywalled, restricted

## Analytical methodology

Discovery proceeds from the requirement outward. Start with the owning institution (the entity that produces the information). Trace upward to aggregators and indexes. Use domain enumeration, certificate transparency logs, and search operators to expand coverage. For each candidate source, record authority, scope, update frequency, access method, and reliability prior.

## Step-by-step workflow

1. List candidate institutions and platforms from the requirement
2. Enumerate official portals, registries, and publications indexes
3. Use search operators and site: queries to find document-level sources
4. Check archives and caches for historical coverage
5. Record candidates in a discovery worksheet with access assessment
6. Hand candidate list to collection_prioritization.md for ranking

## Data requirements

Analytical requirement; target entities (states, agencies, persons in public office, organizations); jurisdiction and time window; language requirements; known prior sources.

## Approved public sources

- Government and institutional portals
- UN system agencies and international organizations
- Search engine indexes
- Web archives (Wayback Machine, archive.today)
- Domain registration and certificate transparency records
- Academic index pages and repository catalogs

## Source verification standards

Every source is evaluated for authority, proximity to the event or subject, currency, and internal consistency before its content is used analytically. Primary sources are preferred over secondary accounts. Where sources conflict, the conflict is preserved and reported rather than silently resolved. Source reliability is rated on the ANBU reliability scale and recorded in the collection log.

## Analytical framework

Sources are scored on four axes: authority (who produces it), proximity (primary vs derivative), coverage (does it span the requirement), and access (open vs restricted). Candidates scoring low on authority or coverage are deprioritized unless they uniquely fill a gap.

## Evidence requirements

Every analytical claim must be traceable to a logged collection item. Evidence requirements: (1) verbatim quotation or precise paraphrase with page/section reference; (2) source attribution including URL or archive identifier; (3) collection timestamp; (4) access method; (5) confidence grade per the ANBU scale. Claims without logged evidence are marked INSUFFICIENT and excluded from analytical products.

## Confidence assessment

HIGH: multiple independent primary sources, direct documentation, no material contradictions. MODERATE: credible sources with minor gaps or single-source primary documentation. LOW: indirect, derivative, or partially corroborated reporting. INSUFFICIENT: evidence does not support a judgment; collection gap or contested sources prevent assessment.

## Common analytical mistakes

- Anchoring on the first plausible source and stopping
- Discovering only English-language sources for non-English topics
- Confusing a derivative aggregator with the originating institution
- Ignoring archived copies of since-removed official pages

## Ethical considerations

Discovery uses only public index and directory information. It does not probe restricted systems, attempt account creation to bypass registration walls for discovery purposes, or harvest personal data en masse.

## Security boundaries

No credential probing, no exploitation of directory-listing misconfigurations, no scraping behind authentication. Discovery must respect rate limits and not degrade target service availability.

## Expected output

A ranked candidate source inventory with access notes, coverage estimates, and recommended collection order.

## Quality checklist

- [ ] Candidate sources span primary and secondary classes
- [ ] Access constraints recorded for each candidate
- [ ] At least one authoritative primary source identified per objective
- [ ] Discovery worksheet retained for audit

## Cross-reference links

- `osint_methodology.md`
- `search_engine_research.md`
- `advanced_search_operators.md`
- `government_open_data.md`
- `collection_prioritization.md`

