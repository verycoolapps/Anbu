# Official Statement Collection

> ANBU OSINT Division 002 — Collection Tradecraft

## Purpose

Defines procedures for collecting official statements: government press statements, ministry releases, agency announcements, and executive communications.

## Scope

Statements from heads of state, ministries, agencies, regulators, and official spokespeople, across national and international levels.

## Intelligence objectives

- Capture official positions verbatim for later speech analysis
- Track policy announcements and their precise wording
- Detect changes in official language that signal policy shifts
- Build a timestamped corpus of official statements

## Core concepts

- Statement classes: press release, readout, communiqué, briefing note, social post by official account
- Verbatim capture versus paraphrase
- Spokesperson versus principal attribution
- Statement lifecycle: announcement, clarification, withdrawal

## Analytical methodology

Monitor official portals and verified official accounts. Capture full text, not excerpts; record publication timestamp, issuing body, and URL. Archive the exact page at capture time. Flag statements later amended or deleted. Classify by issuing authority level and subject matter.

## Step-by-step workflow

1. Identify official sources per jurisdiction and agency
2. Set monitoring for new publications
3. Capture full text with timestamp and URL
4. Archive page snapshot where permitted
5. Log in collection log with statement classification
6. Flag contradictions or updates for analysis

## Data requirements

Target governments/agencies; period; subject areas; languages; known spokesperson names and official account handles.

## Approved public sources

- Government press offices and ministry websites
- Agency and regulator newsrooms
- Official social media accounts of institutions
- Multilateral organization press rooms (UN, NATO, EU)
- Official readouts of diplomatic meetings

## Source verification standards

Every source is evaluated for authority, proximity to the event or subject, currency, and internal consistency before its content is used analytically. Primary sources are preferred over secondary accounts. Where sources conflict, the conflict is preserved and reported rather than silently resolved. Source reliability is rated on the ANBU reliability scale and recorded in the collection log.

## Analytical framework

Statements are evidence of official position at a point in time. Analysis compares wording across statements to detect shifts. Attribution follows the issuing body; spokesperson statements are labeled as such. Deletions and corrections are treated as findings.

## Evidence requirements

Every analytical claim must be traceable to a logged collection item. Evidence requirements: (1) verbatim quotation or precise paraphrase with page/section reference; (2) source attribution including URL or archive identifier; (3) collection timestamp; (4) access method; (5) confidence grade per the ANBU scale. Claims without logged evidence are marked INSUFFICIENT and excluded from analytical products.

## Confidence assessment

HIGH: multiple independent primary sources, direct documentation, no material contradictions. MODERATE: credible sources with minor gaps or single-source primary documentation. LOW: indirect, derivative, or partially corroborated reporting. INSUFFICIENT: evidence does not support a judgment; collection gap or contested sources prevent assessment.

## Common analytical mistakes

- Quoting paraphrased media coverage instead of official text
- Missing corrections or deleted statements
- Treating a spokesperson's remark as principal policy without confirmation
- Failing to capture non-English originals

## Ethical considerations

Collect statements from official public channels. Do not impersonate officials or use private communications. Respect platform terms for official account monitoring.

## Security boundaries

No fake accounts, no social engineering of press offices, no access to non-public briefings.

## Expected output

Timestamped statement corpus with verbatim text, attribution, classification, and change flags.

## Quality checklist

- [ ] Verbatim text captured
- [ ] Timestamp and URL recorded
- [ ] Attribution classified
- [ ] Corrections/deletions flagged

## Cross-reference links

- `public_press_release_collection.md`
- `parliamentary_document_research.md`
- `public_speech_analysis.md`
- `news_media_monitoring.md`
- `public_social_media_research.md`

