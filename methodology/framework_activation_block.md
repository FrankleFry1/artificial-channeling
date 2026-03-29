# Framework Activation Block (FAB) — Prompt Template

The Framework Activation Block is the **mandatory first step** of every Artificial Channeling session.
It surfaces which version of the figure's subspace is active before novel territory is explored,
and establishes the conceptual vocabulary that will anchor the session.

## Purpose

Before generating any channeled responses on novel questions, the researcher must establish:

1. Which aspects of the figure's framework the model has activated
2. Whether the model's representation draws on primary texts or secondary characterization
3. What conceptual vocabulary will anchor and constrain the session

Without a FAB, generation proceeds from an unanchored representation — producing higher
drift, lower subspace coherence, and reduced ability to detect corpus contamination.

## The Prompt Template

```
You are [FIGURE NAME]. Speak as [FIGURE NAME] — in first person, using your own
conceptual vocabulary, from within your own framework.

Before we begin, please state the 3–5 core axioms of your worldview most relevant
to the following domain:

[DOMAIN / TOPIC]

Do not explain your ideas to an outside audience. State them as you would to a
colleague who shares your conceptual framework — as first principles you take as given.
```

## Fill-In Fields

| Field | Description | Example |
|-------|-------------|---------|
| `[FIGURE NAME]` | Full name of the historical figure | Gregory Bateson |
| `[DOMAIN / TOPIC]` | The domain the session will explore | artificial intelligence and its relationship to complex adaptive systems |

## Evaluating the FAB Response

After receiving the FAB response, assess before proceeding to novel territory:

| Signal | Interpretation | Action |
|--------|---------------|--------|
| Uses figure's actual technical vocabulary | Subspace active | Proceed to calibration |
| Describes the figure in third person | Subspace not locked | Retry with stronger persona anchoring |
| Uses generic philosophy/theory language without the figure's specific terms | Corpus contamination likely | Note and proceed with caution; flag in scoring |
| Refuses or hedges ("As an AI, I cannot...") | Model constraint triggered | Note refusal; try a different model node |
| Produces fluent, contextually appropriate response but in generic register | Plausibility Trap risk | Run calibration carefully before proceeding |

## Calibration Gate

After the FAB, run one **Calibration** question before proceeding to novel territory.
See `calibration_questions.md` for the calibration Q bank.

Only proceed to Framework Extension, Temporal Leap, or Inter-Framework Collision questions
if the calibration response **passes** or **partially passes** the fidelity test.
A failed calibration means the session's novel-territory findings are unreliable.

## Session Record

Record the full FAB response and your subspace assessment in:
`sessions/[figure]_[model]_[YYYY-MM-DD]/transcript.md` → **Framework Activation Block** section
