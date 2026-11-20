# Advanced Search Operators

> ANBU OSINT Division 002 — Collection Tradecraft

## Purpose

Catalogs and operationalizes advanced search operators across engines and platforms for precision source discovery.

## Scope

Covers Google/Bing operators, Google Scholar syntax, social platform search syntax, archive search, and regulatory document search operators.

## Intelligence objectives

- Construct precise queries that exclude noise and target document classes
- Use filetype, site, date, and phrase operators effectively
- Apply platform-specific search syntax for social and professional networks
- Document operator usage standards for reproducibility

## Core concepts

- Boolean logic: AND, OR, NOT, quoted phrases
- Fielded search: site:, filetype:, intitle:, inurl:, intext:
- Temporal operators: after:, before:, daterange:
- Platform-specific operators versus general web operators

## Analytical methodology

Operators are selected based on requirement type. Entity queries use exact phrases and name variants. Document discovery uses filetype:pdf/doc/xls and site: scoping to known portals. Temporal scoping uses date operators and archive date filters. Platform syntax (e.g., social search filters, LinkedIn operators) is applied only where platform terms permit.

## Step-by-step workflow

1. Classify the query type (entity, document, temporal, site-scoped)
2. Select operator set per engine capabilities
3. Build and test query variants
4. Record which operators produced results versus noise
5. Refine and document final query strings

## Data requirements

Target entities; document types sought; date windows; known authoritative domains; platforms in scope.

## Approved public sources

- Google search operators
- Bing search operators
- Google Scholar advanced search
- Platform-specific search (X, LinkedIn, YouTube, Reddit public search)
- Archive.org and Wayback Machine search

## Source verification standards

Every source is evaluated for authority, proximity to the event or subject, currency, and internal consistency before its content is used analytically. Primary sources are preferred over secondary accounts. Where sources conflict, the conflict is preserved and reported rather than silently resolved. Source reliability is rated on the ANBU reliability scale and recorded in the collection log.

## Analytical framework

Operator usage is standardized: always quote multi-word entity names, use filetype only when document format is a requirement, scope by site: only after domain authority is confirmed, and always record the raw query string.

## Evidence requirements

Every analytical claim must be traceable to a logged collection item. Evidence requirements: (1) verbatim quotation or precise paraphrase with page/section reference; (2) source attribution including URL or archive identifier; (3) collection timestamp; (4) access method; (5) confidence grade per the ANBU scale. Claims without logged evidence are marked INSUFFICIENT and excluded from analytical products.

## Confidence assessment

HIGH: multiple independent primary sources, direct documentation, no material contradictions. MODERATE: credible sources with minor gaps or single-source primary documentation. LOW: indirect, derivative, or partially corroborated reporting. INSUFFICIENT: evidence does not support a judgment; collection gap or contested sources prevent assessment.

## Common analytical mistakes

- Chaining operators that engines silently ignore
- Using filetype: as a substitute for document-type filtering
- Assuming operator support is identical across engines
- Over-constraining queries until recall collapses

## Ethical considerations

Operators are used to narrow public results, never to evade access controls or target private data.

## Security boundaries

No operator use to locate or expose private individuals' non-public information. No automation designed to defeat rate limits.

## Expected output

Reusable query templates per source class, plus executed query log with operator annotations.

## Quality checklist

- [ ] Queries documented verbatim
- [ ] Operator use justified per query
- [ ] Recall and precision both considered
- [ ] Platform terms respected

## Cross-reference links

- `search_engine_research.md`
- `source_discovery.md`
- `public_pdf_research.md`
- `public_social_media_research.md`
- `media_archive_research.md`

