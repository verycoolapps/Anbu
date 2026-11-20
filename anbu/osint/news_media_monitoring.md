# News Media Monitoring

> ANBU OSINT Division 002 — Collection Tradecraft

## Purpose

Defines systematic monitoring of news media: wires, broadcasters, online outlets, and their publication patterns.

## Scope

National and international news organizations, wires, broadcast transcripts, and online news platforms, across languages.

## Intelligence objectives

- Detect breaking developments relevant to requirements
- Track how events are framed across outlets and regions
- Identify media ecosystems and ownership patterns
- Archive reports that are later corrected or removed

## Core concepts

- Media tiers: wires, national broadcasters, regional, partisan, social-first
- Framing and agenda-setting
- Correction and clarification patterns
- Geographic and linguistic media ecosystems

## Analytical methodology

Build outlet lists by tier and region. Monitor homepages, RSS, and wire feeds. For broadcast, use official transcripts and caption services. Archive articles at capture time. Tag by outlet, region, language, and framing. Compare coverage of the same event across outlets.

## Step-by-step workflow

1. Define outlet universe by tier, region, language
2. Set monitoring via RSS, wires, and homepage checks
3. Capture articles with timestamps and outlet attribution
4. Archive snapshots
5. Classify framing and tag entities
6. Flag corrections, removals, and divergent accounts

## Data requirements

Target regions and topics; languages; outlet tiers; time window; broadcast vs online requirements.

## Approved public sources

- Wire services (AP, Reuters, AFP, regional wires)
- National broadcasters and their transcript services
- Major online outlets
- Regional and local media
- Partisan and advocacy outlets (labeled as such)
- Media ownership and circulation data

## Source verification standards

Every source is evaluated for authority, proximity to the event or subject, currency, and internal consistency before its content is used analytically. Primary sources are preferred over secondary accounts. Where sources conflict, the conflict is preserved and reported rather than silently resolved. Source reliability is rated on the ANBU reliability scale and recorded in the collection log.

## Analytical framework

News is treated as reporting, not fact: each item is graded by outlet reliability, proximity to event, and corroboration. Framing differences across outlets are preserved. Outlet ownership and funding are recorded as context for bias assessment.

## Evidence requirements

Every analytical claim must be traceable to a logged collection item. Evidence requirements: (1) verbatim quotation or precise paraphrase with page/section reference; (2) source attribution including URL or archive identifier; (3) collection timestamp; (4) access method; (5) confidence grade per the ANBU scale. Claims without logged evidence are marked INSUFFICIENT and excluded from analytical products.

## Confidence assessment

HIGH: multiple independent primary sources, direct documentation, no material contradictions. MODERATE: credible sources with minor gaps or single-source primary documentation. LOW: indirect, derivative, or partially corroborated reporting. INSUFFICIENT: evidence does not support a judgment; collection gap or contested sources prevent assessment.

## Common analytical mistakes

- Treating a single outlet's account as confirmed
- Ignoring regional-language coverage
- Failing to archive before articles change
- Missing corrections and follow-up reporting

## Ethical considerations

Monitor public news output only. Do not contact journalists deceptively or interfere with reporting.

## Security boundaries

No paywall bypass, no credential sharing, no harassment of journalists or sources.

## Expected output

Monitoring logs with timestamped articles, outlet attribution, framing tags, and divergence flags.

## Quality checklist

- [ ] Outlets classified by tier
- [ ] Articles archived at capture
- [ ] Corrections tracked
- [ ] Framing differences preserved

## Cross-reference links

- `media_archive_research.md`
- `official_statement_collection.md`
- `public_press_release_collection.md`
- `advanced_search_operators.md`
- `verification/`

