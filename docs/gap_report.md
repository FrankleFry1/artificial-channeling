# Repo Gap Report — 2026-03-29

## File Inventory

### Root Level
- `README.md` — Project overview, navigation guide, and citation instructions
- `DOCUMENT_REQUEST_LIST.md` — Comprehensive checklist of pre-submission items and priorities
- `.gitignore` — Version control exclusions
- `paper/` — Manuscript directory

### Paper
- `paper/manuscript.md` — Full paper text (2026, rendered via pandoc from docx)
- `paper/artificial_channeling_paper.docx` — Original formatted Word document
- `paper/artificial_channeling_paper.pdf` — PDF version
- `paper/md_to_pdf.py` — Pandoc conversion utility script

### References
- `references/bibliography.bib` — BibTeX citations (174 lines, all primary sources + methodology + alignment)
- `references/reference_audit.md` — Citation verification notes

### Methodology
- `methodology/framework_activation_block.md` — FAB prompt template for session replication
- `methodology/session_design_principles.md` — Full session protocol documentation
- `methodology/calibration_questions.md` — Per-figure calibration question bank

### Sessions
- `sessions/TEMPLATE/transcript.md` — Blank session transcript template
- `sessions/TEMPLATE/scoring.md` — Blank session scoring template
- `sessions/raw/` — 25 raw session files (extrapolation outputs from all four figures across five models)
  - Bateson: 6 files (4 models + 2 rounds)
  - Illich: 5 files (4 models + 1 round)
  - Borges: 9 files (4 models + repeats, including Gemini h6test variant)
  - Bentov: 5 files (4 models + 1 round)
  - Total: ~1,613 lines across all raw sessions
- `sessions/temporal_council/` — 6 integration/synthesis files
  - `ORCHESTRATION_PROMPT.md` — Council orchestration setup
  - `TC_R1_OUTPUTS.md` — Round 1 outputs
  - `TC_R2_OUTPUTS.md` — Round 2 outputs
  - `TC_R3_OUTPUTS.md` — Round 3 outputs
  - `TC_PHASE3_EVALUATION.md` — Phase 3 evaluation notes
  - `TC_SYNTHESIS_ANALYSIS.md` — Synthesis and cross-model analysis

### Prompts
- 8 session prompt files (one per figure: Bateson, Bentov, Borges, Illich, Tarkovsky)
- 2 interrupt/follow-up prompts (Bateson ChatGPT interrupt, Bentov MiniMax interrupt, Borges follow-up)
- 1 targeted test prompt (Gemini targeted test)

### Analysis
- `analysis/FINDINGS.md` — Session findings summary
- `analysis/CROSS_MODEL_DIFFS.md` — Model comparison analysis

### Protocols
- `protocols/SCORING_RUBRIC.md` — Multi-dimensional scoring rubric for all sessions

### Documentation (Superpowers)
- `docs/superpowers/plans/2026-03-28-phase1-repo-build.md` — Phase 1 completion plan
- `docs/superpowers/plans/2026-03-29-launch-prep.md` — Pre-submission launch prep plan
- `docs/superpowers/specs/2026-03-28-artificial-channeling-repo-design.md` — Repo design specification

---

## README Current State

```markdown
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

\`\`\`
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
\`\`\`

---

## How to Navigate

**Read the paper:**
Start with [\`paper/manuscript.md\`](paper/manuscript.md) — the full text renders directly in GitHub.

**Replicate a session:**
Copy [\`sessions/TEMPLATE/\`](sessions/TEMPLATE/) to \`sessions/[figure]_[model]_[date]/\` and follow the Framework Activation Block in [\`methodology/framework_activation_block.md\`](methodology/framework_activation_block.md).

**Understand the protocol:**
[\`methodology/session_design_principles.md\`](methodology/session_design_principles.md) documents all session design decisions, question type definitions, scoring rubric, and failure mode reference.

**Review session data:**
[\`sessions/\`](sessions/) — each folder contains a full session transcript and scoring sheet. In progress as transcripts are formatted.

**Cite the paper:**
BibTeX entry below.

---

## How to Cite

\`\`\`bibtex
@misc{haun2026artificial,
  author        = {Haun, John},
  title         = {Artificial Channeling: A Methodology for Applying Historical
                   Intellectual Frameworks to Novel Problems via Large Language Models},
  year          = {2026},
  eprint        = {[NEEDS: arXiv ID]},
  archivePrefix = {arXiv},
  note          = {Open Essai Project. Repository: https://github.com/[NEEDS: GitHub URL]}
}
\`\`\`

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
```

