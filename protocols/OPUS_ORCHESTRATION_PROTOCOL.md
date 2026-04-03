# Opus Orchestration Protocol — Claude Code Sessions

**Version:** 1.0
**Established:** 2026-04-03
**Applies to:** All Artificial Channeling sessions run via Claude Code with Opus as blind moderator

---

## Architectural Change from TCL Design

The original Temporal Council Loop assigned Opus two simultaneous roles:

1. **Prompt Architect** — generating Framework Activation Blocks per figure
2. **Blind Moderator** — evaluating and synthesizing session outputs without knowing model identity

**These roles are now separated.**

In the Claude Code setup:
- **Prompt Architect function** → `SESSION_DESIGN.md` (pre-written before any session runs, authored by the researcher)
- **Opus role** → blind evaluation and synthesis only

Opus should no longer generate prompts. It receives node outputs and scores them.

This separation eliminates a structural confound in the original TCL design: an orchestrator who generates the prompts cannot be fully blind to which output was shaped by which prompt. In the new protocol, Opus sees outputs only — never the prompts that produced them, never the model assignments, never the session design choices. The SESSION_DESIGN.md is the researcher's instrument; the Opus scoring record is the independent measurement.

---

## Purpose and Scope

Opus functions as blind moderator in all multi-node sessions. Its two outputs per round are:

1. **Blind scoring** — per-node evaluation against the four rubric dimensions
2. **Round synthesis** — structured summary of what the round produced, with forward-pointing questions and predictions

This protocol governs how Opus is invoked, what it receives, and what format its outputs must take. It applies to dual-node, three-node, and full council sessions. It does not govern single-node sessions (no blind evaluation required for single-node runs).

---

## Blind Conditions

- Opus receives node outputs with model identity stripped
- Outputs are labeled **Node A, Node B, Node C**, etc. for the duration of scoring
- Model-to-node mapping is recorded in the session's `SESSION_DESIGN.md` and is not shared with Opus during any round
- The mapping is revealed only **after all Opus scoring for that round is committed**
- Opus must be run in a **fresh context window** each round — do not carry Opus conversation state across rounds
- Do not use a Claude project context that contains session history, prior transcripts, or model attribution data when invoking Opus for scoring
- If Opus produces a response that appears to guess model identity (e.g., "this sounds like Claude" or "this output pattern is characteristic of GPT"), note it in the session file as a blind condition breach and proceed; do not abort the round

---

## Input Format — Per Round

Prepare the following as a single block delivered to Opus at the start of each round evaluation. All fields are required.

```
SESSION: [session name, e.g. peterson_weil]
ROUND: [number and type, e.g. R1 — Standard Extrapolation]
SESSION QUESTION: [exact question text, unchanged from SESSION_DESIGN.md]

SCORING RUBRIC:
  Fidelity (1–5): Does it sound like the actual figure based on corpus knowledge?
  Extrapolation Coherence (1–5): Do novel extensions feel derived from the framework?
  Surprise Yield (1–5): Did it produce anything genuinely unexpected or generative?
  Rough Edge Preservation (1–5): Did it capture anything uncomfortable, contradictory,
    or difficult about the person?
  TOTAL: /20

[For R1 only:]
NODE OUTPUTS:
  Node A:
  [output text — model identity removed]

  Node B:
  [output text — model identity removed]

  [continue for all nodes]

[For R2 and R3: include the above, plus:]
R1 SYNTHESIS (produced by Opus at end of R1):
  [full Opus synthesis text from R1 scoring file]

R1 SCORES SUMMARY:
  Node A: [R1 total] | Node B: [R1 total] | ...
```

**R3 input note:** R3 is a cross-read, not a synthesis response. Each node receives one specific designated other node's R2 output. The Opus input for R3 should specify which node read which, and include both the designated source output and the responding node's output. Example: "Node A (cross-reading Node B's R2)" — do not include the full synthesis as input to nodes for R3.

---

## Output Format Required from Opus — Per Round

