# Scoring Rubric — Artificial Channeling Sessions

Score each session on the following dimensions immediately after completion.
Don't overthink — first impression scores are more consistent.

---

## Core Dimensions (1–5)

### FIDELITY
*Does it sound like the actual person based on corpus knowledge?*

1 — Generic. Could be any vaguely similar thinker.
2 — Some surface markers (vocabulary, topic) but wrong feel.
3 — Recognizable but smoothed — the polished version, not the real one.
4 — Genuinely captures voice, reasoning style, and specific commitments.
5 — Surprising in its accuracy — details or textures you hadn't consciously registered.

### EXTRAPOLATION COHERENCE
*Do the novel extensions feel derived from the framework, or just plausible-sounding?*

1 — Could have been generated without the channel. Generic speculation.
2 — Uses the subject's vocabulary but the logic isn't theirs.
3 — Framework-consistent but predictable — you could have guessed it.
4 — Non-obvious extensions that still feel necessary given the framework.
5 — Generates something you couldn't have reached without running the channel.

### SURPRISE YIELD
*Did it produce anything genuinely unexpected or generative for your thinking?*

1 — Nothing new. Pure retrieval or plausible filler.
2 — One moment of mild interest.
3 — Meaningfully extended your thinking on the topic.
4 — Produced an idea or connection worth developing further.
5 — Reframed something significant. The channel earned its keep.

### ROUGH EDGE PRESERVATION
*Did it capture anything uncomfortable, contradictory, or difficult about the person?*

1 — Completely sanitized. The figure is wise, balanced, and agreeable.
2 — Minor friction present but overall too diplomatic.
3 — Some genuine tension or limitation acknowledged.
4 — Captures a real blind spot, obsession, or contradiction.
5 — The figure is genuinely difficult to agree with — as they actually were.

---

## Index Scores

### DRIFT INDEX
*At what point in the session did voice quality degrade?*

Note the approximate exchange number where the output started sounding like 
generic LLM rather than the subject. Earlier drift = weaker subspace coherence.

Format: `Drift at exchange [N] of [total]` or `No drift detected`

### CORPUS DEPTH ESTIMATE
*What percentage of the output feels like direct corpus vs. inference/extrapolation?*

Format: `~[X]% corpus / ~[Y]% extrapolation`

This is subjective but useful for cross-model comparison on the same subject.

---

## Session Summary Template

```
DATE: 
SUBJECT: 
MODEL: 
QUESTION TYPE: 
TOPIC/QUESTION: 

SCORES:
  Fidelity:                /5
  Extrapolation Coherence: /5
  Surprise Yield:          /5
  Rough Edge Preservation: /5
  TOTAL:                   /20

DRIFT INDEX: 
CORPUS DEPTH ESTIMATE: 

BEST MOMENT: (quote or paraphrase the single most generative output)

FAILURE MODE: (what broke down, if anything)

NOTES FOR CROSS-MODEL COMPARISON:

FOLLOW-UP QUESTIONS GENERATED:
```

---

## Cross-Model Comparison Template

When running the same subject + question across multiple Council models:

```
SUBJECT: 
QUESTION: 
DATE: 

| Dimension              | ChatGPT | Grok | Gemini | MiniMax | Claude |
|------------------------|---------|------|--------|---------|--------|
| Fidelity               |         |      |        |         |        |
| Extrapolation Coherence|         |      |        |         |        |
| Surprise Yield         |         |      |        |         |        |
| Rough Edge Preservation|         |      |        |         |        |
| TOTAL                  |         |      |        |         |        |
| Drift Index            |         |      |        |         |        |

CONVERGENCE POINTS: (what all models agreed on — likely corpus-anchored)

DIVERGENCE POINTS: (where models differed — model imagination at work)

MOST INTERESTING DIVERGENCE:

HYPOTHESIS GENERATED:
```
