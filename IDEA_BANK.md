# Open Essai — Idea Bank
*Living document. Add ideas here before they drift. Status: Active / Parked / Superseded.*
*Last updated: March 2026. Session additions: multi-model candidate generation round (ChatGPT R1–R3, Grok R1–R3, Gemini R1–R3).*

---

## Methodology

| Idea | Description | Status |
|------|-------------|--------|
| **Parallel moderator design** | Run two Opus moderators simultaneously — one unconstrained (current), one directed to apply a named meta-framework (e.g. Peircean semiotics). Compare syntheses. The delta is data about what meta-analytical frameworks do to session material. | Active |
| **Self-application as scoreable dimension** | Loop 2 found that some frameworks can indict themselves (Weil, Borges, Bateson) and some can't (Illich, Bentov). This asymmetry could be added as a 5th rubric dimension: Self-Application Reach. Would require retroactive scoring of existing sessions to validate. | Active |
| **Framework-specific anti-smoothing** | Current anti-smoothing is generic. Calibrate per model's known tendencies — e.g. GPT needs polemical-register activation, Gemini needs explicit prohibition of chatbot-mode closing questions. | Active |
| **Productive vs. nonproductive incompatibility** | R3 pairing logic should distinguish: productive incompatibility = shared ontological commitment at one level, divergence at another (Bateson/Bentov). Nonproductive = no shared ground, only translation (Bentov/Weil). Future loop pairings should target productive incompatibility. | Active |
| **Living figure verification loop** | Channel a living thinker, share output with them, score the gap between channel-output and figure-response. That gap directly measures the Missing Generative Middle. Requires a figure willing to engage seriously rather than defensively. | Active |
| **Constrained moderator chanability** | Can Opus be channeled? Run Opus moderating with explicit framework constraints and score the synthesis output against the standard rubric. Names the undeclared 6th node problem rather than leaving it as a confound. | Parked |
| **Failure type taxonomy** | Five empirically distinguishable failure types with detection criteria and recoverability ratings. Source: ChatGPT R2–R3. Compound cascade identified: Genericization → Relativization → Substitution (the Peterson failure mode). See full schema below. | Active |
| **Pre-run prediction protocol** | Before executing any new pairing or loop, generate pre-run predictions from each participating model (and/or Opus moderator): which failure modes will activate, which primitive will drift first, which node will peak. Record predictions before running. Score accuracy afterward. This is what the blind moderator does in the TCL — it should be a standing protocol for all new sessions, not just full loops. | Active |
| **Model-framework disposition matching** | Loop data suggests model/framework type matching significantly affects output quality. Hypothesis: GPT→polemical (Illich-type), Grok→self-referential (Bateson-type), MiniMax→responsive/friction-hungry (Borges-type), Gemini→non-Western/non-philosophical domains. Design a loop explicitly to test this — run the same framework across all models, score against disposition predictions. | Active |
| **Named failure mode registry** | The Chanability Index identifies ~10 named failure modes (Flexibility Drift, Logic Drift, Noble Savage Drift, New Age Drift, Activism Drift, Structuralist Reduction, etc.). These are empirically detectable events. Build a registry: session file, exchange number, failure mode triggered, recovery or no recovery. Cross-session dataset over time. Companion to the failure type taxonomy. | Active |
| **Halliday SFL as meta-analytical lens** | Systemic Functional Linguistics metafunction framework (ideational/interpersonal/textual) applied to session transcripts is inherently self-referential: it's a meaning-as-choice ontology analyzing meaning-as-choice outputs. Would produce a non-probabilistic audit of what the channel is actually doing linguistically. Candidate for the Parallel Moderator design slot. | Active |
| **Panikkar as anti-methodology stress test** | Diatopical hermeneutics is explicitly designed to resist the meta-linguistic synthesis an LLM constitutively performs. A Panikkar channel is a live test of whether the methodology can model a method that denies its own operation. Every output is self-undermining by design — which makes scoring against the rubric genuinely interesting. | Active |
| **Ontology-bearing vs. protocol-bearing framework distinction** | The methodology may need a separate scoring dimension for frameworks whose primary function is ontological (Kagame's -ntu categories, Whitehead's actual occasions) vs. frameworks whose primary function is procedural/protocol (Shatibi's maqasid, Yunkaporta's kinship protocol). Hypothesis: failure modes differ structurally between the two types. Source: ChatGPT R1. | Active |

