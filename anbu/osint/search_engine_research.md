# Search Engine Research

> ANBU OSINT Division 002 — Collection Tradecraft

## Purpose

Governs the use of general-purpose web search engines as an OSINT discovery and collection surface, covering query construction, result triage, and coverage estimation.

## Scope

Applies to use of Google, Bing, DuckDuckGo, Brave, Yandex, Baidu, Naver and regional engines for source discovery and targeted retrieval of public pages.

## Intelligence objectives

- Build reproducible queries that surface relevant public documents
- Estimate search coverage and detect result-set saturation
- Triage results by authority and proximity before collection
- Document queries verbatim for audit and re-execution

## Core concepts

- Search engine as index of public web, not archive of record
- Query classes: entity, document type, site-scoped, temporal, linguistic
- Result saturation: when new queries yield diminishing returns
- SERP features (news, images, scholar, patents) as separate indexes

## Analytical methodology

Queries are constructed from requirement keywords, entity names (including native-language variants and former names), document type terms, and temporal bounds. Site-scoped queries target known domains. Results are triaged by domain authority, date, and document class. Saturation is tested by rephrasing with synonyms and alternate scripts until new relevant results drop below threshold.

## Step-by-step workflow

1. Extract entities and document types from the requirement
2. Generate base query set plus linguistic variants
3. Execute queries; record verbatim queries and result counts
4. Triage top results; open candidates to verify content and access
5. Test saturation with synonym and operator variants
6. Export result list and query log into the collection log

## Data requirements

Requirement keywords; entity name variants; target document types; languages; date range; known relevant domains for site: scoping.

## Approved public sources

- Google, Bing, DuckDuckGo, Brave Search
- Google Scholar and regional scholarly indexes
- News verticals (Google News, Bing News)
- Regional engines for non-English coverage (Yandex, Baidu, Naver, Seznam)

## Source verification standards

Every source is evaluated for authority, proximity to the event or subject, currency, and internal consistency before its content is used analytically. Primary sources are preferred over secondary accounts. Where sources conflict, the conflict is preserved and reported rather than silently resolved. Source reliability is rated on the ANBU reliability scale and recorded in the collection log.

## Analytical framework

Each result is scored for authority (official/primary/secondary), freshness, and relevance. Queries are tagged by type (entity, document, site, temporal). Coverage is declared sufficient when three consecutive query variants return no new relevant primary sources.

## Evidence requirements

Every analytical claim must be traceable to a logged collection item. Evidence requirements: (1) verbatim quotation or precise paraphrase with page/section reference; (2) source attribution including URL or archive identifier; (3) collection timestamp; (4) access method; (5) confidence grade per the ANBU scale. Claims without logged evidence are marked INSUFFICIENT and excluded from analytical products.

## Confidence assessment

HIGH: multiple independent primary sources, direct documentation, no material contradictions. MODERATE: credible sources with minor gaps or single-source primary documentation. LOW: indirect, derivative, or partially corroborated reporting. INSUFFICIENT: evidence does not support a judgment; collection gap or contested sources prevent assessment.

## Common analytical mistakes

- Treating search ranking as credibility ranking
- Over-reliance on a single engine's index
- Ignoring non-English queries for global topics
- Failing to save verbatim queries, making work non-reproducible

## Ethical considerations

Use search engines within their published terms. Do not automate queries at volumes that constitute abuse, do not bypass CAPTCHAs, and do not use search to locate private individuals for exposure.

## Security boundaries

No CAPTCHA bypass, no automated scraping of SERPs at abusive volume, no use of leaked search API keys. Respect engine rate limits and robots policies.

## Expected output

Query log with verbatim queries, result counts, triaged source list, and saturation assessment.

## Quality checklist

- [ ] Verbatim queries recorded
- [ ] Multiple engines and languages used where topic warrants
- [ ] Saturation tested and documented
- [ ] Results triaged by authority before collection

## Cross-reference links

- `advanced_search_operators.md`
- `source_discovery.md`
- `news_media_monitoring.md`
- `public_social_media_research.md`
- `osint_methodology.md`

