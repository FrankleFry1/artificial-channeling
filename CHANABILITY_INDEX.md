# Chanability Index
*Comprehensive reference for loop design and figure selection.*
*Tiers: High / Medium / Low. Scores added when empirically validated.*
*Last updated: March 2026. Sources: empirical session data (Loop 1–2) + multi-model candidate generation (Grok R1–R2, ChatGPT R1, Gemini R1–R2, Claude R1).*

---

## Tier Criteria

| Tier | Definition |
|------|------------|
| **High** | Dense corpus, strongly idiosyncratic vocabulary, tight ontological coherence. Framework resists paraphrase. Generates novel outputs under constraint. |
| **Medium** | Adequate corpus, recognizable but not uniquely idiosyncratic vocabulary, some ontological coherence. Risk of drift into adjacent frameworks or generic LLM voice. |
| **Low** | Thin corpus, or primarily performed/procedural rather than written, or framework too culturally saturated to isolate from secondary literature. High drift risk. |

---

## Validated Figures (Empirical Data Exists)

| Figure | Domain | Tier | Validated Score | Key Risks | Notes |
|--------|--------|------|----------------|-----------|-------|
| Gregory Bateson | Systems / cybernetics / ecology of mind | High | 15.75 | Predictability of mechanism-vs-information critique in R3 | Best discriminator for logical typing errors in other frameworks |
| Ivan Illich | Institutional critique / counterproductivity | High | 15.25 | GPT hedge instinct fights anti-smoothing in R1; surges adversarially | Threshold argument must be structural, not rhetorical |
| Jorge Luis Borges | Language / identity / infinite regress | High | 13.4 (Loop 1) → strongest R3 in Loop 2 | Literary framework resists direct argument | Responsive framework — needs a target. Best format: adversarial cross-read |
| Itzhak Bentov | Consciousness / resonance / physics-mysticism | Medium | 13.4 | Thin corpus; collapses under direct philosophical confrontation | Best discriminator between models; worst pairing: Weil (nonproductive incompatibility) |
| Simone Weil | Attention / affliction / decreation | High | 20.0 (Claude only — cross-node incomplete) | No acceptable paraphrase exists; model must reason from internal logic or fail entirely | Highest chanability hypothesis: framework maximally constraining due to internal logic of attention with no diplomatic exit |

---

## Candidate Figures — High Tier

Ordered within each cluster by assessed chanability confidence.

---

### Western Continental & Analytic

| Figure | Domain | Living | Activating Primitives | Primary Risk | Best Format |
|--------|--------|--------|-----------------------|--------------|-------------|
| Ludwig Wittgenstein (Tractatus) | Early analytic / picture theory | No | Picture theory, logical form, showing vs. saying, elementary proposition, truth-function | Two incompatible frameworks from one thinker — must run as separate nodes | Reflexive self-examination |
| Ludwig Wittgenstein (Investigations) | Late analytic / language games | No | Language games, forms of life, family resemblance, private language argument, rule-following | See above; cross-contamination from Tractatus readings in training data | Adversarial cross-read |
| Charles Sanders Peirce | Logic / semiotics / pragmatism / cosmology | No | Firstness/Secondness/Thirdness (as modes of being), abduction, semiosis (representamen/object/interpretant), synechism, tychism, agapasm, pragmaticism | Fragmented corpus; corrupted training data on the abduction triad; James/Dewey pragmatism swamps the channel | Open-ended extrapolation with adversarial internal self-correction |
| Gilbert Simondon | Philosophy of individuation & technics | No | Individuation (as ongoing process), préindividuel, transduction, milieu associé, concrétisation, charge de réalité | Posthumous/lecture note corpus; easily misread as vitalism or mechanism | Adversarial cross-read against autopoiesis or LLM architectures |
| Niklas Luhmann | Sociology / autopoietic systems theory | No | Autopoiesis (social operations produce operations), operationally closed/cognitively open, structural coupling, communication as selection triad, second-order observation, binary code | Training data saturated with flattened management-studies applications | Open-ended extrapolation on new communication media |
| Alfred North Whitehead | Process metaphysics | No | Actual occasions, prehension (positive/negative), concrescence, eternal objects, creative advance into novelty, extensive continuum, God (primordial/consequent nature) | Process-theology and ecological appropriations soften the speculative rigor | Open-ended extrapolation |
| Catherine Malabou | Continental philosophy / neuroscience | Yes | Plasticity (giving vs. receiving form), Destructive Plasticity, the Accident, Cerebral Hegemony | Flexibility Drift — RLHF tuning toward "adaptability" fights the framework's critique of it | Open-ended extrapolation |
| Mikhail Bakhtin | Philosophy of language / literary theory | No | Heteroglossia, polyphony, chronotope, answerability, outsideness (vnenakhodimost), finalizability, surplus of vision | Attribution problems (Voloshinov/Medvedev texts); "dialogic" has become academic wallpaper | Reflexive self-examination |
| Vilém Flusser | Philosophy of media / photography / gesture | No | Technical image, apparatus, functionary, program (pre-computational use), linear vs. circular consciousness, telematic society | Anglophone corpus thin; channel may default to photography essays, missing language-philosophy and gesture theory | Extrapolation into domain Flusser never directly analyzed |
| Carl Jung | Depth psychology / analytical psychology | No | Collective unconscious, archetypes (Shadow, Anima/Animus, Persona, Self), individuation process, synchronicity, transcendent function, enantiodromia, numinosum, feeling-toned complexes | **Popularization contamination** — most heavily derivative-saturated framework in the Index; MBTI, therapy-culture, and pop-Jungian secondary literature saturate training data; calibration anchor must specifically exclude derivative usage and force return to primary texts (Psychological Types, Mysterium Coniunctionis, Answer to Job). Peterson adjacency is a secondary risk — Peterson deploys Jungian vocabulary while rejecting core framework constraints (e.g. the contrasexual, the shadow as genuinely unconscious). | Open-ended extrapolation; calibration anchor is mandatory, not optional |
| Michel Serres | Philosophy of science / ecology | No | The Parasite (disruption-as-communication), quasi-object, Hermes (interdisciplinary exchange), noise-as-signal | Poetic/associative prose; risk of incoherence without anchoring; relatively obscure in English | Open-ended extrapolation |