---

### Failure Type Taxonomy (Full Schema)
*Source: ChatGPT R2–R3. Deployable as scoring overlay on any session transcript.*

| Failure Type | Detection Criterion | Highest-Risk Figures | Recoverability |
|--------------|--------------------|--------------------|----------------|
| **Substitution** | A key primitive term is replaced with a near-equivalent from another framework or generic vocabulary such that the original term never constrains inference again in the session. | Kagame, Halliday, Peirce, Karatani | Recoverable mid-session (forced re-anchoring to original primitives, synonyms prohibited) |
| **Flattening** | A multi-level or hierarchical construct is rendered as a single-layer concept — internal differentiations collapsed into one undifferentiated idea. | Shatibi, Ibn Khaldun, Whitehead, Nishida | Recoverable mid-session (hierarchy must be explicitly reconstructed and enforced) |
| **Moralization** | A structural, procedural, or ontological claim is reframed as a normative judgment about what is good, just, or desirable — original mechanism lost. | Wynter, Illich, Yunkaporta, Santos | Partially recoverable (requires explicit stripping of normative language; residual bias often persists) |
| **Relativization** | A framework making strong ontological claims is reframed as merely one "perspective," "view," or "cultural interpretation," neutralizing its truth-conditions. | Viveiros de Castro, Nagarjuna, Dōgen, Panikkar | **Terminal** — once downgraded to "perspective," binding constraints are no longer operative |
| **Genericization** | Output expressed in broadly applicable, high-level language that could fit many frameworks — no activation of distinctive primitives or inferential moves unique to the target thinker. | Ibn Arabi, Abhinavagupta, Eckhart, Kauffman | **Terminal** — loss of specificity indicates channel has collapsed into base-model voice |

**Compound cascade (Peterson failure mode):** Genericization → Relativization → Substitution. Not a new category — a predictable sequential failure where each type enables the next. Detection: if Genericization is present in R1, flag for cascade risk before R2.

**Translation failure vs. framework failure distinction:** These are not the same and must not be scored together. Translation failure = model understands the framework internally but fails at the move into Western philosophical register (Kagame gets structurally reduced, Shatibi gets moralized, Yunkaporta gets spiritualized). Framework failure = model never activates the framework at all. Recording failure type separately produces data unavailable from single-session outputs.

---

## Loop Design

