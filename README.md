# Research Question Assessment

An AI assistant skill for critically assessing, comparing, formulating, and redesigning scientific research questions. Created by **[Dr Yusuf R. Almalki](https://yusufradad.com/)**.

**This is an experimental, evidence-informed framework, not a scientifically validated predictor of research impact.** It supports reasoned decisions about what to investigate; it does not predict citations, funding, publication, or transformative outcomes.

## Purpose

Move beyond finding a publishable gap to identifying a consequential unresolved problem and a credible way to investigate it. The skill encourages independent criticism, explicit uncertainty, strong alternatives, and inexpensive tests before committing to a full research programme.

Use it for a **quick screen**, an **evidence-backed assessment**, a **portfolio comparison**, or **question development**. Evidence-backed assessments require access to relevant literature or sources supplied by the researcher.

## Assessment criteria

| Criterion | Central question |
| --- | --- |
| Importance and bottleneck | What cannot currently be explained, measured, predicted, or decided, and who needs the answer? |
| Originality | What distinct contribution would go beyond the closest prior work? |
| Generalisability and use | Where would the result transfer, who would use it, and where would it fail? |
| Testability | What decisive evidence distinguishes the proposal from credible alternatives? |
| Timing and historical relevance | Why does the question matter in its scientific context now? |
| Enduring value and delayed impact | What might remain useful in 10–20 years, including work whose adoption depends on future capabilities? |
| Feasibility and opportunity cost | What are the dependencies, cheapest meaningful first test, and reasons to stop or pivot? |

The framework recognises consequential contributions within a narrow domain. It does not equate breadth or early citation counts with scientific value.

Assessments use **supported / plausible / unclear / contradicted**, with a reasoned verdict: **PURSUE**, **PILOT FIRST**, **REDESIGN**, **PARK**, or **DROP**. There is no numeric impact score or preset weighting. Verdicts remain provisional when evidence is weak.

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

Ask the assistant to use `research-question-assessment`, choose a mode, and supply your research question, intended contribution, relevant prior work, available data or equipment, constraints, and alternatives where known. In evidence-backed mode, provide sources or enable literature-search tools. The assistant should distinguish verified evidence, your supplied context, reasoned inference, and unknowns.

Expect a sharpened question, verdict and confidence, assessment across the criteria, strongest objection, improved formulations when warranted, a minimal staged research plan, and evidence gaps. The plan should identify a decisive pilot and explicit conditions to expand, stop, or pivot.

### Example

The following is a hypothetical teaching example in wave energy, not a description of the author's research plans.

```text
Use the research-question-assessment skill in quick-screen mode.

Question: How much does neglecting wave directional spreading change
the estimated annual energy yield of a generic wave energy converter
at a hypothetical coastal site?

Assume access to a public directional wave dataset and a published
benchmark converter model. Compare predictions using the directional
wave distribution with predictions that represent each sea state by
a single direction, keeping the other modelling assumptions consistent.
The proposed contribution is guidance on when this simplification is
adequate for preliminary energy-yield estimates. Resources are limited
to a small numerical study using existing data.

Assess whether the question adds anything beyond established findings.
Challenge the baseline, validation, and scope of inference. Identify
the closest prior work that would need checking, propose the cheapest
informative pilot if warranted, and specify when to expand, pivot, or stop.
Do not assume the question is novel or worth pursuing.
```

This illustrative prompt does not establish that the proposed question is novel or valuable. A verdict depends on the evidence and research context.

## Attribution and licence

Created by **Dr Yusuf R. Almalki** — [yusufradad.com](https://yusufradad.com/).

Released under the [MIT License](LICENSE). You may use, adapt, and redistribute the skill subject to that licence, including preservation of its copyright and permission notice.
