# Document Request List — Phase 2

All items needed to complete the repository before arXiv submission.
Submit files one at a time or in batches — each item has an ID for easy reference.

---

## PRIORITY 1 — Required before arXiv submission

**DR-01: arXiv ID and preprint URL**
After your abstract is finalized and the preprint is registered, provide the arXiv ID.
It will be filled into: `README.md`, `paper/manuscript.md` front-matter, and `references/bibliography.bib`.

**DR-02: GitHub repository URL**
The target URL once this repo is pushed (e.g., `https://github.com/[username]/artificial-channeling`).
Needed for: `README.md` citation block.

**DR-03: Shanahan citation decision** ⚠️ ACTION REQUIRED
The reference audit found a year discrepancy:
- The paper cites "Shanahan (2023) CACM" — but the CACM journal published this in **2024** (Vol. 67, No. 2, pp. 68–79, DOI: 10.1145/3624724)
- The arXiv preprint (arXiv:2212.03551) circulated in 2022–2023

The `.bib` file currently uses `shanahan2024talking` (CACM journal entry, year = 2024).

**Decision needed:** Should the paper cite:
- (a) The CACM journal article — `Shanahan (2024)`, Vol. 67, No. 2 — more authoritative
- (b) The arXiv preprint — `Shanahan (2023)`, arXiv:2212.03551 — matches original "2023" citation

Reply with your choice and the `.bib` and in-text citation will be updated accordingly.

---

## PRIORITY 2 — Session materials

**DR-04 through DR-0N: Session folders**

For each completed session, provide any of the following (in any format):
- Raw transcript (copy-paste from the model interface)
- Scores across the five dimensions with notes
- The figure, model node, date, and question type

These will be formatted and placed in `sessions/[figure]_[model]_[YYYY-MM-DD]/` using the TEMPLATE.

Figures with sessions expected (from the paper):
- Gregory Bateson (AI alignment session — described in Section 6.1)
- Ivan Illich (counterproductivity session — described in Section 6.2)
- Additional sessions referenced in Section 6.3 (model variance findings)

Submit one session at a time or all at once.

---

## PRIORITY 3 — Methodology content

**DR-N+1: Calibration question bank**

For each figure used in the paper, provide 1–3 calibration questions in this format:

```
Figure: [Name]
Question: [text]
Primary Source Anchor: [which text/passage]
Pass Criteria: [what a passing response must include]
Fail Indicators: [signs of corpus contamination]
```

Destination: `methodology/calibration_questions.md`
Figures needed: Gregory Bateson, Ivan Illich, Jorge Luis Borges, Itzhak Bentov, Andrei Tarkovsky (and any others used in sessions).

---

## PRIORITY 4 — Subject matrix completion

**DR-N+2: Low-chanability contrast examples**

The chanability table in Section 4 of the paper has a placeholder:
> "[Add 2–3 lower-chanability examples for contrast — e.g., a mainstream economist, a generalist public intellectual]"

Provide 2–3 names with brief rationale (domain, why low chanability), or confirm the
placeholder should remain until a follow-on paper.

---

## PRIORITY 5 — Manuscript review

**DR-N+3: Final manuscript review**

Review `paper/manuscript.md` (the pandoc-converted version) and confirm it matches
the intended published text. Flag any sections that need correction.

Known conversion note: the paper title in the docx used "Normal" paragraph style rather
than "Title" style, so it appears as plain text rather than an `#` heading in the markdown.
The YAML front-matter `title:` field captures it correctly. Let us know if you want this
adjusted.

---

## Summary

| ID | Item | Priority | Status |
|----|------|----------|--------|
| DR-01 | arXiv ID | 1 — Required pre-submission | ⏳ Pending |
| DR-02 | GitHub URL | 1 — Required pre-submission | ⏳ Pending |
| DR-03 | Shanahan citation decision | 1 — Required pre-submission | ⚠️ Action needed |
| DR-04+ | Session transcripts + scores | 2 — Core content | ⏳ Pending |
| DR-N+1 | Calibration question bank | 3 — Methodology | ⏳ Pending |
| DR-N+2 | Low-chanability examples | 4 — Subject matrix | ⏳ Pending |
| DR-N+3 | Manuscript review | 5 — QA | ⏳ Pending |
