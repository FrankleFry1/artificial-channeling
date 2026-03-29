# Artificial Channeling: A Methodology for Applying Historical Intellectual Frameworks to Novel Problems via Large Language Models

**Author:** John Haun — Independent Researcher, Open Essai Project
**Preprint:** [NEEDS: arXiv link once registered]
**Status:** Pre-publication repository — Phase 1 complete, session transcripts in progress
**License:** [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)

---

## What Is This?

This repository supports the paper *Artificial Channeling*, which introduces a structured methodology for prompting large language models to apply the conceptual frameworks of historical thinkers to problems those thinkers never addressed.

When you channel a historical figure through an LLM, you are not simulating a person. You are performing *constrained generation from a learned subspace* — collapsing the model's probability distribution over a corpus into a coherent voice vector, then directing that vector toward novel territory. The methodology functions simultaneously as a practical thinking tool, an evaluation instrument for LLM creative intelligence, and a source of genuine intellectual output when the channeling succeeds.

The paper describes a complete protocol: a subject matrix of historical figures with analyzed *chanability*, a five-model AI council (ChatGPT, Grok, Gemini, MiniMax, Claude), four session question types, and a multi-dimensional scoring rubric. Selected findings include a Bateson-derived critique of AI alignment that independently converges with arguments in the alignment literature, and an Illich-derived analysis of AI counterproductivity that held consistently across all five model nodes.

---

## Repository Structure

```
artificial-channeling/
│
├── paper/
│   ├── manuscript.md                    ← Full paper (readable here)
│   └── artificial_channeling_paper.docx ← Original formatted version
│
├── sessions/
│   ├── TEMPLATE/                        ← Blank templates for replication
│   │   ├── transcript.md
│   │   └── scoring.md
│   └── [session folders in progress]    ← Individual session records
│       ├── transcript.md
│       └── scoring.md
│
├── methodology/
│   ├── framework_activation_block.md   ← The FAB prompt (replicate sessions from here)
│   ├── session_design_principles.md    ← Full session protocol
│   └── calibration_questions.md        ← Per-figure calibration question bank
│
└── references/
    ├── bibliography.bib                ← All citations in BibTeX
    └── reference_audit.md              ← Verification notes on citations
```

---

## How to Navigate

**Read the paper:**
Start with [`paper/manuscript.md`](paper/manuscript.md) — the full text renders directly in GitHub.

**Replicate a session:**
Copy [`sessions/TEMPLATE/`](sessions/TEMPLATE/) to `sessions/[figure]_[model]_[date]/` and follow the Framework Activation Block in [`methodology/framework_activation_block.md`](methodology/framework_activation_block.md).

**Understand the protocol:**
[`methodology/session_design_principles.md`](methodology/session_design_principles.md) documents all session design decisions, question type definitions, scoring rubric, and failure mode reference.

**Review session data:**
[`sessions/`](sessions/) — each folder contains a full session transcript and scoring sheet. In progress as transcripts are formatted.

**Cite the paper:**
BibTeX entry below.

---

## How to Cite

```bibtex
@misc{haun2026artificial,
  author        = {Haun, John},
  title         = {Artificial Channeling: A Methodology for Applying Historical
                   Intellectual Frameworks to Novel Problems via Large Language Models},
  year          = {2026},
  eprint        = {[NEEDS: arXiv ID]},
  archivePrefix = {arXiv},
  note          = {Open Essai Project. Repository: https://github.com/[NEEDS: GitHub URL]}
}
```

---

## Key Terminology

This paper introduces several original terms. Brief definitions:

| Term | Definition |
|------|-----------|
| **Artificial Channeling** | Prompting an LLM to apply a historical thinker's framework to a problem they never addressed; distinct from simulation or impersonation |
| **Subspace Coherence** | Degree to which session output stays within the figure's learned framework vs. drifting to generic LLM voice |
| **Chanability** | A figure's suitability as a channeling subject; function of corpus density, vocabulary idiosyncrasy, and ontological coherence — not fame |
| **Rough Edge Preservation** | Whether a session retains the figure's uncomfortable or counterintuitive implications; diplomatic softening is scored as a failure |
| **The Plausibility Trap** | The most dangerous failure mode: output sounds like the figure and is internally consistent, but the framework is not actually generative |
| **Extrapolation Threshold** | The point at which a prompt moves from framework retrieval into genuine application |

---

## About Open Essai

Open Essai is a longitudinal study of human experience and consciousness. This paper describes its first published methodology — a protocol developed from the project's need to apply pre-AI conceptual frameworks to questions those frameworks were not built to answer.

---

## License

This work is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).
You are free to share and adapt this material for any purpose, provided appropriate credit is given.
