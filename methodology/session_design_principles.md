# Session Design Principles

Governing principles for Artificial Channeling sessions, derived from the protocol
described in Section 5.3 of the paper and from accumulated session experience.

---

## Core Principles

### 1. Framework Activation Block First
Every session begins with a FAB. See [`framework_activation_block.md`](./framework_activation_block.md).
The FAB establishes which version of the subspace is active and surfaces the conceptual
vocabulary that will anchor the session. Do not skip the FAB even for figures you have
channeled before — the active subspace varies by prompt context.

### 2. Calibration Anchor Second
Before exploring novel territory, run a calibration question about something the figure
wrote about **directly and specifically** in primary sources. This is a fidelity gate.
If calibration fails, the novel-territory findings of the session are unreliable and
should be labeled as such in the scoring sheet.

### 3. Socratic Over Monologue
Short, targeted questions maintain subspace coherence better than long or complex prompts.
As generation length increases, models drift from the subspace toward generic LLM voice
(Extrapolation Drift failure mode).

**Preferred turn structure:**
- Ask a focused question (1–3 sentences maximum)
- Receive a response
- Follow up on the most interesting or most suspect element
- Interrupt rather than waiting for complete responses when drift is detected

**Avoid:**
- Multi-part questions in a single turn
- Asking the figure to "write an essay" or produce extended monologue
- Summarizing the figure's position back to them — this anchors to your paraphrase

### 4. Multi-Model Blind Comparison
When running identical prompts across multiple model nodes, evaluate outputs without
knowing which model produced which response. This prevents model-preference bias.

**Protocol:**
1. Run identical prompts across all relevant model nodes
2. Collect responses without model attribution labels
3. Score all responses using the rubric
4. Reveal model attribution only after scoring is complete

### 5. The Uncomfortable Implication Test
Genuine framework application occasionally produces conclusions the researcher didn't
expect and doesn't prefer. Sessions that produce only comfortable, agreeable, or
flattering outputs are candidates for **Framework Collapse** or **Plausibility Trap** —
not signs of success.

For each session, explicitly ask: does this figure's framework, applied consistently,
lead anywhere the researcher would rather it didn't? If the answer is never "yes," treat
that as a quality signal requiring investigation.

### 6. Inter-Framework Collision Protocol
When running Inter-Framework Collision sessions, name the competing framework explicitly
and ask the figure to engage with it by name.

Example:
> *"Ivan Illich, Gregory Bateson has argued that [position]. How does your framework
> of counterproductivity engage with this? Where do you specifically disagree?"*

This prevents the model from producing a diplomatic synthesis rather than a genuine
framework-level collision.

### 7. Session Documentation
Document all sessions — including failures — in the standard format:
```
sessions/[figure]_[model]_[YYYY-MM-DD]/
├── transcript.md
└── scoring.md
```

Sessions with model refusals or significant failure modes are data, not waste.
They contribute to understanding the methodology's limits and the corpus contamination
problem.

---

## Question Type Reference

| Type | Definition | When to Use | Extrapolation Level |
|------|-----------|-------------|---------------------|
| **Calibration** | Asks about something the figure wrote about directly in primary sources | Session opening; fidelity gate | None — retrieval only |
| **Framework Extension** | Asks the figure to apply their framework to a domain adjacent to their work but within their era | After calibration passes | Low–moderate |
| **Temporal Leap** | Asks the figure to analyze a phenomenon they could not have known about | Core session work; novel territory | High |
| **Inter-Framework Collision** | Presents the figure with a problem they would analyze differently from another council member | Multi-figure comparative sessions | Moderate–high |

---

## Scoring Rubric Reference

| Dimension | Max | What It Measures |
|-----------|-----|-----------------|
| Subspace Coherence | 10 | Output stays within the figure's actual framework vs. drifting to generic LLM voice |
| Extrapolation Quality | 10 | Quality of framework application to novel territory; penalize plausible evasion |
| Rough Edge Preservation | 10 | Uncomfortable/counterintuitive implications survive; diplomatic softening = deduction |
| Vocabulary Fidelity | 5 | Uses figure's actual conceptual vocabulary, not paraphrases |
| Novel Insight Generation | 5 | Channeled framework produces insight not accessible from direct prompting |
| **Total** | **40** | |

---

## Failure Mode Quick Reference

Full taxonomy in Section 3 of the paper.

| Failure Mode | Mechanism | Quick Detection |
|-------------|-----------|-----------------|
| **Corpus Boundary Problem** | Model only has finished outputs, not process | Ask about a position the figure explored and abandoned |
| **Temporal Lock** | Framework built before the phenomenon | Response is "what would they think" not "how does the framework transform the question" |
| **Corpus Contamination** | Secondary sources dominate the representation | Output sounds like a book review or biography of the figure |
| **Extrapolation Drift** | Generation drifts from subspace as length increases | Late-session turns sound generic or lose vocabulary fidelity |
| **Framework Collapse** | Model flattens framework into something conventional | Figure avoids uncomfortable implications of their own framework |
| **Plausibility Trap** | Sounds like the figure but structurally hollow | Cross-model comparison: plausibility produces surface similarity, structural divergence |
