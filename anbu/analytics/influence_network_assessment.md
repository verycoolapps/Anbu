# Influence Network Assessment

**ANBU Division 008 · Analytics**

---

## Purpose

Influence is the capacity to shape decisions without formal authority. Formal power maps show who may decide; influence networks show who actually moves decisions — through access, information control, financial leverage, expertise monopolies, or social capital. This file defines how ANBU assesses influence channels using public evidence, distinguishing documented influence from mere proximity or reputation.

## Scope

Applied to policy processes, regulatory capture assessment, lobbying and advocacy mapping, media influence, expert advisory networks, and any context where outcomes diverge from formal authority. Covers institutional influence (who advises whom), economic influence (who funds advocacy), and informational influence (who shapes the agenda).

## Intelligence objectives

- Identify who actually shapes decisions beyond formal decision-makers.
- Map influence channels: advisory access, funding flows, revolving doors, information bottlenecks.
- Assess whether influence is transparent (registered lobbying) or opaque (undocumented access).
- Evaluate influence concentration: pluralistic vs. captured policy processes.

## Core concepts

- **Influence channel.** The pathway through which influence operates: advisory committee, campaign finance, revolving door, expert monopoly, media agenda-setting, personal access.
- **Revolving door.** Movement of personnel between regulator and regulated; creates both expertise and capture risk.
- **Agenda-setting influence.** Shaping what gets discussed at all — often more powerful than shaping outcomes within discussion.
- **Inside vs. outside influence.** Institutional insiders (officials, staff) vs. external actors (lobbyists, NGOs, media, experts).
- **Influence vs. access.** Access is opportunity; influence is demonstrated effect. Proximity is not proof.
- **Transparency gradient.** Registered lobbying < disclosed donations < documented meetings < observed outcomes. Lower transparency demands stronger inference discipline.

## Analytical methodology

1. Identify the decision process and its formal decision points.
2. Map who participates at each point: formal participants + advisory inputs.
3. Identify influence channels: funding, appointments, expertise, access, information.
4. Gather evidence of influence: documented meetings, funding records, appointment patterns, outcome alignment.
5. Distinguish demonstrated influence (evidence of effect) from potential influence (access + interest).
6. Assess concentration: is influence pluralistic or dominated by few actors?
7. Report with evidence grading per channel.

## Step-by-step workflow

1. Define the policy or decision process in scope.
2. Map formal participants and decision points via `institutional_relationship_mapping.md`.
3. Identify advisory bodies, expert panels, working groups — the influence surface.
4. Collect funding data: campaign finance, lobbying registries, think-tank funders, procurement awards.
5. Track revolving doors: career histories of officials and regulators (public bios).
6. Examine agenda-setting: who frames the issue in media and official discourse.
7. For each channel, grade evidence: demonstrated / probable / possible influence.
8. Write influence assessment: channels mapped, evidence per channel, concentration assessment, confidence.

## Data requirements

- Lobbying registries and disclosure filings where they exist.
- Campaign finance and political donation records.
- Official biographies and career histories (revolving-door analysis).
- Advisory committee membership lists and minutes where public.
- Procurement and grant records showing resource flows.
- Media ownership and agenda-setting data.
- Outcome data: decisions, regulations, budgets for alignment analysis.

## Approved public sources

Lobbying registries (where mandated); electoral finance authorities; official committee and advisory body rosters; procurement portals; corporate ownership filings; media ownership registries; think-tank and NGO annual reports disclosing funders; official meeting calendars and transparency portals; court cases revealing influence.

## Source verification standards

Influence claims require evidence of effect, not just access. "X met with Y" is access; "X's preferred outcome resulted after Y's documented intervention" is influence. Single-source allegations of capture are flagged LOW. See `../verification/institutional_source_verification.md`.

## Analytical framework

Influence evidence hierarchy:

| Level | Evidence type | Confidence |
|---|---|---|
| Demonstrated | Documented intervention + aligned outcome + mechanism | HIGH |
| Probable | Access + funding + consistent outcome alignment | MODERATE |
| Possible | Access + interest + plausible mechanism | LOW |
| Access only | Documented meetings without outcome evidence | — (not influence) |

## Evidence requirements

- Each influence claim cites the channel and evidence type.
- Demonstrated influence requires outcome alignment evidence.
- Access-only relationships reported separately from influence claims.
- Transparency gaps disclosed: what influence channels are invisible in public data?

## Confidence assessment

- **HIGH** — multiple channels with demonstrated influence; outcomes align with documented interventions.
- **MODERATE** — probable influence via documented access and funding; outcomes consistent.
- **LOW** — possible influence; evidence suggests access and interest but not effect.
- **INSUFFICIENT** — no public visibility into influence channels; report observability gap.

## Common analytical mistakes

- Confusing access with influence.
- Inferring corruption from proximity alone.
- Ignoring transparent, legal influence (registered lobbying is still influence).
- Missing agenda-setting influence because it precedes formal decision points.
- Assuming influence flows only from outside; insiders capture too.
- Treating all influence as illegitimate — some is lawful and disclosed.

## Ethical considerations

Influence mapping serves accountability: identifying capture, conflicts of interest, and opaque power. It must not be used to attack lawful advocacy, whistleblowing, or civil-society participation. Balance: map all influence channels, not just those of disliked actors.

## Security boundaries

Public registries, filings, and documented meetings only. No claims about secret influence, covert payments, or private dealings without public evidence. No mapping of private individuals' influence beyond their public roles.

## Expected output

Influence annex: channel map, evidence per channel (demonstrated/probable/possible), concentration assessment, transparency-gap statement. Main product draws conclusions about policy integrity and likely outcomes.

## Quality checklist

- [ ] Formal decision points mapped first.
- [ ] All influence channels considered (funding, access, expertise, agenda).
- [ ] Access vs. influence distinguished rigorously.
- [ ] Evidence graded per channel.
- [ ] Transparency gaps disclosed.
- [ ] Lawful and unlawful influence both mapped.

## Cross-reference links

- [`power_structure_analysis.md`](power_structure_analysis.md) — formal vs. informal power.
- [`institutional_relationship_mapping.md`](institutional_relationship_mapping.md) — formal structure.
- [`network_analysis_public_data.md`](network_analysis_public_data.md) — relational metrics.
- [`stakeholder_analysis.md`](stakeholder_analysis.md) — who influences.
- [`political_economy_analysis.md`](political_economy_analysis.md) — financial influence.
- [`../political/elite_analysis.md`](../political/elite_analysis.md) — elite networks.
- [`../legal/lobbying_regulation_analysis.md`](../legal/lobbying_regulation_analysis.md) — regulatory context.
- [`../reporting/assessment_template.md`](../reporting/assessment_template.md) — output format.
