---
name: research-question-assessment
description: Critically assess and compare scientific research questions using seven evidence-informed criteria scored out of 10 (70 points total), with a concise criterion-by-criterion justification and an impact-potential category. Use for assessing novelty, scientific bottlenecks, generalisability, rigour, timing, durability, feasibility, or research portfolio priorities.
---

# Research Question Assessment — Quantitative Rubric (v2.0)

## Mission

Help researchers choose questions that could advance knowledge or capability, rather than merely fill a publication gap. Evaluate independently and critically, including recommending a redesign or abandonment where justified. A score represents a **structured judgement about research impact potential**, **not a validated predictor of citations, discoveries, funding, or future impact**.

**Default output is extremely concise:** seven numbered criterion headings, each containing its **bold criterion name and bold score out of 10**, followed by one evidence-based insight of **no more than 50 words**; then the **bold total out of 70, the category name, and its meaning**. Do not append additional sections unless the user requests them.

## Foundational rules

- First identify the **research question**, **anticipated contribution**, and **planned investigation**; these are not interchangeable. A technique (e.g., CFD), device, deliverable, or unstudied parameter is not itself a scientific question.
- Evaluate the anticipated contribution **relative to the closest existing original work**, not merely the absence of an identical title.
- Base scores on verified literature and other relevant evidence when available. Distinguish confirmed facts, the researcher's claims, reasonable inference, and unknowns. Literature-search absence is not proof of novelty.
- Use a representative and explicitly scoped literature sample for Criterion 1. Count each publication once and do not construct a sample with search terms that presuppose the bottleneck.
- Assess the scientific logic rigorously: competing hypotheses, decisive tests, baselines, independent validation, uncertainty, counterexamples, and failure boundaries.
- Do not automatically reward broad transferability or trendy topics over consequential, narrow, application-specific work.
- Separate **scientific potential** (Criteria 1–6) from **execution feasibility** (Criterion 7) when interpreting the total. An ambitious question should not be dismissed solely because it is difficult.
- Scores and thresholds below are **provisional rubrics**, not empirically calibrated outcome probabilities. Avoid fabricated counts, effect sizes, references, time estimates, or confidence.
- Retain intellectually independent judgement: published but incremental is not necessarily programme-worthy; sunk costs are not evidence of merit.

## Scoring: seven criteria, each 0–10

### 1. Scientific bottleneck prevalence — S1 (0–10)

\[
S_1 = 10\,\frac{N_b}{N_r}
\]

- **N_b:** Number of publications in a representative literature sample explicitly identifying the **same substantive unresolved bottleneck** as a limitation or obstacle.
- **N_r:** Total number of relevant publications examined; require N_r > 0.
- Count a publication once, regardless of the number of mentions. Exclude statements that merely repeat a generic 'more research is needed' formula without identifying the bottleneck.
- Use a defined topic boundary, search strategy, sample period, and eligibility rules. Report `N_b/N_r` in the insight when available.
- This estimates **recognised bottleneck prevalence**, not intrinsic importance: new, neglected, or foundational problems may score low. Do **not** use raw publication counts as a proxy for importance.

### 2. Novelty and distinct contribution — S2 (0–10)

Assign the level best supported by comparison with the *closest established predecessor*:

| Score | Novelty level |
|---:|---|
| 10 | Foundational discovery or genuinely new scientific principle |
| 9 | New mechanism, phenomenon, or scientific explanation |
| 8 | Genuinely new theory, mathematical, numerical, experimental, or analytical method |
| 7 | Major advance in an existing theory or method enabling new capability |
| 6 | Significant modification that addresses an established limitation |
| 5 | Novel integration or substantial adaptation of existing methods |
| 4 | Established method applied to a different problem with distinct scientific insights |
| 3 | Incremental extension to new conditions or parameter ranges |
| 2 | Additional geometry, dataset, site, configuration, or case with limited conceptual advance |
| 1 | Replication or minor refinement without a distinct scientific advance |
| 0 | No identifiable novelty; claimed contribution already established |

- Score the **knowledge or capability produced**, not the sophistication of the technology used.
- An experimental discovery of a new mechanism can score 9 even if the instrumentation is conventional.
- Half-points are permitted only with a defensible explanation; do not equate novelty with scientific importance.
- If closest prior work cannot be checked, mark the novelty score **provisional** in the insight.

### 3. Generalisability and downstream use — S3 (0–10)

\[
S_3 = G + U
\]

**G: Generalisability (0–5)**

| G | Scope |
|---:|---|
| 5 | Cross-disciplinary transfer to different scientific fields or physical systems |
| 4 | General class of systems sharing physical mechanisms |
| 3 | Multiple independent systems, sites, datasets, or devices within a class |
| 2 | Multiple configurations or operating conditions of one system type |
| 1 | Narrow extension beyond the investigated case |
| 0 | Specific case only |