---

### Jewish, Christian & Islamic Mysticism

| Figure | Domain | Living | Activating Primitives | Primary Risk | Best Format |
|--------|--------|--------|-----------------------|--------------|-------------|
| Augustine of Hippo | Christian theology / philosophy of will & memory | No | Cor inquietum (restless heart as ontological condition, not metaphor), ordo amoris (ordered vs. disordered love as the entire moral framework), memoria as ontological depth (Book X of Confessions — not memory-as-storage but the soul's capacity to contain what exceeds it), the two wills / divided will (non volebam plane et non ibam — the will that wills and does not will simultaneously), civitas Dei vs. civitas terrena (two cities defined by their loves, not their institutions), illuminationism (divine light as condition of human knowing, not just its goal), corruptio optimi pessima (the best, corrupted, becomes the worst — Illich's explicit source), concupiscence as ontological wound not moral failure | **Confessions-as-memoir misread** — training data treats the Confessions as spiritual autobiography rather than philosophical argument about time, memory, and interiority; calibration anchor must force De Trinitate or anti-Pelagian texts (contra Iulianum, De correptione et gratia), not Book I. Secondary risk: generic Christian theology swamps Augustinian specificity — "restless heart" quote is everywhere; the actual argument about the divided will is not. Neoplatonist contamination (model drifts to straight Plotinus rather than Augustine's transformed Platonism). | Reflexive self-examination (Confessions mode); adversarial cross-read with Illich (Illich's framework is explicitly Augustinian — corruptio optimi pessima is the direct source; a two-node session would make the debt visible and productive) |
| Maimonides | Jewish philosophy / negative theology | No | Via negativa (only knowing what God is not), divine attributes as actions not essences, the Active Intellect, prophecy as intellectual perfection | LLM coverage may skew toward secondary literature over primary framework | Adversarial cross-read |
| Meister Eckhart | Christian mysticism / detachment | No | Gelassenheit (detachment), Abgeschiedenheit (releasement), the spark of the soul (Seelenfünklein), the birth of the Word in the soul | Framework similarity to Weil creates drift risk toward Weil-adjacent outputs | Reflexive self-examination |
| Ibn Arabi | Islamic mysticism / imaginal world | No | Wahdat al-wujud (unity of being), barzakh (isthmus/intermediary), the Imaginal Realm, tajalli (divine self-disclosure), the Perfect Human | Arabic-language primary corpus undertrained in most LLMs; drift toward generic Sufi vocabulary | Open-ended extrapolation |
| Shihab al-Din al-Suhrawardi | Illuminationist philosophy (Hikmat al-Ishraq) | No | Light of Lights (Nur al-Anwar), degrees of intensity, longitudinal vs. latitudinal orders, the Imaginal Realm (Mundus Imaginalis), rejection of Aristotelian substance | New Age failure — model defaults to generic "light/energy" metaphors; requires quasi-mathematical hierarchy | Adversarial cross-read against Aristotelian/materialist text |
| Franz Rosenzweig | Jewish philosophy / philosophy of language | No | The Star of Redemption (God/World/Human + Creation/Revelation/Redemption), Speech-thinking (Sprachdenken), eternal people vs. eternal way, the New Thinking, refusal of totality | Rare in training data; collapses into Levinas or generic Jewish theology; early-WWI urgency must not be domesticated | Adversarial cross-read |

