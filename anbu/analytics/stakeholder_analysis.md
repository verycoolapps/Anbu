# Stakeholder Analysis

**ANBU Division 008 · Analytics**

---

## Purpose

Stakeholder analysis identifies the actors affected by, able to influence, or invested in a development — and assesses their interests, leverage, and likely behavior. In ANBU it supports everything from policy forecasts to conflict assessment: a decision cannot be understood without knowing who wants what and who can deliver or block it.

## Scope

Applied to policy decisions, institutional reform, electoral processes, conflict dynamics, corporate and regulatory developments, and any question where multiple actors' interests intersect. Covers institutional stakeholders (ministries, agencies, SOEs), political stakeholders (parties, factions, movements), economic stakeholders (firms, unions, investors), and international stakeholders (allies, donors, multilateral bodies).

## Intelligence objectives

- Enumerate stakeholders systematically — including those easily overlooked.
- Assess each stakeholder's interest intensity, leverage, and position.
- Predict coalition formation, defections, and blocking behavior.
- Identify which stakeholders can actually deliver outcomes vs. merely opine.

## Core concepts

- **Stakeholder.** Any actor with a stake in the outcome: affected by it, able to shape it, or bearing costs/benefits.
- **Interest intensity.** How much the outcome matters to the actor — not how loud they are.
- **Leverage.** Formal power (votes, budgets, vetoes) plus informal power (expertise, mobilization, access).
- **Position vs. interest.** Stated positions may mask true interests; stated interests may be post-hoc rationalizations.
- **Veto player.** A stakeholder who can block the outcome regardless of majority support.
- **Swing stakeholder.** A stakeholder whose defection or support changes the outcome.
- **Salience.** Combination of power, legitimacy, and urgency — the classic stakeholder salience model adapted to OSINT.

## Analytical methodology

1. Define the decision or development the analysis serves.
2. Enumerate stakeholders: who is affected, who can influence, who bears costs.
3. For each: interests (what they want), position (stated), leverage (formal + informal), intensity.
4. Map the stakeholder space: allies, opponents, neutrals, swing actors, veto players.
5. Assess likely behavior: who mobilizes, who defects, who bargains, who obstructs.
6. Identify the winning coalition requirements and blocking coalitions.
7. Report with per-stakeholder confidence and evidence for claimed interests.

## Step-by-step workflow

1. Define the outcome or decision in scope.
2. Brainstorm stakeholders; then systematically search for missing categories (affected publics, bureaucratic implementers, external actors).
3. For each stakeholder, collect evidence of interests: votes, statements, budgets, litigation, mobilization.
4. Rate interest intensity and leverage separately — high voice ≠ high leverage.
5. Classify: supporter / opponent / conditional / veto / swing.
6. Model scenarios: minimum winning coalition, likely blocking coalition.
7. Cross-check with `power_structure_analysis.md` for leverage assessment.
8. Write stakeholder annex with evidence per claim.

## Data requirements

- Voting records, committee memberships, public statements.
- Budget and resource allocations revealing priorities.
- Litigation and regulatory filings showing active engagement.
- Membership and mobilization data for civil-society stakeholders.
- Official statements and voting patterns for political stakeholders.
- Market data, employment, and investment flows for economic stakeholders.

## Approved public sources

Parliamentary records and roll-call votes; official statements and manifestos; budget documents; regulatory filings; court records; NGO and civil-society publications; electoral data; business registries and corporate disclosures; trade union and employer organization publications; multilateral organization records.

## Source verification standards

Stakeholder positions must be documented from the stakeholder's own statements or actions, not inferred from ideology. Inferred interests must be labeled as inference with supporting evidence. See `../verification/stakeholder_source_verification.md`.

## Analytical framework

Stakeholder scoring matrix:

| Dimension | Question | Scale |
|---|---|---|
| Interest intensity | How much does outcome matter? | Low–High |
| Leverage | Can they deliver or block? | Low–High |
| Position certainty | How well do we know their stance? | Low–High |
| Mobilization likelihood | Will they act? | Low–High |

Classification rules: veto player = high leverage + opposed; swing = high leverage + uncertain position; noise = high voice + low leverage.

## Evidence requirements

- Every stakeholder's position cites a primary statement or action.
- Leverage claims cite formal authority or documented capability.
- Inferred interests labeled as inference.
- Stakeholder omissions assessed: who is missing and why?

## Confidence assessment

- **HIGH** — stakeholders comprehensively enumerated; positions documented; leverage verifiable.
- **MODERATE** — main stakeholders identified; some positions inferred or fluid.
- **LOW** — stakeholder set incomplete; positions largely speculative.
- **INSUFFICIENT** — cannot enumerate stakeholders reliably; report what is known and gaps.

## Common analytical mistakes

- Confusing loud stakeholders with influential ones.
- Missing quiet veto players (agencies, courts, regulators).
- Treating stated positions as fixed — positions shift with bargaining.
- Ignoring implementation stakeholders (civil servants, local officials).
- Assuming all affected parties are aware of or organized around the issue.
- Forgetting external stakeholders (allies, donors, markets).

## Ethical considerations

Stakeholder analysis must not become a targeting tool against lawful political actors. It describes interests and leverage for understanding outcomes; it must not be used to predict or enable suppression of legitimate dissent.

## Security boundaries

Public statements and records only. No assessment of private individuals' unstated preferences beyond what public behavior documents. No stakeholder maps used for harassment or intimidation.

## Expected output

Stakeholder annex: stakeholder table (interests, position, leverage, evidence), coalition analysis, likely behavior scenarios. Main product summarizes stakeholder dynamics relevant to the question.

## Quality checklist

- [ ] Stakeholder set systematically enumerated, omissions checked.
- [ ] Interests evidenced, not assumed.
- [ ] Leverage separated from voice.
- [ ] Veto and swing actors identified.
- [ ] Positions dated and sourced.
- [ ] Coalition scenarios plausible.

## Cross-reference links

- [`power_structure_analysis.md`](power_structure_analysis.md) — who holds leverage.
- [`institutional_relationship_mapping.md`](institutional_relationship_mapping.md) — formal institutional stakeholders.
- [`influence_network_assessment.md`](influence_network_assessment.md) — informal influence channels.
- [`political_economy_analysis.md`](political_economy_analysis.md) — economic stakeholders.
- [`network_analysis_public_data.md`](network_analysis_public_data.md) — relational structure.
- [`../political/elite_analysis.md`](../political/elite_analysis.md) — political elites.
- [`../reporting/stakeholder_map_template.md`](../reporting/stakeholder_map_template.md) — output format.
