# Software Work Under Delegation

> Three axioms — about the medium, the wanting, and the participants — from which the practices of software work can be derived rather than inherited. Stated so that they hold whether the parties are people, machines, or both, and so that they stay standing as capabilities move.

## Contents

- [What this is](#what-this-is)
- [How to read and adopt](#adoption)
- [Bedrock](#bedrock)
- [The setting](#setting)
- [The three axioms](#axioms)
- [The derivation graph](#graph)
- [The engineering directions index](#directions)
- [The razor audit](#audit)
- [Amendment rules](#amendments)
- [The corpus](#corpus)

## <span id="what-this-is">What this is</span>

Software work has always had the same shape: some party wants behavior in the world, and some party produces the text that causes it. But the field's inherited practices — how work is planned, reviewed, trusted, handed off — grew up during a long era in which one kind of actor did all the producing, and they quietly encode that era's facts: production slow and expensive, judgment relatively plentiful, participants persistent and few. Those facts have moved. Software now writes software at scale; production can be fast, cheap, parallel, and episodic. Practices tuned to the old profile fail without announcing it, because their assumptions were never written down as assumptions.

This body of theory is the response: instead of patching practices, write down the facts that never moved. It consists of three axioms — one about software as a material ([the Medium](1-medium.md)), one about wanting software ([Intent](2-intent.md)), one about those who do the work ([Actors](3-actors.md)) — carrying eleven clauses in all. From these, fourteen theorems are derived, and under the theorems, forty-one engineering directions: problems any framework governing software work must solve. **What is derived can be re-derived when circumstances shift; what is merely inherited can only be defended or abandoned.** Much of what the theorems produce is deliberately familiar — version control, regression testing, staging environments, review all reappear — because a derivation does two things a tradition cannot: it explains _why_ a practice exists, and it shows _which of its features_ were contingent on a profile-era that has ended.

What this is not: a methodology, a tool guide, or a policy document — norms and obligations enter the theory only as constraints held by some party, never as annexed subject matter. Its unit of analysis is deliberately small — one delegating party, one producing party, and the artifacts between them — and larger arrangements are composed from that unit ([the setting](#setting) gives the mechanisms). It assumes no programming background: every term of art is introduced in plain language before use, analogies carry their breaking points marked, and names from current practice appear in parentheses as labels, never as authorities.

## <span id="adoption">How to read and adopt</span>

The corpus is layered by rate of change, and it is meant to be entered shallowly and inhabited progressively.

### Depth 0 — the lens (minutes)

Read the three axiom statements at the top of each axiom document. Then carry four questions into any piece of software work:

1. _What unstated decisions is this work closing, and should any have been surfaced?_ ([Axiom 2](2-intent.md), [T6](2-intent.md#t6))
2. _What evidence stands behind this claim, beyond its maker's say-so?_ ([Axiom 3](3-actors.md), [T9](3-actors.md#t9))
3. _Which durable record will hold what this episode learned, once the episode ends?_ ([3a](3-actors.md#3a), [T10](3-actors.md#t10))
4. _Would today's confidence survive a change to the text — or a change in the world?_ ([Axiom 1](1-medium.md), [T3](1-medium.md#t3), [T4](1-medium.md#t4))

### Depth 1 — the reasoning

Read the commentary and theorems. Use them to audit existing practice: for each rule or habit in force, find the theorem it descends from. A practice with no derivation is one of three things — a missing theorem (file an amendment), era-furniture (see [T11's audit](3-actors.md#d-era-audit)), or an external constraint held by some party and entering the work as an expression of intent, not as a framework rule.

### Depth 2 — the directions

Build on the engineering directions: a framework, a tool, a working agreement. Every component built should cite the direction anchors it answers; that citation habit is what keeps the [traceability chain](#graph) unbroken from running code all the way back to an axiom clause.

Navigation conventions, corpus-wide:

- clauses carry anchors `1a`–`3d`
- theorems `t1`–`t14`
- directions `d-…` (name-based, insertion-proof)
- Every theorem opens with a **Descends from** line linking its parents
- every direction sits inside its theorem's section
- Anchors are permanent once published.

## <span id="bedrock">Bedrock</span>

Facts imported whole from outside this theory's domain, used without argument and marked where they appear:

1. Machines follow text exactly, at great speed, at negligible marginal cost.
2. No general method can answer every question about what an arbitrary program will do.
3. Communication between parties never guarantees identical understanding.
4. When one party acts for another, information and aims can diverge.
5. The world changes on its own.
6. Some events cannot be undone.

The axioms are not restatements of bedrock; they are the domain-level facts that bedrock licenses, stated where they do work. Finitude and fallibility of participants are stated at domain level in [Axiom 3](3-actors.md), not imported here — so the deletion tests below can still do their work.

## <span id="setting">The setting</span>

The theory's subject is **software production under delegation**: one party turns production over to another while retaining authority over whether the result fits.

### Two roles

The **delegator** holds authority over fit — its present intent is what behavior must satisfy ([Axiom 2](2-intent.md)). The **producer** does the work of production. These are roles, not kinds of being: either may be a person, a group, or software itself, and the theory's rules never depend on which ([T11](3-actors.md#t11) derives why they must not).

### The shared record between them

Everything durable the collaboration has — the software's text, the record of intent, the evidence — lives in artifacts both roles can reach ([T10](3-actors.md#t10)). The collaboration's memory is exactly this record.

### Why delegation happens

Commonly, for leverage: the delegator seeks more accepted behavior per unit of its own effort and judgment. (Not universally — delegation for training or redundancy exists — but leverage is the case that shapes the economics: [T9](3-actors.md#t9), [T12](3-actors.md#t12).)

### Relations, not appointments

The dyad is relational and composable. A producer that delegates part of its work onward is the delegator of that further dyad; every axiom and theorem applies at every link unchanged, because all are stated over roles. Roles may also be _re-occupied_: the work persists indefinitely ([T4](1-medium.md#t4), [T7](2-intent.md#t7)) while occupants change, and nothing ties a role to one actor for the work's life. Even the degenerate case obeys the theory: an actor working alone holds both roles, and the axioms still bite — self-trust is bounded by [3c](3-actors.md#3c), and notes to a future self are notes to what is, for every purpose here, another actor ([3a](3-actors.md#3a)).

### Composition

Larger structures are built from dyads under one invariant: **every producer faces exactly one delegator-side corpus of expressions.** Multiplicity of authority is always resolved _into_ that corpus — by explicit precedence marks and adjudication — never left for the producer to arbitrate case by case. The three shapes:

#### Chains

A delegates to B, B to C. Constraints from further up enter the nearer dyad on its delegator side, carrying precedence marks — _binding_ (the far constraint prevails and conflicts surface upward) or _advisory_ (the near instruction prevails). The mechanism is [T8's authority-ordering](2-intent.md#d-expression-authority); its enforcement half is [T12's escalation design](3-actors.md#d-escalation-design). C never faces two delegators; it faces B, holding one corpus with marked strata.

#### Fan-out

One delegator, many producers:

- Scope is partitioned ([T14](3-actors.md#t14))
- producers meet at seams governed by stated promises ([Promises at the seams](3-actors.md#d-seam-promises))
- coordination flows through the shared record ([T10](3-actors.md#t10))
- conflicts peers cannot settle at a seam escalate to the common delegator.

#### Fan-in

Multiple delegators over one producer — _not a primitive the theory grants._ It must be composed away:

- merge the authorities upstream into a single marked corpus (one dyad)
- or partition the producer's scope into disjoint dyads
- or refuse the assignment until one of those compositions is done

Escalation has a target only where a common superior can perform the merge; without one, refusal is the remaining move. A producer holding two unmerged authorities over one scope has an undefined task, and no framework should pretend otherwise.

One reflexive note: the collaboration's own machinery — its checks, records, and rules, wherever they are executable — is software, and every claim in this corpus applies to it.

## <span id="axioms">The three axioms</span>

### [Axiom 1 — The Medium](1-medium.md)

_Software is text whose entire worth lies in the behavior it causes when it runs. The text is almost free to change; what it will do can never be fully known from the text alone._

**Clauses:**

- [1a — Enactment](1-medium.md#1a)
- [1b — Situation](1-medium.md#1b)
- [1c — Malleability without locality](1-medium.md#1c)
- [1d — Opacity](1-medium.md#1d)

### [Axiom 2 — Intent](2-intent.md)

_What software should do exists only as finite expressions of intent; every expression leaves most behavior undecided, and no expression is final._

**Clauses:**

- [2a — Expression-boundedness](2-intent.md#2a)
- [2b — Underdetermination](2-intent.md#2b)
- [2c — Motion and present authority](2-intent.md#2c)

### [Axiom 3 — Actors](3-actors.md)

_Every participant in software work — human or machine, producing or judging — is bounded, fallible, and unable to certify its own work; and participants differ from one another in ways that keep changing._

**Clauses:**

- [3a — Boundedness](3-actors.md#3a)
- [3b — Fallibility](3-actors.md#3b)
- [3c — No self-certification](3-actors.md#3c)
- [3d — Heterogeneity in motion](3-actors.md#3d)

## <span id="graph">The derivation graph</span>

Every theorem opens with a **Descends from** line naming its parents — clauses, plus the [setting](#setting), [bedrock](#bedrock), and any earlier theorems serving as premises. In the table below, clauses, setting, and bedrock fill the _Descends from_ column; the _Uses_ column is mechanical — it lists every _earlier_ theorem cited in the theorem's own prose, premises included, directions excluded. A reference to a _later_ theorem is a forward pointer, never a dependency: it may appear in a theorem's prose, never in this column — which keeps the graph acyclic by construction. Junction theorems draw equally on two axioms and are homed with the axiom bearing their subject.

| #                      | Theorem                                                | Home          | Descends from                                                                                                         | Uses                       |
| ---------------------- | ------------------------------------------------------ | ------------- | --------------------------------------------------------------------------------------------------------------------- | -------------------------- |
| [T1](1-medium.md#t1)   | All assurance is partial                               | A1            | [1d](1-medium.md#1d), [1b](1-medium.md#1b)                                                                            | —                          |
| [T2](1-medium.md#t2)   | Questions of behavior are settled by running           | A1            | [1d](1-medium.md#1d), [3c](3-actors.md#3c)                                                                            | T1                         |
| [T3](1-medium.md#t3)   | Change is cheap; re-trust is not                       | A1            | [1c](1-medium.md#1c), [1d](1-medium.md#1d)                                                                            | —                          |
| [T4](1-medium.md#t4)   | Unchanged software still drifts                        | A1            | [1b](1-medium.md#1b), bedrock                                                                                         | —                          |
| [T5](1-medium.md#t5)   | Some runs are rehearsals; some are real                | A1            | [1a](1-medium.md#1a), [1b](1-medium.md#1b), [1d](1-medium.md#1d), bedrock                                             | T1                         |
| [T6](2-intent.md#t6)   | Every act of production decides unstated things        | A2            | [2b](2-intent.md#2b), [setting](#setting), [1a](1-medium.md#1a)                                                       | T5                         |
| [T7](2-intent.md#t7)   | Intent is discovered through the loop                  | A2            | [2a](2-intent.md#2a), [2b](2-intent.md#2b), [2c](2-intent.md#2c), [1d](1-medium.md#1d)                                | T5                         |
| [T8](2-intent.md#t8)   | The record of intent is maintained, never finished     | A2            | [2a](2-intent.md#2a), [2c](2-intent.md#2c)                                                                            | T4, T6                     |
| [T9](3-actors.md#t9)   | Testimony is not evidence                              | A3            | [3c](3-actors.md#3c), [1d](1-medium.md#1d), [setting](#setting)                                                       | T2, T3                     |
| [T10](3-actors.md#t10) | What is not in the shared record is lost               | A3            | [3a](3-actors.md#3a), [setting](#setting)                                                                             | T4, T6, T7, T8, T9         |
| [T11](3-actors.md#t11) | Rules must bind roles and profiles, not kinds of actor | A3            | [3d](3-actors.md#3d), [setting](#setting)                                                                             | —                          |
| [T12](3-actors.md#t12) | Judgment is the scarce budget                          | A3            | [3a](3-actors.md#3a), [3b](3-actors.md#3b), [3c](3-actors.md#3c), [3d](3-actors.md#3d), [setting](#setting)           | T1, T5, T6, T8             |
| [T13](2-intent.md#t13) | Intent wants to become executable                      | A2 (junction) | [2b](2-intent.md#2b), [2c](2-intent.md#2c), [1d](1-medium.md#1d), [3a](3-actors.md#3a), [3c](3-actors.md#3c), bedrock | T1, T2, T3, T6, T7, T8, T9 |
| [T14](3-actors.md#t14) | Structure is how bounded actors survive scale          | A3 (junction) | [3a](3-actors.md#3a), [1c](1-medium.md#1c)                                                                            | T3, T4, T7, T10            |

Cross-axiom co-parentage is also indexed at each axiom document's _Descendants homed elsewhere_ section, so the graph can be walked from either end.

## <span id="directions">The engineering directions index</span>

Every concrete engineering concern the theory points toward, grouped under its theorem. Each link lands on the direction's own anchor; from there, the theorem's _Descends from_ line completes the chain back to an axiom clause.

- **T1 — All assurance is partial**
  - [Choosing what to check](1-medium.md#d-verification-selection)
  - [Saying how sure](1-medium.md#d-assurance-expression)
  - [Expecting escapes](1-medium.md#d-operating-detection)
- **T2 — Questions of behavior are settled by running**
  - [Making "run it" cheap](1-medium.md#d-cheap-demonstration)
  - [Recording what a run did and did not establish](1-medium.md#d-evidence-scope)
- **T3 — Change is cheap; re-trust is not**
  - [Bounding a change's reach](1-medium.md#d-change-reach)
  - [Sizing and batching change](1-medium.md#d-change-shape)
  - [Binding evidence to exact text](1-medium.md#d-evidence-binding)
- **T4 — Unchanged software still drifts**
  - [Tending as a standing function](1-medium.md#d-tending)
  - [Keeping an account of what the software leans on](1-medium.md#d-leanings)
- **T5 — Some runs are rehearsals; some are real**
  - [Rehearsal spaces](1-medium.md#d-rehearsal-spaces)
  - [The crossing](1-medium.md#d-the-crossing)
  - [Consequence-classing the work itself](1-medium.md#d-consequence-classes)
- **T6 — Every act of production decides unstated things**
  - [Drawing the boundary](2-intent.md#d-boundary-drawing)
  - [Making closed decisions inspectable](2-intent.md#d-decision-surfacing)
  - [Asking versus assuming](2-intent.md#d-ask-vs-assume)
- **T7 — Intent is discovered through the loop**
  - [The loop as the unit of work](2-intent.md#d-loop-unit)
  - [Cheapening encounters](2-intent.md#d-encounter-cost)
  - [Capturing the yield](2-intent.md#d-encounter-capture)
- **T8 — The record of intent is maintained, never finished**
  - [An authority-ordering among expressions](2-intent.md#d-expression-authority)
  - [Reconciliation as standing work](2-intent.md#d-record-reconciliation)
  - [Cheap, visible supersession](2-intent.md#d-cheap-supersession)
- **T9 — Testimony is not evidence**
  - [The evidence bundle](3-actors.md#d-evidence-bundle)
  - [Gaming resistance](3-actors.md#d-gaming-resistance)
  - [Testimony's proper rank](3-actors.md#d-testimony-rank)
- **T10 — What is not in the shared record is lost**
  - [What must be recorded](3-actors.md#d-record-scope)
  - [Episode boundaries as record events](3-actors.md#d-episode-handoff)
  - [Loading within bounds](3-actors.md#d-bounded-loading)
- **T11 — Rules must bind roles and profiles, not kinds of actor**
  - [A role vocabulary with defined powers](3-actors.md#d-role-vocabulary)
  - [Profiles as maintained measurements](3-actors.md#d-profile-currency)
  - [Auditing rules for encoded eras](3-actors.md#d-era-audit)
- **T12 — Judgment is the scarce budget**
  - [Risk-routing as explicit policy](3-actors.md#d-risk-routing)
  - [Calibrated trust](3-actors.md#d-calibrated-trust)
  - [Escalation design](3-actors.md#d-escalation-design)
- **T13 — Intent wants to become executable**
  - [The migration ratchet](2-intent.md#d-executable-migration)
  - [Honest accounting of the floor](2-intent.md#d-floor-coverage)
  - [Checks as tended intent](2-intent.md#d-check-maintenance)
- **T14 — Structure is how bounded actors survive scale**
  - [Partitioning for bounded change](3-actors.md#d-partition-for-change)
  - [Promises at the seams](3-actors.md#d-seam-promises)
  - [Convention as comprehension subsidy](3-actors.md#d-convention-subsidy)
  - [Concurrent production](3-actors.md#d-concurrent-production)

## <span id="audit">The razor audit</span>

The axiom set claims two properties — minimal completeness and mutual independence — and both are checked directly rather than assumed.

### Necessity, by deletion

- Remove [Axiom 1](1-medium.md) and reading could substitute for running: checking becomes optional in principle, re-verification after change pointless, rehearsal indistinguishable from reality.
- Remove [Axiom 2](2-intent.md) and complete one-shot specification becomes available: production stops being decision-making, iteration is mere inefficiency, and a finished suite of checks could equal intent.
- Remove [Axiom 3](3-actors.md) and an oracle could exist: its testimony would suffice, shared records would be a convenience, and rules could safely name kinds of actor.

Each deletion collapses a distinct, indispensable region — verification, discovery, and trust respectively.

### Independence, as non-derivability

Axiom 1 holds for unwanted software and for ideal observers — it mentions neither intent nor actors. Axiom 2 holds even if behavior were fully transparent: seeing everything a system does would still not disclose whether it is wanted in situations not yet met. Axiom 3 holds even given complete specifications and transparent behavior: bounded, erring, self-blind participants would remain so. The axioms interact constantly downstream; independence here means none is derivable from the others. The same tests run at clause grain inside each document:

- [Axiom 1's audit](1-medium.md#clause-audit)
- [Axiom 2's audit](2-intent.md#clause-audit)
- [Axiom 3's audit](3-actors.md#clause-audit)

### Completeness, by sweep

Every phase of software work finds its ground:

- wanting and expressing ([2a](2-intent.md#2a), [2b](2-intent.md#2b))
- producing ([setting](#setting), [T6](2-intent.md#t6))
- knowing what it does ([1d](1-medium.md#1d), [T1](1-medium.md#t1), [T2](1-medium.md#t2))
- judging fit ([2c](2-intent.md#2c), [3c](3-actors.md#3c), [T9](3-actors.md#t9))
- accepting ([3c](3-actors.md#3c), [T5](1-medium.md#t5))
- operating ([1b](1-medium.md#1b), [T4](1-medium.md#t4))
- changing ([1c](1-medium.md#1c), [T3](1-medium.md#t3), [T7](2-intent.md#t7))
- remembering ([3a](3-actors.md#3a), [T8](2-intent.md#t8), [T10](3-actors.md#t10))
- coordinating at scale ([T14](3-actors.md#t14), [composition](#setting))
- trusting ([3b](3-actors.md#3b), [T12](3-actors.md#t12))

The sweep is refutable: a phenomenon of software work with no home in this list is a defect — file it as an amendment.

### Considered and cut

Candidates weighed for axiom status and placed lower, because the razor demanded it:

- _verification must be independent of production_ — derivable, now [T9](3-actors.md#t9)
- _iteration is fundamental_ — derivable, now [T7](2-intent.md#t7)
- _the artifacts are the ground truth_ — derivable, now [T10](3-actors.md#t10)
- _frameworks must not assume the parties' kinds_ — derivable, now [T11](3-actors.md#t11), which is stronger as a conclusion than it would have been as an assumption
- _communication is lossy_ — bedrock, not domain
- _delegation exists_ — the setting's definition, not a claim
- _machines now produce faster than people can review_ — a present-day profile measurement, outside the theory's domain; it may inform frameworks built on the directions, but nothing in this corpus depends on it.

## <span id="amendments">Amendment rules</span>

The corpus is layered by rate of change, and dependence points strictly downward: directions cite theorems, theorems cite clauses.

- **Directions** may be added at any time: nested under exactly one theorem, stating a problem rather than a design, carrying a new `d-` anchor. The [index above](#directions) is updated in the same change.
- **Theorems** may be added when they do work no existing theorem does: the amendment names parent clauses (plus setting or bedrock where used), lists theorem-uses, homes the theorem with the axiom bearing most of its weight, and adds co-parentage lines to the other parents' _Descendants homed elsewhere_ sections and to the [graph](#graph).
- **Clauses and axioms** change rarely and only under the full razor: the addition must pass the deletion test (something real becomes underivable without it), the independence test (it is not derivable from what stands), and a re-run of the completeness sweep.
- **Editorial invariants:**
  - anchors are permanent once published — titles may be reworded, identifiers may not
  - imported vocabulary always arrives as a parenthetical label after the derived concept, never before it
  - analogies state their breaking points.

## <span id="corpus">The corpus</span>

- [README](README.md) — this document: the spine, the setting, the graph, the audit, the rules.
- [1-medium.md](1-medium.md) — Axiom 1: the Medium. Theorems T1–T5.
- [2-intent.md](2-intent.md) — Axiom 2: Intent. Theorems T6–T8, T13.
- [3-actors.md](3-actors.md) — Axiom 3: Actors. Theorems T9–T12, T14.
