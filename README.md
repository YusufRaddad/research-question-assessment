# Research Question Assessment

An AI assistant skill for critically assessing and comparing scientific research questions using a seven-criterion quantitative rubric (v2.0). Created by **[Dr Yusuf R. Almalki](https://yusufradad.com/)**.

**This is an experimental, evidence-informed framework, not a scientifically validated predictor of research impact.** It supports reasoned decisions about what to investigate; it does not predict citations, funding, publication, or transformative outcomes.

## Purpose

Move beyond finding a publishable gap to identifying a consequential unresolved problem and a credible way to investigate it. The skill encourages independent criticism, explicit uncertainty, strong alternatives, and inexpensive tests before committing to a full research programme.

Use it to assess a research question or compare candidate directions against existing scientific evidence. Literature-based assessments require access to relevant publications or sources supplied by the researcher. Deeper analysis, question reformulation, and pilot planning are available when explicitly requested.

## Assessment criteria

| Criterion | Central question |
| --- | --- |
| Scientific bottleneck prevalence | What proportion of a defined, representative literature sample explicitly identifies the same unresolved bottleneck? |
| Novelty and distinct contribution | What new knowledge or capability would go beyond the closest established predecessor? |
| Generalisability and downstream use | Where would the result transfer, and which distinct applications have literature support? |
| Scientific testability and rigour | Are hypotheses, decisive tests, independent validation, uncertainty, and strong comparisons addressed? |
| Timing and historical relevance | Why does the question matter in its scientific context now? |
| Enduring value and delayed impact | What might remain useful in 10–20 years, including work whose adoption depends on future capabilities? |
| Feasibility and opportunity cost | What are the dependencies, cheapest meaningful first test, and reasons to stop or pivot? |

Each criterion is scored **0–10**, for a **total of 70**. The framework recognises consequential contributions within a narrow domain. Bottleneck prevalence measures recognition in the sampled literature, not intrinsic importance; breadth and early citation counts are not measures of scientific value.

Totals map to provisional categories from **Very low potential** to **Exceptional potential**, with thresholds and scoring rules defined in [SKILL.md](SKILL.md). These bands are not empirically calibrated predictions. Critical weaknesses in novelty, rigour, or feasibility must remain visible even when the total is high.

Missing evidence must not be replaced with invented scores. If a required score cannot be defended, the assistant reports **N/A/10** and **Total: Not defensible /70 — evidence incomplete** rather than fabricating a comparable total.

## Installation

No packages, API keys, or executable code are required by the skill itself.

1. Clone this repository, or download it using **Code → Download ZIP** and extract it:

   ```sh
   git clone https://github.com/YusufRaddad/research-question-assessment.git
   ```

2. For an assistant that supports `SKILL.md` skills, place the `research-question-assessment` folder in that assistant's configured skills directory. Follow its instructions for loading or enabling local skills; directory locations vary by assistant.
3. For other AI assistants, attach [SKILL.md](SKILL.md) or paste its contents into the conversation, then explicitly ask the assistant to apply it.

The folder contains a `SKILL.md` with YAML `name` and `description` metadata. The skill is provided as plain Markdown; automatic discovery depends on the assistant. The original methodology and instructions are preserved unchanged in [SKILL.md](SKILL.md).

## Usage

Ask the assistant to use `research-question-assessment` and supply your research question, intended contribution, relevant prior work, available data or equipment, constraints, and alternatives where known. Provide sources or enable literature-search tools. The assistant should distinguish verified evidence, your supplied context, reasoned inference, and unknowns.

The default response contains **exactly seven numbered criteria**, each with a bold score out of 10 and one evidence-based insight of no more than 50 words, followed by the total, its category, and a brief interpretation. Detailed calculations, alternative formulations, and research plans are included only when requested.

### Example

The example below is phrased as a proposal and draws on the topic of completed, published work:

Almalki, Y.R. and Karmpadakis, I. (2026). [Effects of OWC geometry on total energy efficiency and turbulent dissipation](https://doi.org/10.1016/j.apor.2026.105026). *Applied Ocean Research*, **170**, 105026.

```text
I am considering investigating how front and back wall geometries affect the hydrodynamic performance of caisson-integrated oscillating water columns (OWCs), particularly the role of turbulent energy dissipation.
I plan to use physical experiments and CFD simulations to investigate the underlying mechanisms, performance differences, and scale effects.
Use the `research-question-assessment` skill to critically evaluate this research question based on the existing scientific literature.
```

This is an illustrative reformulation of a published research topic, not a claim of a new research question or a disclosure of future research plans. Publication alone does not validate the assessment framework or establish future impact.

## Attribution and licence

Created by **Dr Yusuf R. Almalki** — [yusufradad.com](https://yusufradad.com/).

Released under the [MIT License](LICENSE). You may use, adapt, and redistribute the skill subject to that licence, including preservation of its copyright and permission notice.