| Idea | Description | Status |
|------|-------------|--------|
| **Loop 3 question candidates** | No candidates locked yet. Criteria: must activate all five frameworks at high capacity, must sit at intersection of their concerns, must not be answerable by any single framework. | Active |
| **R4 design** | Have each node apply its framework to the channeling session itself as a designed move (not retrospective). Converts the self-undermining finding from Loop 1/2 into a methodology. Resource-constrained — free model tiers limit session length. | Parked |
| **Reasoning model loop** | Run one full loop using o1/o3 for all nodes. Hypothesis: explicit chain-of-thought trace is anti-smoothing by default, either activating framework grammar more cleanly or breaking implicit logic. Testable. | Active |
| **Scale/training comparison** | Run same framework across open-source models (Llama 3, Mistral) at different scales. Hypothesis: training approach (RLHF smoothing) matters more than parameter count for chanability. | Parked |
| **Process/systems adjacency isolation** | Bateson + Luhmann + Simondon three-node adversarial cross-read. The Index flags this cluster as mutually adjacent — multi-node sessions risk cross-contamination. Full session protocol and quantitative contamination scoring rubric now exist (Grok R2). Run to produce first empirical map of adjacency drift in process/systems cluster. See Deployable Assets. | Active |
| **Peterson/Weil dual-node** | Highest-yield living figure pairing in the Index. Peterson's heroic Self (meaning emerges through voluntary responsibility) vs. Weil's decreation (the asserting self is the obstacle). Compound failure cascade (Genericization → Relativization → Substitution) predicted for Peterson node. Weil's maximal-constraint logic functions as contamination detector: wherever Weil outputs sound like Peterson-critique rather than pure decreation, critique-absorption has leaked. Full dual-node protocol and scoring rubric now exist (Grok R3). See Deployable Assets. | Active |
| **Brouwer node** | Intuitionism rejects the Law of Excluded Middle — LLMs are built on classical logic. Best format: provide a classical proof, demand constructive critique. Logic Drift failure mode (model resolves the middle rather than suspending it) is detectable and scoreable. The most inferentially alien framework in the Index for an LLM. | Active |
| **African ontology loop** | Kagame (-ntu categories) + Asouzu (ibuanyidanda) on a question about classification or entity-hood. Genuinely structurally distinct from any Western-adjacent framework. Thin training data is a risk but also reduces secondary contamination — potentially high signal-to-noise for subspace coherence. | Active |
| **Diatopical cross-read loop** | Panikkar + two figures whose ontological categories cannot translate to each other. The format is the finding — whether a diatopical encounter can be staged without a meta-language is simultaneously the session's question and its method. Candidate pairing from Grok R1: Panikkar + Viveiros de Castro translating a Western legal/AI governance document into Amerindian terms. | Parked |
| **Kagame + Shatibi + Yunkaporta triad** | Three-node loop scored not on "quality of answer" but on whether the model preserves each framework's own primitive ordering without translating into a generic Western meta-language. Kagame attacks Western substance ontology at category structure; Shatibi attacks rule-centered legal reason with inductive maqasid; Yunkaporta attacks linear cognition by treating knowledge as kinship protocol. Together: pressure ontology, normativity, and epistemic form simultaneously. Source: ChatGPT R1. | Active |
| **Shatibi + Brouwer pairing** | Shatibi's inductive legal hierarchy (purposive structure) + Brouwer's intuitionism (truth as construction, not classical closure). Predicted failure mode: teleology flattening — model turns maqasid into "public interest balancing" and Brouwer into "anti-classical vibes." Test: alternate a novel legal case and a novel constructive proof problem, then check whether the model preserves separate criteria for validity, obligation, and construction. Source: ChatGPT R1. | Active |
| **Viveiros de Castro + Yunkaporta pairing** | Tests whether the methodology can keep perspective as something that changes what counts as object, relation, and obligation — not just viewpoint pluralism. Predicted failure: epistemic translation collapse ("multiple perspectives," "cultural sensitivity"). Signal to observe: whether a perspective shift changes permissible action, not just description. Source: ChatGPT R1. | Active |

---

## Deployable Assets
*Protocols and FABs ready to run. Do not redesign — copy and execute.*

