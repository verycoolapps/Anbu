# Parliamentary Document Research

> ANBU OSINT Division 002 — Collection Tradecraft

## Purpose

Defines methods for researching parliamentary and legislative documents: bills, debates, committee reports, voting records, and official proceedings.

## Scope

National parliaments, supranational legislatures (European Parliament), and committee systems, using official parliamentary websites, document repositories, and gazettes.

## Intelligence objectives

- Track legislative activity on topics of analytical interest
- Attribute statements and votes to specific legislators
- Retrieve committee reports and evidence sessions
- Document legislative timelines and procedural status

## Core concepts

- Legislative lifecycle: bill, committee, readings, vote, enactment
- Hansard and official debate records
- Committee evidence and witness testimony
- Voting record granularity (voice vote vs recorded division)

## Analytical methodology

Locate the official parliamentary portal and document repository. Search by topic, sponsor, committee, and date. Prefer official XML/PDF APIs where available (e.g., TheyWorkForYou mirrors official data). Record document identifiers, sitting dates, and speaker attributions. Distinguish government statements from backbench remarks.

## Step-by-step workflow

1. Identify relevant parliament(s) and committees
2. Search bill databases and debate archives by keyword and sponsor
3. Retrieve committee reports and evidence transcripts
4. Extract voting records for key divisions
5. Record document IDs and dates in collection log
6. Correlate with official_statement_collection.md and news coverage

## Data requirements

Topic keywords; legislator names; committee names; date range; jurisdictions; language requirements.

## Approved public sources

- Official parliamentary portals and document repositories
- Hansard and official debate records
- Committee evidence archives
- Official voting record databases
- Legislative gazettes and statute databases

## Source verification standards

Every source is evaluated for authority, proximity to the event or subject, currency, and internal consistency before its content is used analytically. Primary sources are preferred over secondary accounts. Where sources conflict, the conflict is preserved and reported rather than silently resolved. Source reliability is rated on the ANBU reliability scale and recorded in the collection log.

## Analytical framework

Parliamentary records are primary sources for what was said in the chamber. Attribution is precise: speaker, date, sitting, and document section are recorded. Government and opposition statements are labeled by affiliation. Transcripts are checked against official records, not media paraphrases.

## Evidence requirements

Every analytical claim must be traceable to a logged collection item. Evidence requirements: (1) verbatim quotation or precise paraphrase with page/section reference; (2) source attribution including URL or archive identifier; (3) collection timestamp; (4) access method; (5) confidence grade per the ANBU scale. Claims without logged evidence are marked INSUFFICIENT and excluded from analytical products.

## Confidence assessment

HIGH: multiple independent primary sources, direct documentation, no material contradictions. MODERATE: credible sources with minor gaps or single-source primary documentation. LOW: indirect, derivative, or partially corroborated reporting. INSUFFICIENT: evidence does not support a judgment; collection gap or contested sources prevent assessment.

## Common analytical mistakes

- Relying on media summaries instead of official transcripts
- Ignoring committee stage where substantive scrutiny occurs
- Failing to distinguish proposed bills from enacted law
- Missing multilingual parliamentary sources for non-English legislatures

## Ethical considerations

Parliamentary proceedings are public records; research focuses on legislative activity, not personal surveillance of members beyond their official acts.

## Security boundaries

No scraping that degrades parliamentary systems. Use official bulk data and APIs where provided.

## Expected output

Legislative activity tables: bills, debates, committee reports, votes, with document citations and speaker attribution.

## Quality checklist

- [ ] Official document IDs cited
- [ ] Speaker and date attribution recorded
- [ ] Committee stage documented
- [ ] Enacted vs proposed status distinguished

## Cross-reference links

- `official_statement_collection.md`
- `government_open_data.md`
- `public_speech_analysis.md`
- `news_media_monitoring.md`
- `source_collection_log.md`

