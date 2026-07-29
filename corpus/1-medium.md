# Axiom 1 — The Medium

> **Software is text whose entire worth lies in the behavior it causes when it runs. The text is almost free to change; what it will do can never be fully known from the text alone.**

This is one of three foundation documents. Each characterizes one element of software work: the medium (this document), the wanting ([Axiom 2 — Intent](2-intent.md)), and the participants ([Axiom 3 — Actors](3-actors.md)). The overview and full index live in the [README](README.md).

## Contents

- [Statement](#statement)
- [Commentary](#commentary)
- [Consequences](#consequences)
- [Descendants homed elsewhere](#elsewhere)

## <span id="statement">Statement</span>

The axiom is stated in four clauses. Together they characterize software as a working material — the way an engineer would characterize steel or timber: what it costs to shape, how its effects travel, and what can be known about it. All four are facts about the material itself, prior to anyone wanting anything from it and prior to any particular participant working on it.

### <span id="1a">1a — Enactment</span>

Software exists as text: a written artifact that can be read, stored, and copied exactly, at almost no cost. Its worth, however, lies entirely in the behavior that arises when a machine runs it. The text is the means; the behavior is the point.

### <span id="1b">1b — Situation</span>

Behavior does not arise from the text alone. It arises from the text together with an environment:

- the machines it runs on
- the information it is given
- the other software it relies on and encounters
- the people and systems that interact with it
- and the moment at which all of this happens

The text does not control its environment, and the environment does not stand still.

### <span id="1c">1c — Malleability without locality</span>

The text can be changed — any part of it, to any degree — and the act of making a change costs almost nothing. But the medium offers no built-in relationship between the size or place of a change and the size or place of its consequences. Nothing confines an effect to the neighborhood of its cause.

### <span id="1d">1d — Opacity</span>

No amount of reading or analysis of the text can fully disclose its behavior. Observing the software actually running is irreplaceable — and any set of observations, however large, covers only a fraction of the behavior that is possible.

## <span id="commentary">Commentary</span>

This section fixes what the axiom means, what its words cover, and what it does not claim.

A note on analogies before they appear: software resembles familiar kinds of writing — recipes, musical scores, contracts — and this document will borrow those resemblances to explain itself. But each clause of the axiom marks a place where the resemblance breaks down. The breaks are the content. Where an analogy is used, the point at which it fails will be marked, because the failure is usually the lesson.

### <span id="terms">Terms used in this document</span>

- **Text.** Any arrangement of symbols that a machine can follow. This is broader than words meant for human reading: program code is text, but so is a configuration file, a formula in a spreadsheet, and the learned numerical parameters inside a machine-learning model. The last of these is text that no person can read at all — an extreme this document returns to.
- **Software / program / system.** Used interchangeably here for text-that-runs, whether small or vast.
- **Running (execution).** A machine following the text step by step, exactly, at enormous speed, for as long as asked, without understanding anything. The machine does what the text says — never what anyone meant. If the text and the wish behind it differ, the machine sides with the text, every time, without noticing that a wish existed. This literalness is not a defect of current machines; it is what executing a text _is_.
- **Behavior.** Everything that happens in the world because the software ran: information displayed, stored, sent, or destroyed; decisions made; money moved; machinery actuated. Behavior is events in the world, not a property of the page.
- **Artifact.** Any made, storable thing. Here, chiefly the text itself and the durable records that accumulate around it.
- **Checking (verification).** Any deliberate effort to learn whether behavior is acceptable. **Assurance** is the accumulated grounds for confidence that it is.
- **Bedrock.** Facts imported from outside this theory's domain — settled results of computer science, plain facts about the world — used without argument and marked as such where they appear.

### <span id="1a-commentary">On 1a — Enactment</span>

A recipe is also a text of instructions, but a recipe's value passes through a cook — someone who understands the goal, tastes as they go, and repairs the instructions' gaps with judgment. Software's reader is the machine, and the machine brings no such repair (see _Running_, above). Whatever the text says happens; nothing the text fails to say happens on its behalf. So the worth of software cannot be located in the text's eloquence, cleverness, or beauty. It is located in what the text, followed literally, goes on to do.

Two boundaries on this clause.

First, 1a does **not** say that qualities of the text are worthless. Clarity, organization, and simplicity of the text matter — but instrumentally, not intrinsically. The text is also the workpiece for every _future_ change (1c), and future behavior will come from changed text. Textual virtues are investments in tomorrow's behavior: they make coming changes cheaper and safer to make and to re-check. The rule this clause imposes is only this: any virtue claimed for the text must be redeemable in behavior — today's or a future day's. A virtue that can never cash out that way is decoration.

Second, the clause's opening — read, stored, and _copied exactly, at almost no cost_ — is load-bearing, not scene-setting. Exact copying is what later makes it possible to rehearse software away from the real world ([T5](#t5)) and to say precisely which version of the text a piece of evidence was about ([T3](#t3)).

### <span id="1b-commentary">On 1b — Situation</span>

A hammer works the same in any house. Software is not like that: a system that ran perfectly yesterday can fail today with not one symbol of its text changed, because something it stood on — another program, a machine, a data format, a service operated by strangers — moved.

What the environment includes deserves spelling out, because each part carries consequences developed later:

- **Other software.** Nearly all software leans on software written elsewhere — borrowed parts, platforms, services. In any system of consequence, most of the text that determines behavior was written by people and machines who have never heard of the system it now serves.
- **People and other parties.** The environment is not neutral. It includes users who behave unexpectedly, and it includes parties who probe and push deliberately, seeking behavior the software's makers never wanted to exist.
- **Time and coincidence.** No two runs are guaranteed identical circumstances. Timing, load, and chance are part of the environment too.

The boundary of the clause: 1b does **not** say the text controls nothing. The text fully determines its own instructions; what it cannot determine is the situation those instructions meet. The result — behavior — is decided jointly. One consequence is worth stating early: every guarantee anyone ever offers about software is conditional. It has the form _"provided the environment honors these assumptions…"_ — and reality is not obligated to honor them.

### <span id="1c-commentary">On 1c — Malleability without locality</span>

Physical media discipline the people who work in them. In a bridge, a small change is small, a large change is costly, and effects sit near their causes; the material itself enforces this. Software's medium enforces nothing of the kind. Editing one character costs the same near-nothing as editing thousands, and the medium offers no promise that the effects of either will stay near the edit.

Why effects travel: software is built of parts that refer to and depend on other parts. Consequence moves along those lines of reference, not along physical adjacency. A long contract behaves a little like this — amend clause 12 and clause 3 may silently change in force, which is why careful lawyers re-read amendments against the whole. But the analogy breaks in software's disfavor: a contract is ultimately read by people, who can notice an absurd result and reach for what the parties must have meant. Software's reader executes the absurdity, at full speed, without flagging it.

The absence of locality runs in both directions, and this matters: a sweeping edit can turn out to change behavior barely at all, and a one-character edit can change everything. Neither the size nor the place of an edit is, by itself, evidence about the size or place of its effects. Any working rule that says otherwise — "it was a small change, so the risk is small" — is not a fact about the medium. At best it is a fact about _constructed_ containment, which somebody built and somebody must maintain.

Two boundaries. First, the near-zero cost refers to the mechanical act of editing. Deciding _what_ to change can be as hard as anything in this field — that difficulty descends from opacity (1d) and from the nature of intent (Axiom 2), not from the medium's resistance. The full act of changing _responsibly_ costs far more than the edit; that is the subject of [T3](#t3).

Second, 1c does **not** claim every change does reach everywhere — most changes, in practice, stay put. The claim is that nothing in the medium _guarantees_ it. Where containment exists, it was engineered, and it can be wrong. The engineering of containment is treated under [T14 — Structure is how bounded actors survive scale](3-actors.md#t14).

### <span id="1d-commentary">On 1d — Opacity</span>

This is the strangest clause to anyone who has not worked in the medium, because it seems to insult the text: the instructions are all _right there_, complete and exact — how can they not disclose what they will do? Three separate grounds, each sufficient to establish the clause, all three operating at once:

1. **A limit of logic.** It is a settled result of computer science — proven in the strong, mathematical sense — that there can be no general method, however clever and however well-resourced, that answers every question about what an arbitrary program will do. (The field calls this family of results _undecidability_.) This is bedrock, not a complaint about today's tools; no future tool escapes it.
2. **A limit of scale.** Even where analysis is possible in principle, the number of distinct situations a system can face — combinations of inputs, timings, and surroundings — exceeds, for any system of consequence, anything that could ever be enumerated. Not "difficult to enumerate": beyond any feasible resources, permanently. Every checking effort, however vast, is a sample.
3. **The situation.** Behavior is made jointly by text and environment (1b). Analysis of the text alone, however perfect, cannot speak for surroundings it has not seen — and the surroundings will not hold still to be seen.

The boundaries of the clause matter as much as its force:

- 1d does **not** say reading is worthless. Inspection narrows the possibilities enormously; it rules things out, directs attention, and catches whole categories of error before any run. The clause bars only _completeness_.
- 1d does **not** say proof is impossible. For specific, stated properties, under stated assumptions, mathematics can certify software absolutely — a real and valuable practice. But the certificate is conditional on its assumptions about the environment (1b), and it covers the properties someone thought to state, not behavior entire.
- Opacity is impartial: it binds every reader of the text — **including its writer**. Whoever or whatever wrote a piece of software holds, at best, a good partial theory of what it does. Ordinary writing offers no true parallel here: a novelist may misjudge how a novel will be received, but a novel does not go on to _do things_ its author never learned of. Software does. (This fact — the author has no privileged sight of behavior — becomes load-bearing when the theory turns to the participants, in [Axiom 3](3-actors.md).)
- Some software deepens the clause further: systems with deliberate randomness, timing-sensitive parts, or learned components can behave differently on the same apparent occasion twice. And the learned numerical parameters of a machine-learning model are the clause's extreme case — text, in this document's sense, that no one can read at all, whose behavior is known almost _only_ through observation.

### <span id="clause-audit">Why these four clauses</span>

The test for each clause is what becomes underivable if it is cut, and whether any clause can be derived from the others.

- **Cut 1a**, and nothing anchors why behavior — rather than the text's own qualities — is the criterion of worth; checking loses its object, and real-world stakes ([T5](#t5)) lose their weight.
- **Cut 1b**, and behavior becomes a fixed property of the text: once checked, checked forever ([T4](#t4) collapses), rehearsal would equal reality ([T5](#t5) loses its hard part), and guarantees would be unconditional.
- **Cut 1c**, and the medium itself would discipline change — by cost or by containment — and the economics of re-trust ([T3](#t3)) would vanish, along with the need to construct boundaries at all.
- **Cut 1d**, and reading could substitute for running: [T1](#t1) and [T2](#t2) collapse, and checking becomes optional in principle.

None follows from the rest: a medium could be transparent yet rigid (1c without 1d), or opaque in a frozen world (1d holds even without 1b, by the limit of logic alone), and a moving world would surround software even if its text were somehow transparent (1b without 1d). Each clause does work the others cannot.

## <span id="consequences">Consequences</span>

Five theorems are homed under this axiom, all descending primarily from it. (T6–T8 and T13 are homed under [Axiom 2](2-intent.md#consequences), T9–T12 and T14 under [Axiom 3](3-actors.md#consequences); numbering is corpus-wide and indexed in the [README](README.md).) _Theorem_ is used in the argued sense, not the formal one: each is a consequence reasoned from the axiom's clauses — and, where marked, from bedrock facts or from clauses of the companion axioms — stated so that the reasoning can be inspected and attacked. Under each theorem sit its **engineering directions**: problems that any framework governing software work must solve, stated as problems, not as designs. (_Framework_ here means any deliberate way of organizing this work — rules, tools, roles, procedures.) Where current practice already has a name for a derived thing, the name is noted in parentheses; the note attaches a label, it does not import an authority.

### <span id="t1">T1 — All assurance is partial</span>

**Descends from [1d](#1d), with [1b](#1b).**

Knowledge of behavior comes only from observation (1d) — or, where mathematics can certify a stated property under stated assumptions, from a proof whose certificate is conditional on those assumptions and covers only the properties someone thought to state (1d commentary). Any body of observations is finite, and the situations a system can face are beyond enumeration (1d, the limit of scale). Meanwhile the environment that shaped past observations — and that any proof assumes — keeps moving (1b). So every honest claim of confidence in software has one of two forms: _"in the situations sampled so far, under the environment as it stood, nothing unacceptable was seen,"_ or _"provided these assumptions about the environment hold, this stated property is guaranteed."_ Confidence in software is a degree (or a conditional), never a settled fact about behavior entire, and there is no reachable state called _verified once and for all_.

**Engineering directions:**

#### <span id="d-verification-selection">Choosing what to check</span>

If exhaustive checking is impossible, a framework must say how finite checking effort is spent: weighted by

- how likely a situation is
- how costly its failure would be
- and how novel or recently disturbed the text is

(Current practice calls families of answers here _test strategy_ and _risk-based testing_.) How that weighting is set, argued about, and revised is a foundational design problem — and it joins the budget question treated under [T12 — Judgment is the scarce budget](3-actors.md#t12).

#### <span id="d-assurance-expression">Saying how sure</span>

If assurance is a degree, a collaboration needs a shared way to express the degree, attach it to the work it describes, and act on it — something richer than a binary pass/fail. Open design questions:

- What granularity it takes
- what it attaches to
- and how it decays as text and environment move

#### <span id="d-operating-detection">Expecting escapes</span>

Partial assurance means some unacceptable behavior _will_ reach real use, given enough time. Noticing it there must be a designed capability — instrumented observation of software as it runs in earnest (current practice: _monitoring_, _observability_) — together with prepared paths from noticing to response. [T4](#t4) compounds this need: even assurance that was valid when earned decays as the world moves.

### <span id="t2">T2 — Questions of behavior are settled by running</span>

**Descends from [1d](#1d); co-parent [3c — no self-certification](3-actors.md#3c).**

If the text cannot fully disclose behavior (1d), then a disagreement about behavior cannot be finally settled by argument over the text — nor by anyone's rank, confidence, or eloquence (co-parent 3c: no participant's say-so is self-validating). Execution is the only tribunal whose verdict does not depend on who is speaking. **In questions of behavior, a demonstration outranks any assertion, whoever asserts.**

Two qualifications keep the tribunal honest. A run settles exactly the case that ran, no more ([T1](#t1)); and a behavior seen once can in principle be made to happen again by controlling enough of the environment (bedrock: machines follow text exactly), though arranging that control is real work, not a given.

**Engineering directions:**

#### <span id="d-cheap-demonstration">Making "run it" cheap</span>

The tribunal is only used if it costs less than the argument it replaces. A framework must provide the standing machinery that makes demonstration the default move: execution contexts ready to hand, and cheap faithful reproduction of any behavior someone reports. What must exist so that reproducing a reported behavior is an act of minutes rather than days?

#### <span id="d-evidence-scope">Recording what a run did and did not establish</span>

A passing demonstration ends a specific question, and human institutions are prone to let it quietly expand into a general certificate. Frameworks need discipline — probably notation — for the _scope_ of any demonstration: which situations it sampled, under which environment, so that its authority ends where its sampling ended.

One forward note: demonstrations are made things, produced by some participant, and whether a produced demonstration can be trusted is a question about participants, not about the medium. It is treated under [T9 — Testimony is not evidence](3-actors.md#t9).

### <span id="t3">T3 — Change is cheap; re-trust is not</span>

**Descends from [1c](#1c) + [1d](#1d).**

Making a change costs almost nothing, and the medium does not confine the change's effects to its neighborhood (1c). Knowing what the changed whole now does requires fresh observation (1d). Put together: after any edit, yesterday's confidence is, strictly speaking, confidence about yesterday's text. Assurance does not survive change by default. So the true cost of a change is dominated not by making it but by re-establishing that the whole still behaves acceptably — **the economics of software work are the economics of re-trust, not of typing.**

**Engineering directions:**

#### <span id="d-change-reach">Bounding a change's reach</span>

Re-checking everything after every edit is unaffordable; not re-checking is unjustifiable. The escape is an argument of the form _"this change cannot have touched that."_ Where such arguments come from — constructed containment, per [T14](3-actors.md#t14) — and when they deserve belief (they are themselves fallible claims about an opaque medium) is a central problem. (Current practice: _impact analysis_; _regression testing_, named for the discovery that a behavior which was acceptable has silently stopped being so — a _regression_.)

#### <span id="d-change-shape">Sizing and batching change</span>

If re-trust cost scales with a change's possible reach, then the size and shape of changes is a design variable, not an accident of workflow: many small, separately re-trusted steps versus few large ones; what makes a change separately checkable at all. (Current practice: small _pull requests_, atomic commits.)

#### <span id="d-evidence-binding">Binding evidence to exact text</span>

Text changes freely (1c) and assurance is specific to the text it was earned on. A collaboration therefore needs to name the _exact_ state of the text that any piece of evidence was about, and to notice when an edit has orphaned old evidence. (Current practice: _version control_; recording every check against a named, exact version.) This machinery also serves the collaboration's memory, treated under [T10](3-actors.md#t10).

### <span id="t4">T4 — Unchanged software still drifts</span>

**Descends from [1b](#1b), with bedrock (the world changes on its own).**

Behavior is made jointly by text and environment (1b), and the environment moves without asking permission (bedrock). So behavior — and fitness, and the validity of every past observation — moves while the text sits still. Software left alone does not stay as it was. It stays only as it was _written_, and what its unchanged text does is decided jointly with a world that keeps moving. **"Finished" is not a stable state of software; it is a statement about attention.**

**Engineering directions:**

#### <span id="d-tending">Tending as a standing function</span>

Work on software cannot be modeled as ending at hand-off. A framework must allocate standing attention to systems nobody is changing: watching their operation ([T1](#t1)'s detection), re-validating their assumptions when the surroundings move, and treating even the decision to _stop_ tending as an explicit act with consequences — abandonment is a decision, not a default. What is watched, what triggers re-validation, and who or what carries this standing duty are the design questions.

#### <span id="d-leanings">Keeping an account of what the software leans on</span>

The environment is not a fog; software leans on nameable things — borrowed parts, platforms, services, formats, counterparty systems. A framework needs those leanings recorded and kept current (current practice: dependency manifests — a maintained list of what the software borrows), so that news of movement in the world can be translated into the question _"what of ours does this touch?"_ This is [T3](#t3)'s reach-bounding problem run in reverse: there the change is ours and the world is still; here the change is the world's.

### <span id="t5">T5 — Some runs are rehearsals; some are real</span>

**Descends from [1a](#1a) + [1b](#1b) + [1d](#1d), with bedrock (some events cannot be undone).**

Software's worth is behavior in the world (1a), behavior reaches the world through the environment (1b), and the world contains events that cannot be taken back (bedrock):

- messages sent
- money moved
- records destroyed
- machinery actuated

Meanwhile, learning what software does requires running it, abundantly (1d, [T1](#t1)). The medium therefore carries a standing tension: the thing that must be done freely in order to learn is the same thing that can do harm. The resolution has to be engineered, because the medium does not provide it: separate execution whose effects do not count — rehearsal — from execution whose effects do, and govern the crossing between them.

One consequence follows immediately and must not be lost: rehearsal is approximation. A rehearsal environment is a _different_ environment (1b), so rehearsal evidence is evidence about a stand-in. How faithfully the stand-in predicts the real thing is a property to be measured and maintained, never presumed.

**Engineering directions:**

#### <span id="d-rehearsal-spaces">Rehearsal spaces</span>

Execution contexts insulated from consequence — exact copies of the software (1a's copyability) running against stand-in surroundings. (Current practice: _sandboxes_, test environments, _staging_.) The framework problems: how such spaces are constructed, how their fidelity to reality is kept honest, and what a rehearsal can and cannot certify given that fidelity.

#### <span id="d-the-crossing">The crossing</span>

Moving behavior into real use (current practice: _release_, _deployment_) is the moment partial assurance ([T1](#t1)) meets irreversible stakes. Frameworks need explicit crossing designs:

- graduated exposure — a little reality at a time
- engineered reversibility — undo is constructed, never given, because the medium comes with no take-backs
- and prepared abort paths

(Current practice: canary releases, rollbacks, feature flags.)

#### <span id="d-consequence-classes">Consequence-classing the work itself</span>

Production is itself execution: whoever — or whatever — is doing the work runs things constantly while working. The rehearsal/real line therefore runs _through_ the workspace, not just around the finished product. Every action available during the work belongs to a consequence class — freely repeatable, costly, or irreversible — and the consequential classes need gates. Where the gates sit and who may open them is a question about decision authority, treated under [T6 — Every act of production decides unstated things](2-intent.md#t6).

## <span id="elsewhere">Descendants homed elsewhere</span>

Clauses of this axiom serve as co-parents to theorems homed under the companion axioms:

- [1a — Enactment](#1a) → [T6 — Every act of production decides unstated things](2-intent.md#t6)
- [1c — Malleability without locality](#1c) → [T14 — Structure is how bounded actors survive scale](3-actors.md#t14)
- [1d — Opacity](#1d) → [T7 — Intent is discovered through the loop](2-intent.md#t7)
- [1d — Opacity](#1d) → [T9 — Testimony is not evidence](3-actors.md#t9)
- [1d — Opacity](#1d) → [T13 — Intent wants to become executable](2-intent.md#t13)

The corpus-wide derivation graph, including theorem-to-theorem uses, is indexed in the [README](README.md).
