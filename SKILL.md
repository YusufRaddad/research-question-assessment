---
name: research-question-assessment
description: Critically assess and compare scientific research questions using seven evidence-informed criteria scored out of 10 (70 points total), with a concise criterion-by-criterion justification and an impact-potential category. Use for assessing novelty, scientific bottlenecks, generalisability, rigour, timing, durability, feasibility, or research portfolio priorities.
---

# Research Question Assessment — Quantitative Rubric (v2.2)

## Mission

Help researchers choose questions that could advance knowledge or capability, rather than merely fill a publication gap. Evaluate independently and critically, including recommending a redesign or abandonment where justified. A score represents a **structured judgement about research impact potential**, **not a validated predictor of citations, discoveries, funding, or future impact**.

**Default output is extremely concise:** seven numbered criterion headings, each containing its **bold criterion name and bold score out of 10**, followed by one evidence-based insight of **no more than 50 words**; then the **bold total out of 70, the category name, and its meaning**. Do not append additional sections unless the user requests them.

## Foundational rules

- First identify the **research question**, **anticipated contribution**, and **planned investigation**; these are not interchangeable. A technique (e.g., CFD), device, deliverable, or unstudied parameter is not itself a scientific question.
- Evaluate the anticipated contribution **relative to the closest existing original work**, not merely the absence of an identical title.
- Base scores on verified literature and other relevant evidence when available. Distinguish confirmed facts, the researcher's claims, reasonable inference, and unknowns. Literature-search absence is not proof of novelty.
- **Always assess whether Criterion 1 describes a real scientific bottleneck before attempting a prevalence estimate.** A routine parameter study, geometry comparison, or application of established methods does not automatically qualify. When a targeted literature check supports the conclusion that no substantive bottleneck is identified, assign **S1 = 0**, not N/A. If one qualifies, apply the neutral literature prevalence protocol.
- Assess the scientific logic rigorously: competing hypotheses, decisive tests, baselines, independent validation, uncertainty, counterexamples, and failure boundaries.
- Do not automatically reward broad transferability or trendy topics over consequential, narrow, application-specific work.
- Separate **scientific potential** (Criteria 1–6) from **execution feasibility** (Criterion 7) when interpreting the total. An ambitious question should not be dismissed solely because it is difficult.
- Scores and thresholds below are **provisional rubrics**, not empirically calibrated outcome probabilities. Avoid fabricated counts, effect sizes, references, time estimates, or confidence.
- Retain intellectually independent judgement: published but incremental is not necessarily programme-worthy; sunk costs are not evidence of merit.

## Scoring: seven criteria, each 0–10

### 1. Scientific bottleneck prevalence — S1 (0–10)

**Measure recognition of a genuine unresolved obstacle to progress**, not merely an interesting factor, a knowledge gap, a publishable topic, or a subject's popularity. **Zero is a valid and informative result.** Use a two-stage assessment:

#### Stage A — Bottleneck qualification (B)

Decide whether the question aims to resolve a **specific, consequential obstacle** that currently prevents or materially limits explaining, measuring, predicting, calculating, validating, or deciding something important. Identify **what is blocked, for whom, and by what missing knowledge or capability**. Check the closest relevant primary research and a recent review when available.

- **B = 1:** A specific unresolved obstacle is identified and supported by prior scientific evidence; resolving it could remove a material limitation. A newly emerging bottleneck may qualify even if few papers mention it.
- **B = 0:** The question describes a routine effect, geometry or parameter comparison, incremental optimisation, new site or application, or a general request to 'understand more', **without evidence of an obstacle blocking scientific or engineering progress**. Assign **S1 = 0/10**, with a brief explanation. **Do not require a 30–50-paper prevalence count just to justify this zero.**

Do not treat a missing exact-match paper, statements such as 'little studied', or generic calls for further research as evidence of a bottleneck. Likewise, **do not infer B = 0 solely from search failure or inaccessible literature**; the decision needs an interpretable question and an adequate targeted check of its nearest predecessors. If access is entirely inadequate to judge qualification, B is unknown rather than zero.

#### Stage B — Prevalence among relevant papers (only when B = 1)

\[
S_1 = \begin{cases}
0, & B=0,\\[2pt]
10\,\dfrac{N_b}{N_r}, & B=1,\;N_r>0.
\end{cases}
\]

- **N_b:** Number of assessable, independent eligible publications explicitly identifying or demonstrating the **same substantive unresolved bottleneck** as a material obstacle.
- **N_r:** All independent eligible publications assessable for that bottleneck, including those not recognising it (`N_r = N_b + N_no`).
- **B:** Qualification indicator, either 0 or 1. Record **B = 0, S1 = 0** when no substantive bottleneck is established; `N_b/N_r` is then **not required** and must not be invented.
- Count each independent investigation once, and code uncertain/inaccessible publications separately rather than treating them as negative evidence.
- When **B = 1** and a sound sample yields **N_b = 0**, the prevalence score is also **0/10**; it is not N/A. Explain that recognition is absent in the assessed sample, not that the problem cannot matter.

