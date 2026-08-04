# Decision Record

> The load-bearing judgment calls behind this corpus's shape: what was decided, what was rejected, why, and what would reopen each question.

This record applies the corpus's own directions to the corpus itself: decisions closed during construction are surfaced rather than left silent ([making closed decisions inspectable](2-intent.md#d-decision-surfacing)); reasons are kept where episodes cannot lose them ([what must be recorded](3-actors.md#d-record-scope)); and every entry states when it should be overturned, so the record stays subordinate to present judgment ([cheap, visible supersession](2-intent.md#d-cheap-supersession)).

Standing and maintenance: this file cites the theory freely; nothing load-bearing — axioms, theorems, directions — ever cites it. It is append-and-mark: later amendments add dated entries (the founding set is undated); superseded entries are marked, never deleted. Anchors (`dr-`) are permanent. The voice is editorial throughout: decisions and reasons, not process narrative.

## Contents

- [Status](#status)
- [Structure and conventions](#structure)
- [Scope and setting](#scope)
- [The razor's close calls](#close-calls)
- [Divergences in deep-writing](#divergences)
- [Voice, presentation, and this record](#voice)

## <span id="status">Status</span>

This record stands at the granularity of the corpus's founding pass: judgment calls large enough to shape axioms, theorems, and conventions, and no finer. A more detailed design pass is expected as the corpus moves from axioms into applied frameworks — likely finer-grained entries, and possibly a revisit of the entry schema once real use shows what the current fields miss. Both are anticipated amendments under the maintenance rule above, not corrections to it: new entries append, and any schema change would be filed as an entry of its own.

## <span id="structure">Structure and conventions</span>

### <span id="dr-strata">DR-1 — Strata by rate of change</span>

**Decision.** Six layers — bedrock, setting, axioms, theorems, directions, observations — with dependence pointing strictly toward the slower-changing layers.

**Instead of.** A flat structure: overview essay plus axiom documents, with engineering directions hanging directly off axioms.

**Because.** Directions descending from two axioms would either be duplicated or orphaned without a theorem layer to hold them. A living corpus also needs its volatile material quarantined from its stable material so each can change at its own pace.

**Reopens if.** A kind of content appears that fits no layer. (The layer set is extensible; this record is itself a layer added after the founding five.)

### <span id="dr-three-axioms">DR-2 — Three axioms carrying eleven clauses</span>

**Decision.** Three axioms — the Medium, Intent, Actors — each bundling clauses that share one subject, with the razor audits run at both grains.

**Instead of.** Eight to eleven flat, single-clause axioms.

**Because.** Once the setting is factored out, the three subjects are the domain's ontology: the thing, the wanting, the participants. Flat axioms would scatter that coherence and make the completeness sweep harder to state. Bundling costs nothing so long as every clause is individually anchored, individually audited, and individually used downstream.

**Reopens if.** A clause accumulates descendants whose subject is alien to its axiom — a sign the bundle is hiding a fourth subject.

### <span id="dr-junction-homing">DR-3 — Junction theorems homed by subject</span>

**Decision.** Theorems drawing equally on two axioms (T13, T14) live under the axiom bearing their subject, with co-parentage indexed in the other parent's _Descendants homed elsewhere_ section.

**Instead of.** Duplicating junction theorems under each parent, or collecting them in a separate junctions document.

**Because.** Every traceability chain should be single-rooted and unbroken. Duplication forks the chain; a junctions document would add a navigation stop that serves the filing system rather than the reader. The elsewhere-sections keep the graph walkable from both ends at the cost of one line per co-parent.

**Reopens if.** Junction theorems multiply to the point that elsewhere-sections dominate the axiom documents.

### <span id="dr-numbering">DR-4 — Corpus-wide, append-only theorem numbers</span>

**Decision.** Theorems are numbered globally (T1–T14), junctions after the per-axiom runs; new theorems take the next free number regardless of home; numbers are never reused or reordered.

**Instead of.** Per-axiom numbering (A2-T1 and the like), or renumbering on insertion.

**Because.** Cross-document references must survive growth. A number that can change is a link that can rot; a number that encodes its home breaks when a theorem's homing is corrected.

**Reopens if.** Never expected; the rule is deliberately boring.

### <span id="dr-anchors">DR-5 — Explicit anchors, name-based direction identifiers</span>

**Decision.** Every clause, theorem, and direction carries an explicit HTML anchor; direction identifiers are names (`d-gaming-resistance`), not numbers; anchors are permanent once published, with two stated exceptions (observations are replaced wholesale; this record is append-and-mark).

**Instead of.** Heading-derived anchors, and numbered directions.

**Because.** Heading-derived anchors break when titles are reworded, and the corpus explicitly reserves the right to reword titles. Numbered directions punish insertion — adding a direction between two others would either renumber or misorder; names do neither.

**Reopens if.** Never expected.

### <span id="dr-argued-theorems">DR-6 — Theorems as argued consequences, not formal proofs</span>

**Decision.** The word _theorem_ is used in the argued sense, and every document says so.

**Instead of.** A formal apparatus — symbolic statements, machine-checked derivations.

**Because.** The corpus should claim exactly what its derivations can back. The arguments are meant to be inspected and attacked in prose by any careful reader, including one with no programming background. Formal dress would narrow the audience while adding rigor the subject matter (wanting, judging, trusting) cannot yet honestly support.

**Reopens if.** Fragments of the derivation graph are formalized — welcome as an addition, never as a replacement for the prose argument.

## <span id="scope">Scope and setting</span>

### <span id="dr-dyad-unit">DR-7 — The dyad as unit of analysis</span>

**Decision.** The theory's unit is one delegator, one producer, and the artifacts between them; every larger arrangement is composed from dyads under a single invariant — every producer faces exactly one delegator-side corpus of expressions.

**Instead of.** Multi-party primitives inside the foundations: committees of delegators, negotiation protocols, stakeholder models.

**Because.** Every multi-party phenomenon examined reduced to the invariant plus three mechanisms already needed for other reasons: precedence marks on inherited constraints (chains), scope partition with seam promises (fan-out), and escalation (conflicts). Admitting multi-party primitives would have grown the axiom set to cover phenomena the dyad already explains.

**Reopens if.** A composition shape appears that provably cannot reduce to the invariant — that would be a defect of the setting, not of a framework.

### <span id="dr-fan-in">DR-8 — Fan-in refused as a primitive</span>

**Decision.** Multiple delegators over one producer and one scope is not granted a resolution mechanism; it must be merged upstream, partitioned into disjoint dyads, or refused and escalated.

**Instead of.** An in-theory arbitration rule letting a producer weigh two live authorities.

**Because.** Any such arbitration rule would itself be an authority-ordering over the delegators — which is exactly the upstream merge the refusal demands, relocated into the producer and performed without a mandate. The refusal is not a gap in the theory; it is the honest location of the merge.

**Reopens if.** Same condition as [DR-7](#dr-dyad-unit).

### <span id="dr-leverage">DR-9 — Leverage demoted from definition to common motive</span>

**Decision.** The setting defines delegation by the transfer of production under retained authority over fit; leverage is noted as the common motive, not a defining property. T12's scarcity claim rests on boundedness (3a), not on the motive.

**Instead of.** Treating "delegation exists to gain leverage" as definitional, and grounding the judgment-budget economics on that purpose.

**Because.** Counterexamples exist — delegation for training, for redundancy, for independence of judgment — and a definition with counterexamples poisons everything derived from it. Judgment is scarce whatever the motive; grounding T12 on 3a made the theorem hold across all of them.

**Reopens if.** Never expected; recorded as an instance of a working rule — definitions are checked against counterexamples before anything is built on them.

### <span id="dr-substrate">DR-10 — Substrate-indifference derived, not assumed</span>

**Decision.** The requirement that rules bind roles and profiles rather than kinds of actor is a theorem (T11, from 3d and the setting).

**Instead of.** An axiom or standing constraint declaring that the theory must not assume the parties' kinds.

**Because.** As a conclusion it carries force an assumption cannot: a reader who doubts the posture can attack the derivation rather than reject a stipulation. It also keeps the axiom set purely descriptive — the axioms say what is true of medium, wanting, and actors; they do not legislate how theory must be written.

**Reopens if.** The derivation from 3d is refuted — in which case the posture would need to be defended as a choice, honestly relabeled.

## <span id="close-calls">The razor's close calls</span>

### <span id="dr-2c-axiomatic">DR-11 — Clause 2c held axiomatic — the closest call on the intent side</span>

**Decision.** Motion and present authority stand as a clause of Axiom 2.

**Instead of.** Deriving intent's motion from bedrock (the world changes) plus encounter-elicitation, with present authority folded into the setting's definitions.

**Because.** Motion is not entailed: a holder who never updates is logically possible, so instability had to be asserted, not derived. Present authority is normative in shape — no descriptive clause forces it. And the clause's expected weight in later engineering work argued for a clean, independently citable statement rather than a conclusion assembled from three sources.

**Reopens if.** A derivation forces present authority from 2a, 2b, and the setting alone; 2c would then drop to a theorem, and the graph would be rewired accordingly.

### <span id="dr-3c-correlation">DR-12 — Clause 3c re-grounded on correlation — the closest call on the actor side</span>

**Decision.** 3c's core claim is that an actor's self-assessment shares the blind spots of the work itself — a claim about the _alignment_ of errors, not about additional fallibility.

**Instead of.** (a) Stating 3c as "reports about one's own work err" — derivable from 3b, and therefore due to be cut; (b) demoting self-certification to a theorem.

**Because.** 3b speaks only to error rates and is silent on how self-assessment errors relate to production errors. The correlation claim is the non-derivable residue — and it is the only ground from which T9's demand for _independent_ verification actually follows. Without it, "verify independently" is an intuition, not a consequence.

**Reopens if.** Never expected; recorded for the method it exemplifies — when the razor threatens a clause, first ask whether the statement is hiding its non-derivable core.

### <span id="dr-discovery-split">DR-13 — Discovery split from motion</span>

**Decision.** "Intent is discovered through encounter" is a theorem (T7); "intent moves" is a clause (2c). They were separated deliberately.

**Instead of.** A discovery clause inside Axiom 2 covering both.

**Because.** Elicitation-through-encounter is derivable (2a, 2b, 1d, plus bedrock's bounded minds), and the razor sends derivable content to the theorem layer. Motion is not derivable ([DR-11](#dr-2c-axiomatic)). The split places each on its correct side of the razor, at the cost of readers meeting two homes for neighboring ideas.

**Reopens if.** Same trigger as DR-11 — the two decisions move together.

### <span id="dr-1d-grounds">DR-14 — Opacity given three independent grounds</span>

**Decision.** 1d rests on a logic limit, a scale limit, and a situation limit — each stated as individually sufficient.

**Instead of.** Grounding opacity on environment-dependence alone.

**Because.** With only the situation ground, 1d risks collapsing into 1b, failing the independence audit. The logic limit holds even in a frozen, fully known environment; it is what secures the clause's standing on its own feet.

**Reopens if.** Never expected; bedrock would have to move.

### <span id="dr-2b-dimensions">DR-15 — Underdetermination grounded in unconsidered dimensions</span>

**Decision.** 2b's ground is that expressions answer only along the dimensions their maker was weighing — not a counting argument about finite texts and infinite cases.

**Instead of.** The cardinality argument.

**Because.** Generality defeats counting: one rule can cover infinitely many cases. What no rule covers is the dimensions unweighed at authorship. The dimensional ground also keeps 2b non-derivable from 2a plus bedrock, which the counting argument would not have survived, and it explains the residue's structure well enough to carry T6 and T7.

**Reopens if.** Never expected.

### <span id="dr-folded-material">DR-16 — Material folded rather than promoted</span>

**Decision.** Three candidates were folded into existing homes rather than granted clause status: exact copyability lives inside 1a's statement; compositional reference (parts referring to parts) lives in 1c's commentary as the mechanism of non-locality; irreversibility stays in bedrock and surfaces at T5.

**Instead of.** Clauses for each.

**Because.** Each failed the clause bar — deletion cost too low or content derivable-adjacent — while still pulling real weight where placed. Copyability is load-bearing for rehearsal spaces and version-binding but is a property, not a gap; reference explains 1c rather than adding to it; irreversibility is a fact about the world, not about software.

**Reopens if.** A body of descendants forms that traces to the folded material specifically rather than to its host clause.

## <span id="divergences">Divergences in deep-writing</span>

### <span id="dr-skeleton-divergence">DR-17 — The skeleton treated as floor, not contract</span>

**Decision.** Where full derivation contradicted or outgrew the planning skeleton, the derivation won, and the graph was corrected in the same change. Parentage corrections: T1 gained 1b (assurance decays as the environment moves); T5 gained 1d (the rehearsal/real tension exists only because learning requires running); T6 gained 1a (code cannot abstain); T12 gained 3d (calibration presupposes measurable difference). Directions not in any plan, discovered by the derivations that needed them: recording what a run established (T2); binding evidence to exact text (T3); consequence-classing the work itself (T5); loading within bounds (T10).

**Instead of.** Preserving planned parentage for stability, or filing discovered directions as future work.

**Because.** The graph's authority derives from the arguments as written, not from any outline of them. A parentage line that flatters the plan over the text is a false record — the exact failure T8 names.

**Reopens if.** Standing rule rather than a decision to reopen: every future amendment inherits it.

## <span id="voice">Voice, presentation, and this record</span>

### <span id="dr-reader-conventions">DR-18 — Reader-facing conventions</span>

**Decision.** Concepts are derived under plain names first, with current practice's terms attached afterward as parenthetical labels; analogies always state where they break; every term of art is introduced before use.

**Instead of.** Leading with standard terminology, and using analogies as ornament.

**Because.** One discipline serves two ends: refusing inherited vocabulary keeps hidden assumptions out of the derivation, and the same refusal makes the corpus readable without a programming background. The marked breaks are not pedagogy alone — in a domain unlike prior media, the point where an analogy fails is usually where the content lives.

**Reopens if.** Never expected.

### <span id="dr-title">DR-19 — The title</span>

**Decision.** _Software Work Under Delegation._

**Instead of.** _Foundations of Software Production under Delegation_ (more precise, viable as an umbrella for later framework volumes; long and administrative in tone) and _The Medium, the Wanting, and the Actors_ (names the axioms themselves, welcoming to lay readers; says "software" only through a subtitle and resists search).

**Because.** The chosen title names the _derived_ subject — software work under delegation — rather than any kind of actor or a claim about document form. That wording puts a central finding on the cover: the arrival of machine producers moved the parameters of software work, not its ontology.

**Reopens if.** The corpus becomes one volume among several; the umbrella option returns.

### <span id="dr-this-record">DR-20 — This record's own shape</span>

**Decision.** A single anchored, append-and-mark log beside the README (`decisions.md`); entries carry decision, alternatives, reasons, and a reopening condition; the voice is editorial; nothing load-bearing cites it.

**Instead of.** One file per decision (disproportionate at this scale, and against the corpus's single-file idiom), or a narrative design history (unappendable, and prone to burying decisions in prose).

**Because.** The corpus's own directions prescribe the elements: closed decisions surfaced, reasons recorded durably, supersession kept cheap and visible. The reopening condition is the load-bearing field — a decision log that only memorializes hardens into the false authority T8 warns of; stating each entry's overturn condition keeps the record subordinate to present judgment.

**Reopens if.** The log outgrows single-file navigation — at which point splitting it is itself an entry.
