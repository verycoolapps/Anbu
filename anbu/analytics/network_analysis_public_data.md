# Network Analysis of Public Data

**ANBU Division 008 · Analytics**

---

## Purpose

Network analysis maps relationships among actors, institutions, and entities using public data — who funds whom, who appoints whom, who contracts with whom, who shares board seats, who co-signs, who appears together. This file defines how ANBU constructs and interprets relationship networks from open sources, what the resulting maps can and cannot support, and the standards that keep network claims honest.

## Scope

Applied to institutional networks (agencies, ministries, state enterprises), political networks (parties, factions, elites), corporate networks (ownership, procurement), and civil-society networks (NGOs, media ownership). Individual-level private relationship mapping is out of scope.

## Intelligence objectives

- Reveal structure invisible in linear reporting: hubs, brokers, clusters, isolates.
- Identify influence channels, dependency relationships, and potential conflict-of-interest structures.
- Track network change over time: new ties, severed ties, shifting centers.
- Provide the relational layer for `institutional_relationship_mapping.md` and `power_structure_analysis.md`.

## Core concepts

- **Node.** An entity: institution, office, company, party, person in an official capacity.
- **Edge.** A documented relationship: appointment, ownership, contract, co-membership, statement of support, family relation where publicly disclosed in official context.
- **Tie strength.** Frequency, recency, and formal vs. informal character of the relationship.
- **Centrality.** Degree (number of ties), betweenness (broker position), eigenvector (connected to well-connected actors). Each answers a different question.
- **Cluster/community.** Dense sub-groups; often factions, ministries, or interest blocs.
- **Broker.** A node connecting otherwise separate clusters — often the most analytically interesting position.
- **Boundary specification.** Which nodes and ties are included defines what the network means; state it explicitly.

## Analytical methodology

1. Define the network's boundary: which actors, which relationship types, which period.
2. Enumerate nodes from authoritative public sources (registers, filings, official biographies).
3. Enumerate edges only from documented public relationships — never inferred intimacy.
4. Weight ties by strength and recency.
5. Compute descriptive metrics: degree, centrality, clustering, components.
6. Interpret structure: identify hubs, brokers, clusters, isolates, and structural holes.
7. Validate: are surprising ties real? Are missing ties actually missing or just unobserved?
8. Report with boundary specification, data completeness caveats, and confidence.

## Step-by-step workflow

1. Receive the network question (e.g., "map procurement ties between ministry X and suppliers").
2. Define boundary: node types, edge types, time window.
3. Build the node list from official registers; assign canonical identifiers.
4. Build the edge list: each edge cites its public source (filing, gazette, official bio).
5. Compute metrics using consistent definitions; document method.
6. Identify structural findings: central actors, brokers, clusters, isolates.
7. Cross-check edges for currency (is the relationship current?) and completeness (are known ties missing?).
8. Produce the network annex: node/edge tables, metrics, structural interpretation, caveats.

## Data requirements

- Official registers: company registries, procurement portals, gazettes, official appointment announcements.
- Corporate filings: ownership, directors, subsidiaries, related-party disclosures.
- Parliamentary records: voting alignments, committee memberships, questions tabled.
- Official biographies and organizational charts.
- Date-stamped evidence for every edge — undated relationships cannot establish network state.

## Approved public sources

National company registries and beneficial-ownership registers where public; government procurement portals; parliamentary open-data portals; official gazettes; central bank and securities filings; court records of corporate relationships; official organizational publications; reputable investigative reporting as leads requiring register confirmation.

## Source verification standards

Every edge requires a documentary basis. Register entries outrank journalism; journalism outranks inference. Relationships asserted only by allegation or single-source reporting are included only as flagged, low-confidence edges or excluded. See `../verification/institutional_source_verification.md`.

## Analytical framework

Interpretation guide:

| Metric | What it suggests | Caveat |
|---|---|---|
| High degree | Well-connected actor | May be ceremonial, not influential |
| High betweenness | Broker/gatekeeper | Position may be structurally forced |
| Dense cluster | Faction or aligned bloc | May reflect shared mandate, not collusion |
| Isolate | Peripheral or excluded actor | May have unobserved ties |
| Structural hole | Gap an actor could bridge | Requires judgment about access |

## Evidence requirements

- Node list cites authoritative source per node.
- Edge list cites documentary basis per edge with date.
- Metrics computed with stated method; raw tables annexed.
- Missing-data assessment: which expected ties could not be observed and why.

## Confidence assessment

- **HIGH** — comprehensive register data, all edges documented, metrics robust.
- **MODERATE** — good node coverage; some edges inferred or single-sourced.
- **LOW** — sparse data, many flagged edges, boundary uncertain.
- **INSUFFICIENT** — no reliable public registers; only impressionistic relationships; do not map, report the gap.

## Common analytical mistakes

- Treating co-appearance as relationship (same conference ≠ tie).
- Confusing formal mandate with informal influence.
- Ignoring boundary specification — the map shows only what was included.
- Reading centrality as power without checking whether ties are active.
- Missing ties are invisible: absence in the map is not absence in reality.
- Over-interpreting sparse networks where metrics are unstable.

## Ethical considerations

Network maps of public officials and institutions serve accountability; maps of private individuals' relationships veer toward doxxing and are out of scope unless the individuals act in official capacity and the relationship is officially documented. No network product may enable harassment.

## Security boundaries

Public registers and filings only. No use of leaked databases, breach data, or non-public corporate information. No mapping of private citizens' associations. No relationship claims based on surveillance or intercepted material.

## Expected output

Network annex: boundary statement, node/edge tables with citations, metrics summary, structural interpretation, completeness caveats. Main product draws only the conclusions the network supports.

## Quality checklist

- [ ] Boundary (nodes, edges, period) explicitly stated.
- [ ] Every edge has a documentary public source with date.
- [ ] Metrics method documented.
- [ ] Missing-data assessment included.
- [ ] Interpretation separated from measurement.
- [ ] Confidence reflects register coverage.

## Cross-reference links

- [`institutional_relationship_mapping.md`](institutional_relationship_mapping.md) — formal institutional ties.
- [`power_structure_analysis.md`](power_structure_analysis.md) — who the network empowers.
- [`stakeholder_analysis.md`](stakeholder_analysis.md) — actors within networks.
- [`influence_network_assessment.md`](influence_network_assessment.md) — influence vs. formal ties.
- [`political_economy_analysis.md`](political_economy_analysis.md) — economic networks.
- [`analytical_reasoning.md`](analytical_reasoning.md) — reasoning foundation.
- [`../verification/institutional_source_verification.md`](../verification/institutional_source_verification.md) — edge standards.
- [`../geopolitical/alliance_network_analysis.md`](../geopolitical/alliance_network_analysis.md) — interstate application.
- [`../reporting/network_map_template.md`](../reporting/network_map_template.md) — output format.