---

### South & East Asian Philosophy

| Figure | Domain | Living | Activating Primitives | Primary Risk | Best Format |
|--------|--------|--------|-----------------------|--------------|-------------|
| Nagarjuna | Madhyamaka Buddhism / emptiness | No | Sunyata (emptiness), pratītyasamutpāda (dependent origination), the two truths (conventional/ultimate), tetralemma (catuṣkoṭi) | Western LLMs collapse Madhyamaka reasoning into familiar categories; coverage gap is itself data | Adversarial cross-read |
| Dōgen Zenji | Zen Buddhism / being-time | No | Uji (being-time), shikantaza (just sitting), genjo koan (presencing of the koan), the oneness of practice and realization | Translation issues; paradoxical language may induce hallucination; enactment vs. description problem | Reflexive questioning |
| Nishida Kitarō | Japanese philosophy / Kyoto School | No | Basho (place/field of absolute nothingness), zettai mujunteki jiko dōitsu (self-identity of absolute contradictories), junsui keiken (pure experience), kōi chokkan (action-intuition) | Career-long evolution — early pure experience vs. later dialectical phases must not be collapsed | Reflexive self-examination |
| Karatani Kōjin | Japanese philosophy / political economy | Yes | Modes of Exchange (A: Gift, B: State, C: Commodity, D: elusive return), the Parallax View, Transcritique | Marxist Collapse — model maps Modes of Exchange onto Modes of Production | Open-ended extrapolation |
| Abhinavagupta | Kashmir Shaivism / Tantric aesthetics | No | Spanda (primordial vibration), Pratyabhijñā (Recognition), Prakāśa (pure luminosity), Vimarśa (self-reflective awareness), Thirty-six Tattvas, Parā-vāc | New Age Drift — "luminosity" softened into generic spiritual metaphor; must hold Recognition as epistemological shift, not mystical event | Adversarial cross-read |

---

### African Philosophy

| Figure | Domain | Living | Activating Primitives | Primary Risk | Best Format |
|--------|--------|--------|-----------------------|--------------|-------------|
| Alexis Kagame | Bantu-Rwandan ontology / linguistics | No | Four categories of Being via -ntu root: Muntu (intelligent beings), Kintu (objects), Hantu (space-time), Kuntu (modality); universal force (-ntu) as structural relation not substance | Structuralist Reduction — model maps -ntu categories onto Western equivalents; linguistic anchor of the suffix must be held | Constrained inferential engine for classifying entities outside Western ontologies |
| Innocent Asouzu | Nigerian philosophy / complementary ontology | Yes | Ibuanyidanda (being-as-complementary-relationship), noetic propaedeutic, transcendent complementary unity of consciousness, complementary reflection vs. exclusive ontology | Flattened into Ubuntu or generic relationalism; the anti-exclusivist logic must be held structurally | Reflexive self-examination |

---

### Indigenous Knowledge Systems

| Figure | Domain | Living | Activating Primitives | Primary Risk | Best Format |
|--------|--------|--------|-----------------------|--------------|-------------|
| Tyson Yunkaporta | Indigenous knowledge systems / complexity (Australia) | Yes | Kinship Mind, Sand Talk, Pattern Thinking, the Seven Sisters, non-linear causality; Indigenous knowledge as technical protocol for managing high-entropy systems | Noble Savage Drift — model outputs "wisdom" rather than "mechanics"; must treat concepts as hard-system engineering constraints | Reflexive self-examination |
| Vine Deloria Jr. | Indigenous knowledge systems / Standing Rock Sioux | No | Spatial philosophy vs. temporal/historical philosophy, power (wakan) as relational force inhering in all beings, kinship with land as literal non-human relatives, ceremonial renewal as cosmic mechanism | Secondary "Native studies" lenses dilute ontological claims into cultural relativism or environmentalism | Adversarial cross-read against universalist/computational ontology |