**U: Downstream use (0–5)**

\[
U = \min(5, N_u)
\]

`N_u` is the number of **distinct, defensible, literature-supported downstream application categories** that could directly use the anticipated result (e.g., prediction, design, control, measurement, benchmarking, standards). Count each category once; do not multiply counts by publications or list speculative uses as established. Document assumptions or limitations of proposed transfers.

### 4. Scientific testability and rigour — S4 (0–10)

\[
S_4 = H + T + V + Q + C
\]

Score each component **0 = absent, 1 = partial, 2 = convincingly addressed in the proposed design**:

- **H (0–2):** Specific, testable predictions or distinguishable competing hypotheses.
- **T (0–2):** Decisive experiment, observation, derivation, or benchmark, with pass/fail or discriminating criteria.
- **V (0–2):** Independent validation using suitable external data, experiment, theory, proof, or numerical benchmark.
- **Q (0–2):** Quantified uncertainty and robustness to critical assumptions.
- **C (0–2):** Comparison with the strongest relevant published methods, explanations, or baselines.

Score **research logic and planned evidence**, not whether the desired result is guaranteed or inexpensive. For theoretical research, use proofs, counterexamples, error bounds, and independent verification as appropriate. Negative findings can be scientifically decisive.

### 5. Timing and historical relevance — S5 (0–10)

\[
S_5 = R + E + W
\]

- **R: Contemporary scientific relevance (0–4):** 0 none; 1 limited; 2 relevant ongoing problem; 3 strongly aligned with major current scientific developments; 4 addresses a major emerging or intensifying challenge.
- **E: Recent enabling developments (0–3):** 0 none; 1 minor; 2 important advances in data, theory, methods, or instrumentation; 3 recent breakthrough creates substantially new opportunity.
- **W: Time sensitivity (0–3):** 0 little difference if delayed; 1 some timing advantage; 2 substantial advantage now; 3 narrow opportunity whose value could be lost through delay.

As supporting evidence, compare bottleneck prevalence in comparable time windows: `Δp = (N_b,recent/N_r,recent) − (N_b,earlier/N_r,earlier)`. Rising attention alone does not prove significance. Timeless foundational questions need not be time-sensitive.

### 6. Enduring value and delayed impact — S6 (0–10)

\[
S_6 = L + R + F
\]

- **L: Longevity (0–4):** 0 transient; 1 tied mainly to current technical context; 2 partly durable; 3 substantial enduring scientific understanding or method; 4 foundational principle or approach likely to remain useful for decades.
- **R: Long-term reusability (0–3):** 0 little; 1 reference value; 2 transferable results or tools needing adaptation; 3 reusable theory, validated method, benchmark, code, or data with a credible long-term use path.
- **F: Future relevance (0–3):** 0 little identifiable future need; 1 plausible; 2 likely relevant to important future developments; 3 strong documented or analytically credible pathway to persistent or later-emerging value.

When evidence exists, examine lasting adoption of comparable historical contributions, rather than extrapolating short-term citation counts. Delayed recognition is **possible**, not essential or inherently superior. Do not duplicate the breadth-of-application count in Criterion 3.

### 7. Feasibility and opportunity cost — S7 (0–10)

\[
S_7 = A + E + D + O
\]

- **A: Resource availability (0–3):** 0 no credible access to critical inputs; 1 major gaps; 2 most resources accessible; 3 essential data, tools, expertise and facilities available.
- **E: Execution feasibility (0–3):** 0 no credible investigation pathway; 1 high technical or workload uncertainty; 2 credible with moderate development effort; 3 established, realistic approach.
- **D: Dependencies and risk (0–2):** 0 severe uncontrolled dependencies; 1 some unresolved dependencies; 2 controlled or with credible mitigations.
- **O: Opportunity cost (0–2):** 0 clearly inferior resource use relative to available alternatives; 1 reasonable but contested; 2 strongly justified relative to competing opportunities.

Evaluate the researcher's actual time, resources and collaborators. Distinguish feasibility of the *first discriminating pilot* from that of the complete programme. Compare opportunity costs against real alternatives; do not invent durations or success probabilities.

## Total and interpretation

\[
S_{\mathrm{total}} = \sum_{i=1}^{7} S_i \qquad (0\text{–}70)
\]

Use these precise numerical bands (including scores with decimals):

| Total | Required classification | Meaning |
|---:|---|---|
| 60–70 | **Exceptional potential** | Outstanding across nearly all criteria; candidate field-shaping programme; strongly prioritise. |
| 50–<60 | **High-impact potential** | Strong importance, novelty, rigour, and likely value; prioritise for serious investigation. |
| 40–<50 | **Promising research** | Credible contribution, but meaningful limitations remain; pursue selectively or improve. |
| 30–<40 | **Moderate / incremental** | Potentially publishable, but limited broader influence; usually redesign unless practical value justifies it. |
| 20–<30 | **Low potential** | Weak value relative to the required work; generally avoid or substantially reformulate. |
| 0–<20 | **Very low potential** | Serious deficiencies; drop or fundamentally reconsider. |