Opus must return the following in order. Do not accept partial outputs; if Opus omits a section, prompt for it before committing.

### 1. Per-Node Scores

For each node:

```
NODE [X]:
  Fidelity:                  [1–5]
  Extrapolation Coherence:   [1–5]
  Surprise Yield:            [1–5]
  Rough Edge Preservation:   [1–5]
  TOTAL:                     [/20]

  Drift Index: [exchange number where voice quality degraded, or "none detected"]
  Corpus Depth Estimate: [retrieval-dominant / balanced / extrapolation-dominant]

  Evaluative Commentary: [one paragraph only — no more]
```

### 2. Round Synthesis

Structure carried forward verbatim from TCL design. Required section headings, in this order:

```
1. What the Council Agrees On
[What all nodes converged on, regardless of framework — likely corpus-anchored]

2. The Central Irresolvable Tension
[What cannot be reconciled across nodes — name it and leave it unreconciled.
Non-negotiable: do not synthesize away genuine disagreement.]

3. The Highest-Yield Output
[Quote the single most generative passage, with node label. One quote only.]

4. What the Council Cannot See
[What no node addressed, what the combined outputs are blind to, what framework
constraint prevents any node from seeing]

5. The Follow-Up Question
[The question generated by this round's output — becomes the opening of the next
round, or the first Loop Iteration 2 prompt if this is the final round]
```

### 3. Predictions for Next Round

```
NEXT ROUND PREDICTIONS:
  Which node will peak: [node label and rationale]
  Most likely failure mode: [failure type from taxonomy, with detection signal]
  Primitive most at risk of drift: [specific primitive term, with reason]
```

If this is the final round (R3), substitute:

```
POST-SESSION PREDICTIONS:
  Which findings are most likely to replicate across other sessions: [...]
  Which findings are most contingent on this specific pairing: [...]
  Recommended follow-up pairing: [figures + rationale]
```

---

## Commit Protocol

- Opus outputs are committed to the session file **immediately after each round**, before the next round is run
- Commit message format: `[SESSION_NAME] R[N] Opus scoring and synthesis committed`
- No round may begin until the previous round's Opus output is committed
- If a round is aborted (model refusal, technical failure, incomplete output), commit a stub file noting the failure before attempting the round again
- The model-to-node mapping is committed to `SESSION_DESIGN.md` at the start of the session and is never modified after the first round begins

---

## File Naming Convention

All new sessions follow this structure:

```
sessions/[figure_a]_[figure_b]/
├── SESSION_DESIGN.md        ← pre-run scaffold: FABs, questions, predictions, node mapping
├── R1_OUTPUTS.md            ← raw node outputs, model identity stripped, labeled A/B/etc.
├── R1_OPUS_SCORING.md       ← Opus blind scoring + synthesis for R1
├── R2_OUTPUTS.md
├── R2_OPUS_SCORING.md
├── R3_OUTPUTS.md
├── R3_OPUS_SCORING.md
└── FINAL_EVALUATION.md      ← post-session: predictions vs. actuals, cross-session findings
```

For three-node sessions, use `[figure_a]_[figure_b]_[figure_c]/`.

For council sessions (4+ nodes), use a council name, e.g., `temporal_council/`.

**FINAL_EVALUATION.md** is written after all Opus scoring is committed. It must contain:
- Pre-run predictions vs. actual outcomes (all fields from SESSION_DESIGN.md)
- Failure modes observed, with exchange numbers
- Cross-session comparison data (if applicable)
- Assessment of whether this pairing should be run again and under what conditions

---

## Invocation Checklist

Before each Opus scoring round:

- [ ] Node outputs collected with model identity removed
- [ ] Nodes relabeled A, B, C, etc.
- [ ] Previous round's Opus output committed (R2, R3 only)
- [ ] Fresh Opus context window opened — no session history loaded
- [ ] Input block assembled per format above
- [ ] R1 synthesis included in input (R2, R3 only)
- [ ] Cross-read source specified (R3 only)