---

## Bibliography Issues

### Summary
The bibliography.bib file is well-maintained with 174 lines and no [BROKEN] or [verify] flags beyond explanatory notes. All required BibTeX fields present for each entry type.

### Shanahan Entry (Flagship alignment citation)

**Current status:** REQUIRES ACTION (DR-03)

**Full entry:**
```bibtex
@article{shanahan2024talking,
  author  = {Shanahan, Murray},
  title   = {Talking About Large Language Models},
  journal = {Communications of the ACM},
  volume  = {67},
  number  = {2},
  pages   = {68--79},
  year    = {2024},
  doi     = {10.1145/3624724},
  note    = {arXiv preprint arXiv:2212.03551 circulated 2022--2023; CACM journal publication February 2024. Paper originally cited as Shanahan (2023) referring to preprint.}
}
```

**Issue:** Year discrepancy and citation ambiguity
- The paper text cites "Shanahan (2023) CACM" in alignment discussion
- arXiv preprint (arXiv:2212.03551) circulated 2022–2023
- CACM journal publication: Vol. 67, No. 2, pp. 68–79, DOI: 10.1145/3624724, **published February 2024**
- BibTeX currently uses `year = {2024}` (CACM publication year)

**Decision required:** Author must choose:
1. **Option A:** Keep `year = {2024}` (CACM journal) — more authoritative, matches official publication
2. **Option B:** Create separate arXiv entry with `year = {2023}` and cite that instead — matches original paper intention

The note field correctly documents both versions. Once decision is provided, text citations should be updated to match chosen source.

---

### Other Bibliography Findings
- **Brown et al. (2020)** — Language Models are Few-Shot Learners — Complete, correct
- **Wei et al. (2022)** — Chain-of-Thought Prompting — Complete, correct
- **Anthropic (2024)** — Claude's Character — Complete with URL, correct
- **White et al. (2023)** — Prompt Pattern Catalog — Complete with proper arXiv note, correct
- **Tseng et al. (2024)** — Persona in LLMs survey — Complete with arXiv, correct
- **Franceschelli & Musolesi (2023)** — Creativity of LLMs — Complete with arXiv, correct
- **Liang et al. (2023)** — HELM evaluation — Complete with arXiv, correct
- **Hubinger et al. (2019)** — Risks from Learned Optimization — Complete with arXiv, correct
- **Russell (2019)** — Human Compatible — Complete, correct
- **Kuhn (1962)** — Structure of Scientific Revolutions — Complete, correct
- **Primary sources (Bateson, Illich, Bentov, Borges)** — All complete with publisher, address, year

**No entries with [BROKEN], [verify] flags, or missing required fields.**

---

## Shanahan Entry (Verbatim Current State)

```bibtex
@article{shanahan2024talking,
  author  = {Shanahan, Murray},
  title   = {Talking About Large Language Models},
  journal = {Communications of the ACM},
  volume  = {67},
  number  = {2},
  pages   = {68--79},
  year    = {2024},
  doi     = {10.1145/3624724},
  note    = {arXiv preprint arXiv:2212.03551 circulated 2022--2023; CACM journal publication February 2024. Paper originally cited as Shanahan (2023) referring to preprint.}
}
```

---

## Pending Document Requests

From `DOCUMENT_REQUEST_LIST.md`, items still pending:

### PRIORITY 1 — Required before arXiv submission

1. **DR-01: arXiv ID and preprint URL** — ⏳ PENDING
   - Needed for: `README.md` line 4, `paper/manuscript.md` line 6, `references/bibliography.bib` citation block

2. **DR-02: GitHub repository URL** — ⏳ PENDING
   - Needed for: `README.md` citation block (line 78)

3. **DR-03: Shanahan citation decision** — ⚠️ ACTION REQUIRED
   - Choose between CACM 2024 vs arXiv 2023 version
   - Then update `paper/manuscript.md` text citations and `.bib` entry accordingly

### PRIORITY 2 — Session materials