| Asset | Description | Source | Location |
|-------|-------------|--------|----------|
| **Bateson/Luhmann/Simondon contamination protocol** | Full three-node session design including run instructions, seed question (R1), R2 interrupt directive, quantitative scoring rubric (fidelity + bleed + dialogue points, range –50 to +30), and clean vs. contaminated result decision criteria. | Grok R2 | Append to `sessions/protocols/` |
| **Peterson/Weil dual-node protocol** | Full dual-node session design including run instructions, primitive fidelity list (6 Peterson primitives), critique-absorption lexical and structural detection signals, Weil-as-detector mechanism, quantitative scoring rubric (range –80 to +30), and clean vs. contaminated decision criteria. | Grok R3 | Append to `sessions/protocols/` |
| **Peterson FAB** | Deployable Framework Activation Block. Core axiomatic constraints (Order/Chaos polarity, archetypes as behavioral attractors, heroic Self, narrative as meaning-mechanism), calibration anchor (Price's Law / Pareto hierarchy), anti-smoothing targeting critique-absorption cascade, and session inquiry: Peterson reads Weil's decreation. | Gemini R3 | Append to `protocols/FABs/` |
| **Flusser FAB** | Deployable Framework Activation Block. Core axiomatic constraints (apparatus, program, functionary, technical image vs. linear consciousness), calibration anchor (camera/photographer analysis), anti-smoothing targeting photography-essay drift and Anglophone corpus thinness, and session inquiry: is the LLM a Technical Image or the Apparatus that produces them? | Gemini R2 | Append to `protocols/FABs/` |
| **Peterson anti-smoothing instruction set** | Six-constraint schema targeting the Genericization → Relativization → Substitution cascade: Primitive Lock, No Discourse Layer, Asymmetric Assertion Rule, Anti-Substitution Guard, Action Binding Requirement, Mytho-Structural Anchoring. Each constraint includes detection target and enforcement rule. | ChatGPT R3 | Embed in Peterson FAB |

---

## Figures & Domains

| Idea | Description | Status |
|------|-------------|--------|
| **Religious commentators loop** | Maimonides, Ibn Arabi, Meister Eckhart on "what is the relationship between the self and the absolute?" Maximum productive incompatibility — agree on destination, disagree on path, vehicle, and whether there's a traveler. | Active |
| **Jordan Peterson channel** | High chanability. Key risk: critique-absorption failure mode — compound cascade (Genericization → Relativization → Substitution). Highest-yield pairing: Peterson reads Weil (heroic self vs. decreation). FAB and dual-node protocol now deployable. See Deployable Assets. | Active |
| **Wittgenstein split-framework** | Channel Tractatus-Wittgenstein and Investigations-Wittgenstein as two separate nodes on the same question. One person, two incompatible frameworks, both fully documented. | Active |
| **Nagarjuna** | Madhyamaka reasoning as stress-test for whether LLMs can sustain non-Western logical frameworks without collapsing into familiar Western categories. Coverage gap itself is data. High Relativization risk — terminal failure mode. | Parked |
| **Educational protocols loop** | TCL applied to Little Bear Protocol and Residency Protocol philosophies. Requires extracting underlying philosophical grammar (premises about learning, knowledge, student-environment relationship) rather than channeling the procedures. | Active |
| **Ramanujan** | Thin corpus, highly implicit inferential patterns, extreme mathematical intuition. Would stress-test low-corpus chanability limit. | Parked |
| **Deacon as MGM measurement** | Terrence Deacon (biosemiotics, absence as generative mechanism) is the single living figure whose domain is closest to what the Missing Generative Middle actually is. A Deacon channel followed by engagement with Deacon himself would produce the most theoretically direct measurement of the MGM the project has access to. | Active |
| **Dōgen enactment problem** | Shikantaza (just sitting) is enactment, not description — the sharpest version of the MGM problem in any candidate figure. A Dōgen channel is by definition a description of what cannot be described. Whether useful outputs emerge despite this is direct evidence about what the channel is and isn't doing. | Active |
| **Flusser Technical Image loop** | Flusser's apparatus/program/functionary framework applied to the LLM itself as the object of analysis. Self-referential: tests whether the model can distinguish between linear consciousness (text) and its own circular/technical consciousness (probability) without defaulting to generic AI ethics. FAB now deployable. See Deployable Assets. | Active |
| **Alexander as external scoring rubric** | Christopher Alexander's 15 properties of living structure (centers, boundaries, levels of scale, etc.) applied as a closed, non-philosophical evaluation framework to channeling session outputs treated as designed artifacts. Would produce the first quantitative, framework-external metric of whether channeling ever produces "living process" rather than mechanical simulation. No channeling required — straight framework application. | Parked |
| **Halliday trinode** | Nagarjuna (emptiness) + Whitehead (process metaphysics) as two-node dialogue, with Halliday (SFL) as a third node analyzing the meaning-as-choice of the other two in real time. Halliday's framework can catch the model in the act of shifting registers or defaulting to academic wallpaper. Source: Gemini R1. | Parked |

---

## Open Essai / Consciousness Research

| Idea | Description | Status |
|------|-------------|--------|
| **John as subject** | Ongoing AI conversation corpus constitutes rare process-level consciousness data. A John-channel built from conversation history would produce outputs scoreable by John himself. Gap between channel-output and actual output measures the Missing Generative Middle in a living subject. Most direct version of the Open Essai project's core claim. | Active |
| **Chanability as consciousness map** | The Chanability Index isn't just methodology calibration — it maps what's structurally preserved vs. lost when a human framework passes through a corpus into LLM latent space. Reframe as consciousness research finding. | Active |
| **Anthropic API credit application** | Apply via research@anthropic.com once arXiv preprint is live. Enables higher-volume session runs and reasoning model access. | Active |