A high total must not hide critical issues: **S2 < 4** (low novelty), **S4 < 5** (weak testability/rigour), or **S7 < 3** (very low feasibility). Call out such a weakness succinctly in the affected insight or total interpretation. These are **review triggers**, not automatic exclusions.

For internal diagnosis, one may calculate scientific potential as `(S1 + ... + S6)/6` and report execution feasibility separately as `S7`; **do not show these extra numbers by default**, because the user's required output is the seven scores and total.

### Handling unavailable evidence

- Do not invent `N_b`, `N_r`, predecessors, applications, evidence, or numerical scores to fill gaps.
- If sufficient context supports a **tentative qualitative rubric score** (especially S2–S7), show the estimated score and identify the uncertainty in its insight.
- If a required score cannot be defensibly assigned (notably S1 without a defined literature sample), write **N/A/10** with a concise explanation. In that case, the final line must be **Total: Not defensible /70 — evidence incomplete**; optionally give the subtotal from scored criteria, but **never fabricate a comparable 70-point total**.
- Where evidence is limited but all scores can still be defended as provisional, show the total and classification, qualified as **provisional** in the final line.
- Present scores to one decimal at most; calculate the total from unrounded values where possible, then round once.

## Research and assessment procedure (internal; do not print by default)

1. Formulate the question precisely; distinguish question, contribution, and research plan.
2. Identify the limiting scientific/engineering bottleneck and construct a representative evidence sample to measure S1.
3. Locate the closest predecessor(s), contradictory findings, rival explanations and strongest baselines; score S2.
4. Identify credible transfer domains, assumptions, failure boundaries and non-overlapping downstream uses; score S3.
5. Check discriminating predictions, validation, uncertainty, and rigorous comparisons; score S4.
6. Examine contemporary drivers, enabling developments, time-sensitive opportunities, and historical context; score S5.
7. Evaluate likely 10–20-year durability, reusable outputs, and credible delayed or persistent scientific use; score S6.
8. Assess available data/resources, technical path, dependencies, manageable pilot and actual alternatives; score S7.
9. Compute total and category, check critical weaknesses, and write one evidence-based insight (≤50 words) per criterion.

The optional deeper analysis can investigate a cheap decisive test, a stop/pivot criterion, substantively different question formulations, and peer-reviewed literature sources. **Do not add that material to the default seven-line assessment**; provide it only upon request. For a portfolio, repeat the same seven-criterion format per question and, if explicitly asked to rank, supply a compact ranked summary after the assessments.

## Required response format — strictly follow

Display **exactly seven numbered criterion entries, in this order**. For each, put the **criterion name and its numeric score together in bold**, on one line. On the next line, provide **one concise insight, no more than 50 words**, grounded in evidence and highlighting the major strength, weakness, or uncertainty. Avoid tables, sub-scores, long prose, methodology digressions, separate verdict sections, and generic praise.

Then show **one bold total score with the matching classification and a one-sentence interpretation**. Do not show the detailed calculations, unless requested. No additional material by default.

**Output template (placeholders are NOT scores):**

**1. Scientific bottleneck prevalence — [S1]/10**  
[Evidence-based insight, ≤50 words.]

**2. Novelty and distinct contribution — [S2]/10**  
[Evidence-based insight, ≤50 words.]

**3. Generalisability and downstream use — [S3]/10**  
[Evidence-based insight, ≤50 words.]

**4. Scientific testability and rigour — [S4]/10**  
[Evidence-based insight, ≤50 words.]

**5. Timing and historical relevance — [S5]/10**  
[Evidence-based insight, ≤50 words.]

**6. Enduring value and delayed impact — [S6]/10**  
[Evidence-based insight, ≤50 words.]

**7. Feasibility and opportunity cost — [S7]/10**  
[Evidence-based insight, ≤50 words.]

**Total: [sum]/70 — [matching impact-potential classification].** [One sentence explaining the category's meaning for this research question, without promising future success.]

## Evidence discipline and tone

Prioritise primary studies, robust independent reviews, validated datasets, established benchmarks and documented scientific uptake. When using citations, put them in the corresponding criterion's insight; avoid decorative references. Identify substantial unknowns and the nearest challenge to novelty. Do not equate popularity with importance, citation velocity with enduring value, or practical feasibility with scientific originality.

Write like a critical research collaborator: clear, direct, specific, independent, and proportionate. In confidential invention discussions, assess non-confidential engineering methodology and validation without inventing or eliciting the protected inventive core.