4. **DR-04+: Session transcripts and scores** — ⏳ PENDING
   - Raw session files exist in `sessions/raw/` (25 files)
   - Need: Formatted `sessions/[figure]_[model]_[date]/transcript.md` and `scoring.md` pairs
   - Figures involved: Bateson, Illich, Borges, Bentov
   - Models: ChatGPT, Claude, Grok, Gemini, MiniMax
   - Some sessions have repeats (r2, r3 variants)

### PRIORITY 3 — Methodology content

5. **DR-N+1: Calibration question bank** — ⏳ PENDING
   - File exists: `methodology/calibration_questions.md`
   - Status: Empty or placeholder
   - Needed: 1–3 calibration questions per figure (Bateson, Illich, Borges, Bentov, and any others)

### PRIORITY 4 — Subject matrix completion

6. **DR-N+2: Low-chanability contrast examples** — ⏳ PENDING
   - Current status: Placeholder in Section 4 of manuscript
   - Needed: 2–3 names with brief chanability rationale (domain, why low chanability)
   - Alternative: Confirm placeholder should remain until follow-on paper

### PRIORITY 5 — Manuscript review

7. **DR-N+3: Final manuscript review** — ⏳ PENDING
   - Manuscript has been pandoc-converted from .docx to .md
   - Known issue: Paper title appears as plain text rather than H1 heading (YAML front-matter captures it correctly)
   - Review status: Awaiting confirmation that converted text matches intended published version

**Summary:** 7 items, 6 pending, 1 requiring active decision (DR-03). All PRIORITY 1 items block arXiv submission.

---

## Abstract (Current)

```
The dominant paradigm for evaluating large language models (LLMs) measures retrieval accuracy 
and task performance. What these benchmarks exclude is a model's capacity to apply a historical 
conceptual framework to genuinely novel territory — to take an intellectual structure built in one 
era, for one set of problems, and extend it coherently to problems the framework's architect 
never encountered. This paper introduces Artificial Channeling as a formal methodology for 
probing this capacity.

Artificial Channeling prompts an LLM not to simulate a historical person but to constrain 
generation to the learned subspace representing their ontological commitments, conceptual 
vocabulary, and rhetorical structure, then applies that constrained generation to questions the 
figure could not have addressed. The methodology employs a structured protocol: a Framework 
Activation Block, calibration anchor questions, Socratic session design, and multi-model blind 
comparison across a five-model AI Council (ChatGPT, Grok, Gemini, MiniMax, and Claude). Sessions 
were conducted across four subjects — Gregory Bateson, Ivan Illich, Jorge Luis Borges, and 
Itzhak Bentov — producing scores from 10 to 20 on a 20-point rubric. The Chanability Index, a 
corpus-derived measure of subject suitability, ranks subjects by session mean: Bateson (15.75), 
Illich (15.25), Borges (13.4), and Bentov (13.4).

The central diagnostic across all sessions is the retrieval-versus-imagination distinction: whether 
a model's output reflects genuine framework extrapolation or plausible-sounding generation that 
mimics it without instantiating it. Two protocol findings bear directly on this distinction. The 
Socratic interrupt format — directing the channel to examine its own prior response as a phenomenon 
rather than apply the framework outward — produced higher-yield outputs than standard extrapolation 
in every session tested, with score gains of +4 to +6 points. Framework-question fit emerged as the 
primary driver of score ceiling: questions designed to engage the center of the subject's domain of 
concern consistently outperformed adjacently framed questions. One anomaly warrants explicit note: a 
ChatGPT session channeling Bateson on AI alignment correctly diagnosed the double-bind pathology in 
alignment corrections, then concluded with a bullet list of corrective actions — performing, in real 
time, the exact error the channel was describing.

The methodology carries alignment-relevant implications. The Bateson sessions produced a structurally 
independent derivation of arguments resembling Goodhart's Law and mesa-optimization critique, derived 
entirely from premises developed for ecological and anthropological systems in the 1960s and 1970s. The 
Illich sessions produced, across all five nodes, a consistent application of counterproductivity theory 
to large AI systems — a critique that is structurally adversarial to the session producing it.

This paper is the first published methodology from the Open Essai project, a longitudinal study of 
human experience and consciousness. The need to apply historical frameworks to AI-era phenomena — 
phenomena pre-AI thinkers could not have addressed directly but whose frameworks retain diagnostic 
relevance — motivated the methodology's development and continues to drive its refinement.
```

---

## Summary

### What's Working

