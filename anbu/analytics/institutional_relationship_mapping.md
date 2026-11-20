# Institutional Relationship Mapping

**ANBU Division 008 · Analytics**

---

## Purpose

Institutions relate to one another through formal mandates, budget flows, legal authorities, reporting lines, and informal coordination. Institutional relationship mapping documents these structured ties — who controls whom, who funds whom, who must consult whom — to reveal where real power and real dependence sit inside a state or organization. This complements `network_analysis_public_data.md` by focusing on formal institutional architecture rather than emergent network metrics.

## Scope

Applied to government ministries, agencies, state-owned enterprises, judiciaries, militaries, central banks, and international bodies. Focuses on formally documented relationships: statutes, org charts, budget documents, inter-agency agreements, reporting obligations.

## Intelligence objectives

- Map the formal architecture of decision-making and resource flows.
- Identify overlapping mandates, jurisdictional conflicts, and coordination bottlenecks.
- Locate the institutions that actually control budgets, appointments, and enforcement.
- Track institutional change: mergers, splits, mandate expansions, capture.

## Core concepts

- **Principal-agent chain.** Who delegates authority to whom; where accountability thins.
- **Mandate overlap.** Two institutions claiming the same function — a classic source of friction or capture.
- **Budget dependence.** An institution's autonomy is constrained by who controls its funding.
- **Gatekeeping.** Institutions positioned to block or enable others' actions (licensing, review, veto points).
- **Informal coordination.** Working groups, memoranda, secondments — often where real decisions happen.
- **Institutional capture.** When an institution's formal mandate is subordinated to the interests of the actor it should regulate.

## Analytical methodology

1. Enumerate the institutions in scope and their legal mandates.
2. Document formal relationships: reporting lines, budget flows, consultation requirements, legal appeals.
3. Identify overlap and conflict zones.
4. Locate gatekeeping and veto points.
5. Assess informal coordination mechanisms visible in public documents (joint communiqués, MOUs, working groups).
6. Interpret the map: where does effective power concentrate?
7. Track recent institutional changes and their drivers.

## Step-by-step workflow

1. Define scope: which institutions, which level of government, which period.
2. Pull legal mandates from statutes, organic laws, official charters.
3. Extract org charts and reporting lines from official publications.
4. Map budget flows from budget laws and appropriation documents.
5. Identify consultation/approval requirements from procedural law.
6. Note informal mechanisms from official announcements and public records.
7. Build the relationship table: institution pair | relationship type | legal basis | direction of dependence.
8. Interpret: power concentration, friction points, capture indicators.
9. Cross-check with `power_structure_analysis.md` for informal power.

## Data requirements

- Organic laws, statutes, and government organization regulations.
- Official organizational charts and leadership directories.
- Budget laws and appropriation schedules.
- Official gazette notices of appointments, delegations, MOUs.
- Parliamentary oversight records where available.
- Official statements describing coordination mechanisms.

## Approved public sources

National gazettes and statute databases; ministry websites and organizational publications; official budget portals; parliamentary records; audit institution reports; central bank publications; international organization mandate documents; government organizational directories.

## Source verification standards

Formal relationships must be grounded in legal or official documents. Informal relationships require at least two independent public indicators (e.g., joint appearance plus documented working relationship). Single-source claims of influence are flagged.

## Analytical framework

Relationship types catalog:

| Type | Examples | Analytical significance |
|---|---|---|
| Hierarchical | Minister → agency | Command and control |
| Fiscal | Treasury → ministry | Resource dependence |
| Legal | Statute → agency | Mandate and constraint |
| Consultative | Agency ↔ agency | Coordination, veto potential |
| Informal | Working group, MOU | Where decisions may actually occur |
| Oversight | Parliament/audit → agency | Accountability channel |

## Evidence requirements

- Each relationship cites its documentary basis (statute section, budget line, official announcement).
- Relationship currency noted — is it current law/practice?
- Informal relationships flagged as such with their evidence type.
- Institutional changes dated.

## Confidence assessment

- **HIGH** — relationships documented in current legal/official sources; structure unambiguous.
- **MODERATE** — formal structure clear; informal layer partially observed.
- **LOW** — patchy documentation; key relationships inferred from indirect evidence.
- **INSUFFICIENT** — no reliable public documentation of institutional relationships; report the gap.

## Common analytical mistakes

- Assuming org charts reflect real power (they show formal authority, not influence).
- Ignoring informal coordination where decisions actually happen.
- Missing mandate overlap because each institution is analyzed in isolation.
- Treating budget dependence as the only constraint — legal and political dependence matter too.
- Confusing coordination mechanisms with power relationships.
- Outdated charts used as current reality.

## Ethical considerations

Institutional mapping is legitimate accountability analysis. Maps must not be used to identify individuals for targeting; they describe structures and offices, not persons' private lives.

## Security boundaries

Public legal and official documents only. No speculation about classified mandates or covert relationships presented as fact. No mapping of private organizations beyond publicly documented institutional roles.

## Expected output

Institutional map annex: node/edge tables by relationship type, overlap and gatekeeping analysis, power-concentration assessment, change log. Main product draws structural conclusions relevant to the question.

## Quality checklist

- [ ] Mandates sourced from law, not description.
- [ ] Budget and reporting flows documented.
- [ ] Overlaps and veto points identified.
- [ ] Informal layer flagged and evidenced.
- [ ] Currency of relationships verified.
- [ ] Formal vs. informal distinction maintained.

## Cross-reference links

- [`network_analysis_public_data.md`](network_analysis_public_data.md) — network metrics complement formal maps.
- [`power_structure_analysis.md`](power_structure_analysis.md) — informal power layer.
- [`stakeholder_analysis.md`](stakeholder_analysis.md) — actors within institutions.
- [`political_economy_analysis.md`](political_economy_analysis.md) — fiscal relationships.
- [`state/state_capacity_assessment.md`](../state/state_capacity_assessment.md) — capacity implications.
- [`../verification/institutional_source_verification.md`](../verification/institutional_source_verification.md) — documentary standards.
- [`../reporting/network_map_template.md`](../reporting/network_map_template.md) — output format.
