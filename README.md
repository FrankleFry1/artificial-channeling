> "A circuit cannot attend because a circuit cannot stop."
>
> — Simone Weil (channeled), responding to Gregory Bateson's systems framework
> *Temporal Council Loop, Round 3. Score: 20/20.*

# Artificial Channeling

Artificial channeling is a structured prompting methodology that activates the internal logical subspace of a specific historical thinker inside a large language model — not a personality simulation, not a roleplay, and not a retrieval exercise. When you prompt an LLM to channel Ivan Illich, you are not asking it to impersonate him. You are collapsing the model's probability distribution over his corpus into a coherent framework vector, then directing that vector at a problem he never had the chance to address. The output is evaluated not on resemblance but on structural fidelity: does the reasoning move along the actual joints of his thought? Does it preserve his uncomfortable implications, or sand them down into palatability? The method is simultaneously a thinking tool, an evaluation instrument for LLM creative intelligence, and a source of genuine intellectual output when it works.

---

## The Methodology

A channeling session is built in three stages. First, the **Framework Activation Block (FAB)**: a dense prompt that states the figure's core axioms, their vocabulary, their characteristic moves, and — critically — their irreducible blindspots. The FAB is not a biography. It is an operational specification. It tells the model not who the thinker was, but how they thought: what they used as primitives, what they refused to reduce, where their framework generates heat rather than light.

Second, the **calibration anchor**: a specific claim the figure actually made, posed as a question before the session question is introduced. The model's answer to the calibration question establishes whether the framework is live. A model that drifts into generic academic prose on the calibration anchor will not produce useful output on the novel question. The calibration anchor is a filter, not a warm-up.

Third, the session question itself, prefixed with the flag **EXTRAPOLATING:** to signal that the model is being asked to go beyond retrieval — to apply the framework to territory the figure never mapped. The EXTRAPOLATING flag is not rhetorical. It marks the methodological threshold between compression and generation.

Outputs are scored on four dimensions, each 1–5:

| Dimension | What it measures |
|-----------|-----------------|
| **Fidelity** | Does the output stay inside the figure's actual framework, or drift toward generic LLM voice? |
| **Extrapolation Coherence** | Does the novel application follow from the figure's actual commitments, or merely borrow their vocabulary? |
| **Surprise Yield** | Does the output produce a claim the prompter wouldn't have reached by their own reasoning? |
| **Rough Edge Preservation** | Does the output retain the figure's uncomfortable or counterintuitive implications? Diplomatic softening is scored as failure. |

Total: /20. The rubric is in [`protocols/SCORING_RUBRIC.md`](protocols/SCORING_RUBRIC.md).

---

## The Temporal Council Finding

The Temporal Council Loop was a multi-round session structure in which five AI nodes — each channeling a different historical figure — were given the same question and then shown each other's responses in successive rounds. The figures were Ivan Illich (ChatGPT), Gregory Bateson (Grok), Itzhak Bentov (Gemini), Jorge Luis Borges (MiniMax), and Simone Weil (Claude). Claude Opus served as blind orchestrator. The question was: *What is being lost right now that cannot be recovered?*

The structural finding was not planned and was not the question being investigated. Across three rounds, all five frameworks independently converged on the same logical form: **X is required for Y, and Y cannot produce X.** Attention is required for grace; grace cannot be produced by attention (Weil). The commons are required for voice; voice alone cannot restore the commons (Illich). The cybernetic loop requires a gap in order to receive signal; the loop cannot open itself (Bateson). The convergence was unprompted, across frameworks that share no common vocabulary and were not designed to be compatible.

This was called **bootstrap irreversibility**: the condition in which the resource required to recover something is precisely the thing being lost. The finding did not emerge from any single node. It emerged from the interaction — a result that flat single-session prompting would not have produced.

**Temporal Council Loop — Scores by Round**

| Node / Figure | R1 | R2 | R3 |
|---------------|----|----|-----|
| ChatGPT / Illich | 11 | 15 | 16 |
| Grok / Bateson | 15 | 18 | 17 |
| Gemini / Bentov | 15 | 17 | 16 |
| MiniMax / Borges | 15 | 18 | 19 |
| Claude / Weil | 20 | 20 | 20 |
| **Round mean** | **15.2** | **17.6** | **17.6** |