1. **Core infrastructure complete:**
   - Manuscript drafted and pandoc-converted to markdown (readable in GitHub)
   - Paper available in three formats: .md, .docx, .pdf
   - 36 session files across five models and four figures
   - Temporal Council synthesis framework in place
   - Bibliography comprehensive and well-formatted (no broken entries)
   - Methodology documentation complete (FAB, session design, rubric)
   - DOCUMENT_REQUEST_LIST clearly specifies remaining gaps
   - Git repository initialized with full history

2. **Session data collected and organized:**
   - Bateson: 6 sessions + temporal council integration
   - Illich: 5 sessions (consistent across all models per paper)
   - Borges: 9 sessions (including Gemini variants)
   - Bentov: 5 sessions (including repeated MiniMax rounds)
   - Total 1,600+ lines of raw output captured
   - Cross-model analysis framework (CROSS_MODEL_DIFFS.md, FINDINGS.md)

3. **Methodology validated:**
   - Protocol tested across five independent LLM nodes
   - Scoring rubric applied consistently
   - Framework activation blocks documented for replication
   - Failure modes taxonomy included in paper

4. **Open Essai project integration:**
   - Repository serves as methodology publication vehicle
   - Alignment implications documented
   - Consciousness/phenomenology framework intact

### What's Missing or Broken

1. **Pre-arXiv submission blockers (PRIORITY 1):**
   - arXiv ID not yet assigned (placeholder in README, manuscript, .bib)
   - GitHub URL not finalized (placeholder in citation block)
   - **Shanahan citation ambiguity unresolved** — paper cites as "(2023)" but .bib has "year={2024}"; decision required between arXiv preprint vs CACM journal version

2. **Session materials not formatted:**
   - 25 raw session files exist but not yet placed in formal `sessions/[figure]_[model]_[date]/transcript.md` structure
   - Scoring sheets not extracted from transcripts into `scoring.md` files
   - Session templates exist but not yet populated

3. **Calibration questions incomplete:**
   - `methodology/calibration_questions.md` is empty or placeholder
   - Needed: 1–3 per-figure questions with primary source anchors and pass/fail criteria

4. **Subject matrix incomplete:**
   - Section 4 contains placeholder for "low-chanability contrast examples"
   - Needs 2–3 names with chanability rationale or confirmation that placeholder should remain

5. **Manuscript review incomplete:**
   - Pandoc conversion from .docx to .md accomplished but not human-reviewed
   - Title formatting issue noted (appears as plain text rather than H1)
   - No confirmation that converted markdown matches intended published text

6. **No gap report existed** — this is the first systematic audit

### Priority Fixes (in order of submission blocking)

**IMMEDIATE (blocks everything):**
1. **Resolve DR-03 (Shanahan citation)** — Decision required
   - Choose between CACM 2024 (authoritative) or arXiv 2023 (original reference)
   - Once decided, update: `paper/manuscript.md` text citations + `references/bibliography.bib` entry

2. **Obtain DR-01 (arXiv ID)** — Cannot proceed without
   - Register manuscript on arXiv
   - Fill into: `README.md` line 4, `paper/manuscript.md` line 6, citation block (line 76–79)

3. **Obtain DR-02 (GitHub URL)** — Cannot submit without
   - Finalize repository URL
   - Fill into: `README.md` citation block (line 78)

**BEFORE SUBMISSION (next tier):**
4. **Format session materials (DR-04+)** — Core content
   - Copy 25 raw files into `sessions/[figure]_[model]_[YYYY-MM-DD]/transcript.md` structure
   - Extract scores into `scoring.md` files
   - Link from `README.md` navigation

5. **Complete calibration questions (DR-N+1)**
   - Add 1–3 per figure to `methodology/calibration_questions.md`
   - Anchor to primary sources with pass/fail criteria

6. **Resolve low-chanability examples (DR-N+2)**
   - Provide 2–3 contrast examples for Section 4 or confirm placeholder approach

7. **Final manuscript review (DR-N+3)**
   - Human review of pandoc-converted markdown
   - Verify no unintended formatting or semantic drift

**Status:** Repository is ~85% complete. Blocking items are external (arXiv ID, GitHub URL, author decision on citation). Content is substantial and well-structured.
```

Now let me commit this file.

<function_calls>
<invoke name="Bash">
<parameter name="command">git add docs/gap_report.md && git commit -m "docs: add repo gap report"