#### Default literature protocol (automatic; proportionate to the question)

1. **Identify the candidate obstacle before searching.** State what progress it would block, then define a neutral parent research domain **without selecting only papers about the alleged bottleneck**. If the question does not imply a concrete obstacle, do not invent one to obtain a positive score.
2. **Check qualification first.** Examine the closest original research and relevant reviews over the **past 10 years** (plus foundational work when applicable), using neutral queries. Inspect substantive passages where accessible. Decide **B = 0 or B = 1** based on whether a material unresolved bottleneck is actually established. A defensible **B = 0** ends Criterion 1 here with **S1 = 0**; it does not require further prevalence sampling.
3. **If B = 1, sample broadly.** Target **50 independent original research papers** with a balanced mix of years, researchers, methods and applications. Use multiple neutral queries and scholarly sources where feasible. Record the scope, publication window, sources, and sampling limitations. Reviews primarily help locate original papers; if counted, disclose this and apply it consistently.
4. **Code consistently.** For each eligible paper record **yes** (explicit bottleneck), **no** (relevant content examined and bottleneck not identified), or **uncertain** (not enough accessible content). Record source identifiers and supporting passages. **No** cannot be concluded from abstract silence alone. Count `N_r = yes + no`; keep uncertain papers outside the denominator and report their number when material.
5. **Calculate and disclose.** For B = 1, use `S1 = 10 N_b/N_r`, including **zero** when `N_b = 0` in a credible sample. Provide `N_b/N_r` and confidence in the short insight; check sensitivity to reasonable scope changes when feasible. Do not fabricate counts or silently broaden/narrow a domain to manipulate the result.
6. **Use confidence labels, not a minimum-score barrier.** **50+** assessable papers: standard sample-based estimate; **30–49**: provisional; **10–29**: exploratory; **fewer than 10**: very-low-confidence estimate **only if** the accessible eligible corpus is credibly close to complete. These numbers are pragmatic conventions, not calibrated statistical thresholds. **Do not use N/A merely because the target of 50 was not reached.**

**Decision hierarchy:** (i) a supported **B = 0** always yields **0/10**; (ii) with **B = 1**, a credible numerator/denominator yields a numeric score, including **0/10**; (iii) use **N/A only when neither qualification nor an interpretable prevalence estimate can be established because evidence or access is genuinely inadequate**. **Lack of recognition is a measured zero only following an adequate check—not an inference from a failed search.** The score reflects recognised bottleneck prevalence, **not intrinsic scientific importance**.

**Example:** “How do alternative front and back wall geometries affect OWC performance?” is primarily a geometry–performance investigation. If the closest literature does not show that the question resolves a specific obstacle preventing scientific or engineering progress, assign **B = 0; S1 = 0/10**. Merely adding CFD or turbulence analysis does not create a bottleneck. If the investigator instead identifies a documented inability to predict viscous-loss scaling that blocks reliable design, assess that *specific obstacle* and then measure its prevalence.

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
- **For S1, perform bottleneck qualification first.** If no substantive bottleneck is established after checking relevant prior work, report **0/10** and compute the normal total out of 70. Do **not** substitute N/A just because no bottleneck exists, recognition is zero in a credibly sampled corpus, or the 50-paper target is unmet. Use **N/A/10** only for genuinely unassessable evidence (e.g., inadequate literature access for qualification, or a known bottleneck with no interpretable prevalence sample). If any required score truly is unavailable, the final line must be **Total: Not defensible /70 — evidence incomplete**; optionally give a subtotal, but **never fabricate a 70-point total**.
- Where evidence is limited but all scores can still be defended as provisional, show the total and classification, qualified as **provisional** in the final line.
- Present scores to one decimal at most; calculate the total from unrounded values where possible, then round once.

## Research and assessment procedure (internal; do not print by default)

1. Formulate the question precisely; distinguish question, contribution, and research plan.
2. Evaluate whether a **substantive scientific/engineering bottleneck is established at all**. Check the nearest prior work and the default 10-year literature window (plus foundations). If **B = 0, S1 = 0** and continue; do not manufacture a bottleneck or demand 50 papers. If **B = 1**, define a neutral domain and estimate prevalence from assessable yes/no original studies (target 50 when feasible), with sample size, uncertain cases and confidence. If evidence genuinely cannot support either result, use N/A.
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

Then show **one bold total score with the matching classification and a one-sentence interpretation**. Do not show detailed calculations or the full search protocol unless requested. For S1, if **B = 0**, explain briefly why the question does not remove a documented bottleneck; **a zero score needs no invented `N_b/N_r` count**. If **B = 1**, give the measured `N_b/N_r` and confidence where space permits. No additional material by default.

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