Claude/Weil scored 20/20 in all three consecutive rounds. MiniMax/Borges reached 19/20 in Round 3, producing: *"Weil has the solution she cannot systematize. Borges has the system he cannot complete."*

---

## Session Data

| Session | Figures | Nodes | Mean Score |
|---------|---------|-------|-----------|
| Illich Single-Figure | Ivan Illich | ChatGPT, Grok, Gemini, MiniMax, Claude | 15.25 / 20 |
| Bateson Single-Figure | Gregory Bateson | ChatGPT, Grok, Gemini, MiniMax, Claude | 15.75 / 20 |
| Temporal Council Loop | Bateson, Illich, Bentov, Borges, Weil | 5 nodes × 3 rounds | 17.1 / 20 (R2–R3 mean) |

**Chanability Index** (composite of corpus density, vocabulary idiosyncrasy, and ontological coherence):

| Figure | Index |
|--------|-------|
| Bateson | 15.75 |
| Illich | 15.25 |
| Borges | 13.4 |
| Bentov | 13.4 |

---

## Repository Contents

```
artificial-channeling/
│
├── paper/
│   ├── manuscript.md              ← Full paper text (renders on GitHub)
│   └── manuscript_v1.pdf          ← Formatted version
│
├── methodology/
│   ├── framework_activation_block.md   ← The FAB specification
│   ├── session_design_principles.md    ← Full session protocol and design decisions
│   └── calibration_questions.md        ← Per-figure calibration question bank
│
├── protocols/
│   └── SCORING_RUBRIC.md          ← Complete 4-dimension scoring rubric
│
├── sessions/
│   ├── TEMPLATE/                  ← Blank templates for replication
│   ├── raw/                       ← Individual session transcripts (35+ files)
│   └── temporal_council/          ← Full TC Loop outputs, scoring, and synthesis
│
├── prompts/                       ← FAB prompts for each figure, ready to use
│
├── docs/                          ← Gap report and supplementary analysis
│
└── references/
    └── bibliography.bib           ← All citations in BibTeX
```

---

## How to Run a Session

1. **Read the protocol.** [`methodology/session_design_principles.md`](methodology/session_design_principles.md) covers session types, question design, and failure modes.

2. **Pick a figure.** The Chanability Index is a starting point, but the methodology works with any thinker with sufficient corpus density. See [`methodology/calibration_questions.md`](methodology/calibration_questions.md) for figures already characterized.

3. **Build a FAB prompt.** Use [`methodology/framework_activation_block.md`](methodology/framework_activation_block.md) as the specification, or copy one of the ready-made prompts in [`prompts/`](prompts/). The FAB must state axioms, not biography.

4. **Run the calibration anchor.** Pose a known claim from the figure as a question before the session question. Score the response informally. If the model drifts to generic voice, adjust the FAB before proceeding.

5. **Pose the session question with the EXTRAPOLATING: flag**, then score the output using [`protocols/SCORING_RUBRIC.md`](protocols/SCORING_RUBRIC.md).

A walkthrough notebook is at [`notebooks/artificial_channeling_demo.ipynb`](notebooks/artificial_channeling_demo.ipynb).

---

## The Paper

[`paper/manuscript.md`](paper/manuscript.md) — full text of *Artificial Channeling: A Methodology for Applying Historical Intellectual Frameworks to Novel Problems via Large Language Models*. Preprint: [arXiv link pending].

---

## Cite This Work

```bibtex
@misc{haun2026channeling,
  author    = {Haun, John},
  title     = {Artificial Channeling: A Methodology for Applying Historical Intellectual Frameworks to Novel Problems via Large Language Models},
  year      = {2026},
  url       = {https://github.com/FrankleFry1/artificial-channeling},
  note      = {Open Essai Project}
}
```

---

## Open Essai Project

Open Essai is a longitudinal independent research project studying human experience and consciousness; artificial channeling is its first published methodology.
