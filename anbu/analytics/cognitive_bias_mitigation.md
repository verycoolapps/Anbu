# Cognitive Bias Mitigation

**ANBU Division 008 · Analytics**

---

## Purpose

Cognitive biases are systematic errors in human judgment that distort intelligence analysis regardless of analyst competence or evidence quality. They operate below awareness, are resistant to goodwill, and must be countered procedurally. This file catalogs the biases most relevant to OSINT analysis, their manifestations, and the specific controls ANBU applies to mitigate them.

## Scope

Applied to all analytical work by every analyst. Bias controls are embedded in procedures (ACH, KAC, red team) but also require individual discipline. This file is both a reference taxonomy and an operational checklist.

## Intelligence objectives

- Make analysts aware of the specific biases that distort their judgment.
- Provide procedural controls that work even when bias operates unconsciously.
- Create a common vocabulary for discussing bias in review.
- Reduce systematic errors that no amount of data quality can fix.

## Core concepts

Biases fall into families:

- **Information-processing biases** — how we select and interpret information.
- **Judgment biases** — how we weigh evidence and estimate likelihood.
- **Social/organizational biases** — how group dynamics and incentives distort analysis.
- **Memory/experience biases** — how past events and training shape current judgment.

## Analytical methodology

Bias mitigation is not a one-time check but a continuous discipline:

1. **Awareness** — know the bias taxonomy (this file).
2. **Procedural controls** — use SATs that externalize reasoning (ACH, KAC, red team).
3. **Deliberate search** — actively seek disconfirming evidence and alternative explanations.
4. **Peer challenge** — externalize reasoning for others to attack.
5. **Calibration** — track forecast accuracy over time to correct systematic over/under-confidence.

## Bias taxonomy and controls

### Anchoring bias
First information received disproportionately influences judgment. A first report's framing persists even after contradictory evidence arrives.
**Control:** Delay hypothesis formation; collect multiple independent sources before drafting; explicitly revisit initial framing.

### Confirmation bias
Seeking, interpreting, and remembering evidence that confirms existing beliefs while discounting disconfirming evidence.
**Control:** ACH matrix forces scoring against all hypotheses; devil's advocacy; red team attack; explicit disconfirming-evidence search.

### Availability bias
Judging likelihood by how easily examples come to mind — recent, vivid, or emotionally salient events seem more probable.
**Control:** Reference class forecasting; base-rate checking; awareness of recency effects.

### Representativeness bias
Judging probability by how well a case matches a stereotype or template, ignoring base rates.
**Control:** Base-rate discipline; reference class selection; statistical reasoning checks.

### Mirror-imaging
Projecting one's own values, logic, and preferences onto the actor being analyzed.
**Control:** Strategic culture analysis; explicit "how would this actor see it?" questioning; cultural/structural context research.

### Overconfidence bias
Excessive certainty in judgments, especially on familiar or emotionally charged topics.
**Control:** Estimative probability language; confidence calibration tracking; forced uncertainty statements; pre-mortem analysis.

### Groupthink
Conformity pressure suppressing dissent within analytical teams.
**Control:** Anonymous initial assessments; devil's advocate role; red team independence; leader speaks last.

### Sunk cost / commitment bias
Persisting with a favored hypothesis because resources have been invested in it.
**Control:** KAC re-testing; explicit "what would make us abandon this?" questions; fresh-eyes review.

### Recency bias
Overweighting recent events relative to older but equally relevant evidence.
**Control:** Full-series trend analysis; historical context requirements; timeline completeness checks.

### Halo/horns effect
One positive (or negative) attribute coloring judgment of unrelated attributes.
**Control:** Separate assessment dimensions; evidence-based evaluation per dimension; awareness of source reputation effects.

### Fundamental attribution error
Attributing others' behavior to disposition while excusing one's own side's behavior by situation.
**Control:** Structural/incentive analysis before intent attribution; symmetric analysis standards.

### Survivorship bias
Analyzing only visible successes while ignoring failures that left no trace.
**Control:** Explicit search for failed/comparable cases; reference class completeness.

