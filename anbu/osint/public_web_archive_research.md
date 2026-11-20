# Public Web Archive Research

> ANBU OSINT Division 002 — Collection Tradecraft

## Purpose

Defines use of web archives (Wayback Machine, archive.today, national web archives) for historical web content and change detection.

## Scope

Internet Archive Wayback Machine, archive.today, national library web archives, and cached page services.

## Intelligence objectives

- Retrieve deleted or changed official pages
- Establish timelines of website changes
- Verify claims about what a page said at a given time
- Access content behind removed or geo-blocked pages

## Core concepts

- Snapshot versus live page
- Archive capture date versus page publication date
- Archive completeness and crawl gaps
- Redirect and canonical URL resolution

## Analytical methodology

Query archive CDX APIs for URL history. Retrieve snapshots nearest to target dates. Compare snapshots over time to detect changes. Record archive timestamps and original URLs. Note that archives are incomplete: absence of a snapshot does not prove absence of the page.

## Step-by-step workflow

1. Identify target URLs and date range
2. Query CDX API for snapshot index
3. Retrieve relevant snapshots
4. Diff snapshots for material changes
5. Record archive timestamps and URLs
6. Log findings with archive citations

## Data requirements

Target URLs; date range; specific content to verify; related domains.

## Approved public sources

- Wayback Machine (web.archive.org)
- archive.today
- National web archives (e.g., UK Web Archive, Bibliotheca Alexandrina)
- Common Crawl index
- Archive.today mirrors

## Source verification standards

Every source is evaluated for authority, proximity to the event or subject, currency, and internal consistency before its content is used analytically. Primary sources are preferred over secondary accounts. Where sources conflict, the conflict is preserved and reported rather than silently resolved. Source reliability is rated on the ANBU reliability scale and recorded in the collection log.

## Analytical framework

Archived pages are point-in-time records. Capture timestamps establish when the archive saw the page, not necessarily when content was published. Changes between snapshots are documented with both timestamps. Archive absence is treated as inconclusive.

## Evidence requirements

Every analytical claim must be traceable to a logged collection item. Evidence requirements: (1) verbatim quotation or precise paraphrase with page/section reference; (2) source attribution including URL or archive identifier; (3) collection timestamp; (4) access method; (5) confidence grade per the ANBU scale. Claims without logged evidence are marked INSUFFICIENT and excluded from analytical products.

## Confidence assessment

HIGH: multiple independent primary sources, direct documentation, no material contradictions. MODERATE: credible sources with minor gaps or single-source primary documentation. LOW: indirect, derivative, or partially corroborated reporting. INSUFFICIENT: evidence does not support a judgment; collection gap or contested sources prevent assessment.

## Common analytical mistakes

- Confusing capture date with publication date
- Treating archive absence as proof of non-existence
- Missing JavaScript-rendered content in archives
- Failing to check multiple archives for coverage

## Ethical considerations

Use archives for research on public pages. Do not use archives to access content that was private when live. Respect archive terms.

## Security boundaries

No circumvention of archive access controls. No use of archives to retrieve private or access-controlled content.

## Expected output

Archive research log with snapshot URLs, timestamps, diff summaries, and change timeline.

## Quality checklist

- [ ] Snapshot timestamps recorded
- [ ] CDX coverage checked
- [ ] Multiple archives consulted
- [ ] Changes documented with dates

## Cross-reference links

- `media_archive_research.md`
- `historical_archive_research.md`
- `source_discovery.md`
- `information_gap_analysis.md`
- `osint_collection_ethics.md`