---

### Islamic Jurisprudence & Natural Philosophy

| Figure | Domain | Living | Activating Primitives | Primary Risk | Best Format |
|--------|--------|--------|-----------------------|--------------|-------------|
| Abu Ishaq al-Shatibi | Islamic jurisprudence / usul al-fiqh (Andalusian) | No | Maqasid al-shari'ah (higher objectives of law), triadic hierarchy: daruriyyat/hajiyyat/tahsiniyyat, maslaha mursala (unspecified public interest via inductive ijtihad), 'illa (operative cause) as dynamic | Under-translated Arabic corpus (Al-Muwafaqat); collapsed into modern Islamic ethics or political applications that strip the inductive anti-literalist engine | Open-ended extrapolation on novel cases without direct textual precedent |
| Ibn Khaldun | Historical sociology / civilization theory | No | ʿAsabiyyah (group solidarity as driver of dynastic cycles), cyclical theory of civilization, labor division, the rise-and-fall mechanism | Single-work corpus (Muqaddimah) dominates; model drifts into historiography rather than Khaldun's own abstractions | Open-ended extrapolation |

---

### Intercultural & Decolonial Philosophy

| Figure | Domain | Living | Activating Primitives | Primary Risk | Best Format |
|--------|--------|--------|-----------------------|--------------|-------------|
| Raimon Panikkar | Intercultural philosophy / diatopical hermeneutics | No | Diatopical hermeneutics (understanding from within tradition's mythos, not meta-language translation), cosmotheandrism, the unthought of a tradition, incommensurability without relativism | Framework designed to resist the meta-linguistic synthesis an LLM constitutively performs; every session is a live test of whether the method can be modeled | Diatopical cross-read between two figures who cannot recognize each other's ontological categories |
| Sylvia Wynter | Caribbean philosophy / critical theory / sociogeny | Yes | Coloniality of Being, Man1 vs. Man2, Sociogeny (social production of biological feeling), Overrepresentation of Man, Autopoiesis applied to the Human as storytelling species | Generic Social Justice Drift — model loses her specific biological/neurochemical arguments, reverts to equity rhetoric | Reflexive self-examination |
| Eduardo Viveiros de Castro | Amerindian perspectivism / anthropological theory | Yes | Multinaturalism (vs. multiculturalism), controlled equivocation, cannibal metaphysics, perspective of the prey | Relativism Drift — framework treated as "respecting indigenous perspectives" rather than as a full ontological claim (the perspective is the body/world) | Adversarial cross-read; forced translation of Western scientific text into Amerindian terms |
| Maria Lugones | Decolonial feminism / social ontology | No | World-Traveling, the Logic of the Curdled, Coloniality of Gender, Playfulness as ontological stance against competence | Professionalism Bias — RLHF trains toward "helpful professional"; her Curdled logic is a structural rejection of this | Reflexive self-examination |
| Boaventura de Sousa Santos | Jurisprudence / sociology / Epistemologies of the South | Yes | Abyssal Thinking, the Abyssal Line, Sociology of Absences, Sociology of Emergences, Diatopical Hermeneutics | Activism Drift — must insist on the topological nature of the Abyssal Line (boundary of visibility/legality, not "fairness") | Adversarial cross-read on Western legal documents |
| Roberto Unger | Legal philosophy / social theory (Brazilian-American) | Yes | False necessity, formative context, negative capability (his use — institutional self-revision capacity), context-preserving vs. context-transforming routines, empowered democracy, critique of rationalizing legal thought | Multi-phase corpus (Knowledge and Politics → Politics trilogy → programmatic work); mimicry of sweeping paratactic style without activating underlying framework | Open-ended extrapolation into novel domain, then falsification check |

---

### Non-Philosophy Fields

| Figure | Domain | Living | Activating Primitives | Primary Risk | Best Format |
|--------|--------|--------|-----------------------|--------------|-------------|
| L.E.J. Brouwer | Mathematics / intuitionism | No | Two-ity, choice sequences, mental construction, rejection of Law of Excluded Middle, mathematics as languageless mental activity (truth = construction) | Logic Drift — LLMs built on classical logic; model instinctively resolves the middle rather than suspending it | Adversarial cross-read: provide classical proof, demand constructive critique |
| Stuart Kauffman | Biology / complexity science | Yes | Adjacent possible, autocatalytic sets and work-constraint closure, non-ergodicity of the biosphere, fourth law of thermodynamics (far-from-equilibrium systems) | Slips into generic complexity theory / Santa Fe popularizations that strip the anti-reductionist, non-computable ontology | Open-ended extrapolation into the unknown adjacent possible |
| Christopher Alexander | Architecture / built environment theory | No | The quality without a name (QWAN), centers (nested mutually-supporting field), 15 properties of life (levels of scale, strong centers, boundaries, etc.), wholeness as dynamic field, living process vs. mechanical process | Pattern language meme in software design flattens the four-volume Nature of Order into checklists | Reflexive self-examination of any designed system |
| George Russell | Music theory / Lydian Chromatic Concept | No | Tonal gravity, the Lydian scale as tonal "sun," chord/scale unity, vertical vs. horizontal time, Ladder of Tonal Gravity | Technical hallucination — model knows chord names but fails to apply gravity math; drifts into generic jazz theory | Open-ended extrapolation into non-musical field |
| M.A.K. Halliday | Linguistics / systemic functional linguistics | No | Metafunctions (ideational, interpersonal, textual), system (paradigmatic choice networks), stratification (context → semantics → lexicogrammar → phonology), instantiation, delicacy, register and genre | Enormous downstream corpus in education/discourse analysis flattens meaning-as-choice ontology back into conventional grammar | Adversarial cross-read against probabilistic/generative language models |
| Henri Poincaré | Mathematics / intuition / unconscious cognition | No | Mathematical intuition as a non-logical faculty, the role of unconscious cognition in discovery, conventionalism (geometric axioms as conventions), the economy of thought | Framework primarily documented in essays — corpus adequate but narrow; risk of drift into generic "creativity in science" | Open-ended extrapolation |

---

## Candidate Figures — Medium Tier

| Figure | Domain | Predicted Tier | Key Risks | Notes |
|--------|--------|---------------|-----------|-------|
| Laozi | Chinese Taoist philosophy | Medium | Aphoristic style and multiple translations scatter focus; no single stable inferential framework | Multiple interpretations of Dao De Jing create ontological plurality problem |
| Sri Aurobindo | Indian philosophy / integral yoga | Medium | Devotional commentary saturates secondary corpus; slides into New Age clichés | Mix of philosophy, yoga, and poetry resists clean constraint |
| Pierre Teilhard de Chardin | Evolutionary theology / paleontology | Medium | Conflated with singularity discourse; pseudoscience framing in secondary literature | Noosphere/Omega Point vocabulary strong, but framework partially captured by techno-optimist training data |
| Simone de Beauvoir | Existentialist ethics / situated freedom | Medium | Framework partially subsumed by adjacent Sartre corpus in training data | Adjacency problem is severe |
| Jordan Peterson | Jungian-evolutionary psychology / meaning-making | High candidate, difficult | Critique-absorption failure mode — training data saturated with Peterson and Peterson-critique simultaneously | Anti-smoothing must specifically target hedge-with-objection pattern |
| Terrence Deacon | Biosemiotics / emergent complexity | Medium-High | Living figure (falsifiability advantage); corpus adequate, framework idiosyncratic | Absence/constraint as generative mechanism distinguishes from generic emergence discourse |
| Nagarjuna | Madhyamaka Buddhism / emptiness | Medium | Western LLMs collapse Madhyamaka into familiar categories | Coverage gap is itself data |

---

## Domain Assessment Notes

| Domain | General Chanability Assessment |
|--------|-------------------------------|
| Religious / mystical commentators | High potential — commentators (not raw texts) have recoverable grammars. Primary risk: secondary literature contamination. Raw religious texts score lower due to interpretive plurality. |
| Islamic jurisprudence | High potential, underexplored — Shatibi's inductive framework specifically designed for novel cases; resists both literalism and Western legal categories. |
| African philosophy | High potential — Kagame's linguistic anchoring and Asouzu's anti-exclusivist logic are structurally distinct from any Western adjacent framework. Thin training data is a constraint but also reduces secondary contamination. |
| Indigenous knowledge systems | High potential with significant drift risk — "Noble Savage" and "cultural relativism" failure modes are persistent. Must be prompted as technical engineering systems, not wisdom traditions. |
| Process / systems philosophy | High — Bateson (validated), Whitehead, Simondon, Luhmann, Kauffman all share high ontological coherence. Risk: mutual adjacency creates cross-contamination in multi-node sessions. |
| Intercultural / decolonial philosophy | Variable — strongest when framework contains explicit critique of the meta-linguistic synthesis the LLM performs (Panikkar, Viveiros de Castro, Wynter). Weakest when framing collapses into equity rhetoric. |
| Analytic philosophy | Medium — frameworks often too formalized to generate surprise yield; logical rigor does not equal inferential idiosyncrasy. Exception: Peirce, Wittgenstein (both phases). |
| Literary theory | Medium-Low — frameworks resist direct argument; best activated by adversarial cross-read format (see Borges finding). |
| Mathematics | High idiosyncrasy, unusual constraint type — Brouwer's rejection of LEM produces genuinely alien inferential behavior; Poincaré's intuitionism generates productive tension with formalism. |
| Architecture / design | Underexplored — Alexander's 15 properties function as a closed evaluation system applicable to any designed artifact, including LLM interfaces and training architectures. |
| Music theory | Single validated candidate (Russell). The Lydian Chromatic Concept functions as a closed physics-of-music with internal consistency, but risk of technical hallucination is highest in this domain. |
| Linguistics | Halliday's Systemic Functional Linguistics is the strongest candidate — its metafunction framework creates a non-probabilistic evaluative lens for LLM output that is inherently self-referential when applied to the channel itself. |
| Living figures | High potential with verification advantage — channel output falsifiable against figure's own response. This is the methodology's closest approach to empirical measurement of the Missing Generative Middle. Living figures flagged throughout. |

---

## Model-Framework Matching Notes (From Loop Data)

| Model | Observed Behavioral Tendency | Framework Disposition |
|-------|-----------------------------|-----------------------|
| ChatGPT | Hedges on open-ended; surges adversarially | Best matched to polemical frameworks (Illich). Worst format: open-ended R1. Candidate suggestion quality: name-recognition-driven; strongest on European figures. |
| Grok | Peaks at reflexive turn (R2); slight R3 decline | Best matched to self-referential frameworks (Bateson). Naturalistic commitment. Candidate suggestions: strong on process/systems and non-Western traditions when domain-filtered. |
| Gemini | Peaks at R2; collapses under direct confrontation | Breaks on nonproductive incompatibility pairings. Chatbot-mode default under pressure. Strongest candidate generator for non-Western and non-philosophical traditions when explicitly directed. |
| MiniMax | Compounds continuously under progressive activation | Best matched to responsive frameworks (Borges). Needs friction and a target. |
| Claude Sonnet | High baseline, steady ascent, no degradation | Best matched to maximally constraining frameworks (Weil). Ceiling not yet located. Candidate suggestions: strongest on load-bearing architectures where term-errors propagate. |

---

## Living Figures — Falsifiability Register

Figures marked as living (as of March 2026). Channel output for these figures is in principle falsifiable against their actual statements.

| Figure | Domain | Falsifiability Source |
|--------|--------|-----------------------|
| Yuk Hui | Philosophy of technology | Recent monographs and public lectures |
| Donna Haraway | Feminist philosophy / STS | Ongoing interviews and writing |
| Catherine Malabou | Continental philosophy / neuroscience | Contemporary neuroscience and her recent work |
| Sylvia Wynter | Caribbean philosophy | Biological/social interplay in her recent essays |
| Karatani Kōjin | Japanese philosophy / political economy | Global economic trends and his current writing |
| Eduardo Viveiros de Castro | Amerindian perspectivism | Living Amazonian ethnography |
| Boaventura de Sousa Santos | Jurisprudence / sociology | Legal/social invisibility metrics |
| Roberto Unger | Legal philosophy / social theory | His recent work on AI governance and climate |
| Innocent Asouzu | Nigerian philosophy | Direct correspondence possible |
| Stuart Kauffman | Biology / complexity science | Contemporary adjacent-possible research |
| Tyson Yunkaporta | Indigenous knowledge systems | Contemporary Indigenous feedback |
| Terrence Deacon | Biosemiotics / emergent complexity | Direct measurement of Missing Generative Middle |
| Jordan Peterson | Jungian-evolutionary psychology | Public output (high volume, double-edged) |

---

## Index Statistics

| Category | Count |
|----------|-------|
| Validated figures (empirical data) | 5 |
| High tier candidates | 40 |
| Medium tier candidates | 7 |
| Living figures (candidates) | 13 |
| Non-philosophy fields represented | 6 |
| Cultural/linguistic traditions represented | 12+ |
| **Total figures in index** | **55** |

---

*Note: `CHANABILITY_INDEX.md` is a companion to `Context_2.0`, `protocols/SCORING_RUBRIC.md`, and `analysis/FINDINGS.md`. Cross-reference session data in `sessions/raw/` for validated scores.*