## Step-by-step workflow

1. Before analysis: review this taxonomy; identify which biases are most likely given the topic and analyst background.
2. During analysis: apply procedural controls (ACH, KAC, alternatives).
3. Before finalizing: run the bias checklist below.
4. In review: red team applies the bias attack category.
5. Post-product: track forecast accuracy for calibration.

## Data requirements

- Awareness of analyst's own potential biases (self-assessment).
- Team composition that diversifies perspectives.
- Access to disconfirming evidence sources.
- Historical forecast record for calibration.

## Approved public sources

N/A — this is a methodological control file. Applies to all source use.

## Source verification standards

Bias mitigation does not replace source verification; it operates on verified evidence. However, bias awareness should extend to source selection: are we seeking sources that confirm or challenge?

## Analytical framework

Pre-submission bias checklist:

| Bias | Question |
|---|---|
| Anchoring | Did first reports disproportionately shape the analysis? |
| Confirmation | Did we actively seek disconfirming evidence? |
| Availability | Are we over-weighting recent/vivid events? |
| Mirror-imaging | Did we assume the actor thinks like us? |
| Overconfidence | Does confidence match evidence quality? |
| Groupthink | Did dissent get heard? |
| Sunk cost | Are we persisting due to invested effort? |
| Recency | Is the full historical context included? |
| Halo/horns | Did one attribute color overall judgment? |
| Attribution | Are we blaming disposition over situation? |
| Survivorship | Did we consider failures/invisible cases? |

## Evidence requirements

- Disconfirming evidence search documented.
- Alternative explanations generated and evaluated.
- Confidence statement reflects genuine uncertainty.
- Red team or devil's advocacy completed for high-stakes products.
- Forecast accuracy tracked where predictions made.

## Confidence assessment

Bias mitigation affects achievable confidence:

- Effective controls + clean review → confidence can be HIGH if evidence supports.
- Weak controls or identified bias concerns → cap at MODERATE.
- Significant unaddressed bias concerns → downgrade to LOW.
- Bias so pervasive that judgment cannot be trusted → INSUFFICIENT, restart with fresh analyst.

## Common analytical mistakes

- Believing bias awareness alone prevents bias (it doesn't — procedures do).
- Treating bias as an individual failing rather than a systematic feature.
- Applying controls ceremonially without genuine engagement.
- Forgetting organizational/incentive biases (pressure for certain conclusions).
- Assuming technical analysts are immune to cognitive biases.
- Not tracking forecast accuracy, so calibration never improves.

## Ethical considerations

Analysts must disclose known biases that could affect their work. Products must not be shaped by political preference, institutional loyalty, or desire to please consumers. The red team process must be protected from pressure to produce preferred findings.

## Security boundaries

Bias controls are internal quality procedures. No additional collection authorized. All boundaries from `../security/` apply.

## Expected output

Bias checklist completed for each product. Review memo notes bias concerns found and addressed. Forecast accuracy tracked for calibration improvement.

## Quality checklist

- [ ] Bias taxonomy reviewed before analysis.
- [ ] Procedural controls applied (ACH, KAC, alternatives).
- [ ] Disconfirming evidence actively sought.
- [ ] Pre-submission bias checklist completed.
- [ ] Red team applied for high-stakes products.
- [ ] Confidence calibrated to evidence, not preference.
- [ ] Forecast accuracy tracked.

## Cross-reference links

- [`red_team_analytical_review.md`](red_team_analytical_review.md) — bias attack in review.
- [`alternative_explanations.md`](alternative_explanations.md) — countering confirmation bias.
- [`key_assumptions_check.md`](key_assumptions_check.md) — countering sunk cost.
- [`analytical_confidence_language.md`](analytical_confidence_language.md) — calibration.
- [`analytical_reasoning.md`](analytical_reasoning.md) — reasoning foundation.
- [`../core/analytical_standards.md`](../core/analytical_standards.md) — doctrine.
- [`../reporting/assessment_template.md`](../reporting/assessment_template.md) — uncertainty communication.
