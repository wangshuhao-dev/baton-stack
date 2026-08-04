# Axiom 3 — Actors

> **Every participant in software work — human or machine, producing or judging — is bounded, fallible, and unable to certify its own work; and participants differ from one another in ways that keep changing.**

This is one of three foundation documents. Each characterizes one element of software work: the medium ([Axiom 1 — The Medium](1-medium.md)), the wanting ([Axiom 2 — Intent](2-intent.md)), and the participants (this document). The overview and full index live in the [README](README.md).

## Contents

- [Statement](#statement)
- [Commentary](#commentary)
- [Consequences](#consequences)
- [Descendants homed elsewhere](#elsewhere)

## <span id="statement">Statement</span>

The axiom is stated in four clauses. Together they characterize the participants: the limits each brings to an episode of work, the errors none escapes, the standing of any actor's word about its own work, and the differences among actors. All four are asserted uniformly — with no exemption for kind, seniority, or track record.

### <span id="3a">3a — Boundedness</span>

Every actor brings to each episode of work finite knowledge, finite attention, and finite memory; and nothing guarantees that what one episode held carries over to the next.

### <span id="3b">3b — Fallibility</span>

Every actor errs — in producing, in judging, and in reporting. Rates vary with actor, task, and circumstance; none is zero.

### <span id="3c">3c — No self-certification</span>

An actor's account of its own work is a product of the same actor: it shares the limits and blind spots that shaped the work, and so cannot serve as independent ground for accepting it. Authority to accept can be granted; reliability can never be assumed — for any actor, of any kind.

### <span id="3d">3d — Heterogeneity in motion</span>

Actors differ in:

- speed
- cost
- endurance
- skill-shape
- and persistence of memory

The differences move: capability profiles shift over time, sometimes gradually, sometimes abruptly.

## <span id="commentary">Commentary</span>

This section fixes what the axiom means, what its words cover, and what it does not claim. As in the companion documents, analogies appear with their breaking points marked; the breaks are the content.

### <span id="terms">Terms used in this document</span>

Terms defined in [Axiom 1](1-medium.md#terms) and [Axiom 2](2-intent.md#terms) are used unchanged. New terms:

- **Actor (participant).** Anyone or anything that does work in the collaboration — producing, judging, checking, deciding. A person, a group, or software itself; the theory declines to make the distinction load-bearing, and [T11](#t11) says why.
- **Episode.** One bounded stretch of work by one actor: a sitting, a shift, a session, a run. The word is deliberately neutral about what kind of actor is working.
- **Profile.** An actor's current pattern of capability and cost: what it does quickly or slowly, cheaply or dearly, reliably or badly, and how durable its memory is.

### <span id="3a-commentary">On 3a — Boundedness</span>

The clause has two halves, and both are needed.

Within an episode, capacity is finite. The comparison that gives this force is not between one actor and another but between any actor and the work: a living system's stock of relevant facts — its text, its record of intent, its evidence, its leanings on the world — grows without natural limit, because change never ends ([T4](1-medium.md#t4), [T7](2-intent.md#t7)) and each change leaves residue worth knowing. Whatever an actor's capacity, the ratio of what it holds to what there is to hold trends downward for as long as the system lives. Any arrangement that assumes some actor "has the whole thing in their head" fails on a schedule; only the date varies.

Across episodes, carryover is an achievement, not a given. Memory fades; sittings end; sessions close; the actor who returns tomorrow — if one returns at all — is not guaranteed to hold what yesterday's held. For some actors the boundary is absolute: the episode ends and nothing private survives it. The engineering of carryover — records deliberately written and deliberately reloaded — is [T10](#t10)'s subject.

The boundary of the clause: this is not a deficiency claim, and it names no amounts. A vastly capable actor is still finite, and the clause holds for it exactly as for a modest one. Nothing here dates; greater capacity moves the date of overflow, never the fact of it.

### <span id="3b-commentary">On 3b — Fallibility</span>

Three words in the clause carry most of its weight: _producing_, _judging_, _reporting_. The first is expected. The second means that checking is itself fallible work — review is performed by actors, so a reviewed error is not a contradiction, and no quantity of checking layers reaches certainty ([T1](1-medium.md#t1) said assurance is partial for reasons of the medium; this clause makes it partial for reasons of the participants, independently). The third means that accounts of work — status, progress, "it's done," "I checked" — err like everything else actors make.

Reporting error covers the honest mistake; bedrock adds that when one party acts for another, aims can diverge, so distortion may also be motivated. The theory's machinery does not need to tell the two apart — the same practices that survive sincere error are the starting point against insincere error — but the two are not equally hard: honest error scatters, while motivated distortion concentrates exactly where checking is thinnest. Defenses sized for the first are undersized for the second; [T9](#t9)'s directions carry that burden.

The boundary: fallibility is not equivalence. The clause says no rate is zero; it does not say rates are equal — they differ enormously, and 3d makes those differences a first-class fact. A framework may trust differentially ([T12](#t12)); what it may never do is trust absolutely.

### <span id="3c-commentary">On 3c — No self-certification</span>

Anyone who has proofread their own writing knows the mechanism: you read what you meant, not what you wrote. The misunderstanding that produced the mistake is the same misunderstanding that reviews it.

This is the clause's core, and it is a claim about _correlation_, not about extra fallibility: an actor's self-assessment is not merely one more fallible report (3b already says that) — it is a report whose errors line up with the errors of the work itself.

A second actor errs too, but its errors line up differently. That decorrelation, not any superiority, is what independent checking buys — and only this clause supplies it; no reading of 3b alone does.

The analogy's break: a missed error in prose miscommunicates; in software it executes ([1a](1-medium.md#1a)) — and the author never had full sight of the behavior to begin with ([1d](1-medium.md#1d), whose commentary planted exactly this point).

The clause's second sentence separates two things that collaborations habitually fuse. _Authority_ is a granted right: the sign-off, the merge, the acceptance — some party's yes is designated to conclude the matter, and designating it is necessary and legitimate (the [setting](README.md#setting) requires it). _Reliability_ is a fact about how often a party is right, and no grant can move it. Acceptance concludes the process; it does not make the work fit — the delegator who accepts may later meet dissatisfaction their own yes did nothing to prevent ([2c](2-intent.md#2c)), and questions of behavior stay settled the only way they settle ([T2](1-medium.md#t2)). Frameworks that let authority impersonate reliability inherit the gap as invisible risk.

Uniformity is the clause's edge: no exemption for the most senior human, the most capable machine, or the checking machinery itself — checks are produced artifacts, produced by actors ([T13](2-intent.md#t13) noted this; [T9](#t9) takes it up). The other boundary: self-accounts are not worthless. They are _testimony_ — often the best available map of what was attempted and where the author is unsure — and [T9](#t9) gives them their proper rank: valuable for direction, insufficient for acceptance.

### <span id="3d-commentary">On 3d — Heterogeneity in motion</span>

Profiles do not rank on a single line. Between two actors, each may dwarf the other somewhere: one produces text a thousand times faster; the other carries context across months without being asked. "Better" and "smarter" are not profile words; a profile is a shape, and shapes are compared dimension by dimension, task by task.

The second half of the clause — _in motion_ — is what makes it dangerous to ignore. Practices tune themselves to the profiles of the actors they grow among, silently: a rule of procedure rarely says "this exists because production is slow and judgment is plentiful," yet many rules exist for exactly such reasons. When profiles move — an actor kind gets faster, cheaper, more parallel, or loses and gains memory — the tuned practices fail without announcing it, because the assumption was never written down as an assumption. Whole eras of method are period furniture in this sense. The clause's standing claim is only this: differences exist, and they move. What to do about it is [T11](#t11) and [T12](#t12).

The boundary: 3d does not say profiles are unknowable — they can be measured, and [T12](#t12)'s calibration depends on measuring them. It also does not say assignment is arbitrary — the opposite: profiles are precisely what assignment should follow, held as current measurements rather than as beliefs about kinds.

### <span id="clause-audit">Why these four clauses</span>

The test for each clause is what becomes underivable if it is cut, and whether any clause can be derived from the others.

- **Cut 3a**, and some actor could hold the whole system and carry it across episodes: shared records become optional in principle ([T10](#t10) collapses), structure loses its ground ([T14](#t14)), and judgment stops being scarce ([T12](#t12) weakens to bookkeeping).
- **Cut 3b**, and an inerrant actor could exist: its work needs no checking, its checking closes questions absolutely, and assurance could be made total by assignment — against both [T1](1-medium.md#t1) and everything downstream of it.
- **Cut 3c**, and self-certification suffices: independent verification ([T9](#t9)) becomes a courtesy, and a grant of authority could stand in for reliability.
- **Cut 3d**, and actors are uniform and static: rules could safely name kinds, workflows tuned once would stay tuned ([T11](#t11) collapses), and calibration would be a one-time act rather than upkeep.

None follows from the rest. A bounded actor could be flawless within its bounds — so 3b is not derivable from 3a. Fallibility is a claim about rates, silent on how self-assessment errors align with production errors — so 3c's correlation claim is not derivable from 3b. And bounded, fallible, self-blind actors could still be identical and unchanging — so 3d stands alone. In the other direction, differing and moving profiles imply nothing about limits or error in themselves.

## <span id="consequences">Consequences</span>

Five theorems are homed under this axiom: four descend primarily from it, and [T14](#t14) is a junction theorem drawing equally on Axiom 1, homed here because bounded actors are its subject. (T1–T5 are homed under [Axiom 1](1-medium.md#consequences), T6–T8 and T13 under [Axiom 2](2-intent.md#consequences); numbering is corpus-wide and indexed in the [README](README.md).) As throughout: _theorem_ means an argued consequence, not a formal proof; **engineering directions** state problems a framework must solve, not designs; names from current practice appear in parentheses as labels, never as authorities.

### <span id="t9">T9 — Testimony is not evidence</span>

**Descends from [3c](#3c) + [1d](1-medium.md#1d), with the [setting](README.md#setting) (the economics of acceptance).**

Finished work arrives with an account of itself: what was done, what was checked, why it is right. Call that account **testimony**. By 3c it shares the blind spots of the work; by [1d](1-medium.md#1d) even a maximally careful and sincere producer could not fully know its artifact's behavior anyway. So testimony can inform, direct, and prioritize — it cannot establish. What establishes is **evidence**: records whose force does not route through the producer's self-assessment. Two properties make the difference:

- _Independence_: the record is produced by a process whose errors do not line up with the producer's — another actor's examination, or best, the machine's own execution of checks ([T2](1-medium.md#t2)'s tribunal, which answers to no one's confidence).
- _Binding_: the record is attached to the exact artifact it speaks about ([T3](1-medium.md#d-evidence-binding)), so it cannot drift onto work it never examined.

The setting sharpens this into economics. Where delegation is for leverage — the case that shapes these economics ([setting](README.md#setting)) — it pays only if accepting work costs the delegator less than doing it. Testimony-plus-full-re-derivation offers only bad choices: accept cheap words, or redo the work. **The entire possibility of delegation therefore rests on a third thing existing: evidence that is far cheaper to check than the work was to produce**, and hard to manufacture except by actually doing the work. Such evidence does not occur naturally; it is engineered, and engineering it is among the first obligations of any framework this theory can endorse.

**Engineering directions:**

#### <span id="d-evidence-bundle">The evidence bundle</span>

A framework must say what accompanies produced work by default: the testimony (kept — it is the map), and per class of claim, bound independent evidence — executed checks with results, reproducible demonstrations ([T2](1-medium.md#t2)), and records made _about_ the producer rather than _by_ its self-summary (a mechanical log of what was actually run and touched is nearer to evidence; a narrative of what was accomplished is testimony, however detailed). (Current practice: check-runs attached to exact versions; the request description as testimony beside them.)

#### <span id="d-gaming-resistance">Gaming resistance</span>

Evidence is produced by actors too, and where the producer controls the evidence channel — writes the checks, chooses what runs, summarizes the results — independence decays quietly. Frameworks must decide, by stakes ([T12](#t12)), where the channel must be separated from the work:

- checks the producer cannot alter
- runs the producer cannot curate
- results the producer cannot phrase

Full separation re-imports the cost delegation was meant to lift; the design problem is where partial separation buys the most decorrelation per unit cost — sized for the motivated case, not the honest one ([3b commentary](#3b-commentary)).

#### <span id="d-testimony-rank">Testimony's proper rank</span>

Discarding testimony wastes the best pointer to where evidence should be sought: stated uncertainties, surprising discoveries, decisions closed at the boundary's edge ([T6](2-intent.md#t6)). Frameworks should rank testimony as targeting data — and fix the classes of decision for which testimony alone may never suffice: acceptance at consequential crossings ([T5](1-medium.md#t5)) heads that list.

### <span id="t10">T10 — What is not in the shared record is lost</span>

**Descends from [3a](#3a) + the [setting](README.md#setting), with [T4](1-medium.md#t4) and [T7](2-intent.md#t7).**

The work outlives its episodes. Software needs tending for as long as it runs ([T4](1-medium.md#t4)), and the loop of discovery never runs dry ([T7](2-intent.md#t7)) — while episodes end with no guaranteed carryover (3a), and the setting adds that roles may be re-occupied: the actor who continues the work need not be the actor who did it. So every piece of knowledge the collaboration will need tomorrow — what was decided and why ([T6](2-intent.md#t6)), what was learned ([T7](2-intent.md#t7)), what was checked and how far ([T9](#t9)), what the system leans on ([T4](1-medium.md#t4)) — survives only if it lives outside every actor: durable, shared, inspectable. **The collaboration's memory is not the union of what its actors know. It is exactly the shared record, no more.** What an actor privately knows, the collaboration has merely borrowed — for one episode.

A relay team is only as fast as its baton-work; software's relay has no finish line, and the team changes mid-race. The record is not only memory across time: contemporaneous actors coordinate through it too ([T14](#t14)) — it is the one place all parties can meet. Its subordination to present intent was settled at [T8](2-intent.md#t8): the record witnesses; it does not rule. (What current practice approximates with the repository and its satellites — issues, documents, check histories — is this record, partially and unevenly.)

**Engineering directions:**

#### <span id="d-record-scope">What must be recorded</span>

A framework must enumerate the classes of knowledge whose loss is expensive —

- decisions with their reasons
- rejections ([T7](2-intent.md#d-encounter-capture))
- evidence with its scope ([T2](1-medium.md#d-evidence-scope))
- leanings ([T4](1-medium.md#d-leanings))
- assumptions-in-force ([T6](2-intent.md#d-ask-vs-assume))

— and give each a durable home. The discipline runs both ways: what is _not_ worth recording matters too, because readers are bounded (3a) and a record that swallows everything buries what it keeps. Buried is lost.

#### <span id="d-episode-handoff">Episode boundaries as record events</span>

Private state evaporates where work crosses episodes — end of a sitting, hand-off to another actor, delegation onward. Frameworks should make writing-to-record the closing act of an episode and loading-from-record the opening act of the next, with the boundary treated as absolute for actors whose episodes truly retain nothing. (Current practice's fragments: the commit message, the hand-off note, the onboarding document.)

#### <span id="d-bounded-loading">Loading within bounds</span>

No actor loads the whole record (3a). The mirror problem of keeping the record is _selecting from it_: which slice enters a given episode, chosen how, at what cost, with what confidence that the unloaded remainder held nothing fatal to the episode's task. Retrieval, curation, and entry points sized to bounded readers are not conveniences; they decide whether the record functions as memory at all.

### <span id="t11">T11 — Rules must bind roles and profiles, not kinds of actor</span>

**Descends from [3d](#3d) + the [setting](README.md#setting).**

A framework's rules must be stated over something. Stated over kinds — "a person approves," "the machine writes, the human reads" — they import the profiles of one era as if permanent; 3d says profiles move, so kind-bound rules fail silently when the ground shifts, their assumptions having never been written as assumptions ([3d commentary](#3d-commentary)). Stated over _roles_ (delegator, producer, and whatever verifying and adjudicating roles a framework adds) and _profiles_ (measured capability and cost), rules survive motion: when profiles shift, assignments change; the rules stand. That is also what lets one theory govern every arrangement the setting allows — person delegating to machine, machine to machine, machine to person — without rewriting itself for each.

The test is mechanical: any rule that names a kind must be re-expressible in role-and-profile terms, or it is encoding an era. Two boundaries. Kind is not meaningless — it is often a reasonable first predictor of profile, and may be evidence about a profile not yet measured; what it may not do is substitute for measurement, or appear in the framework's own rules. Kind constraints that are _external obligations held by a party_ — legal sign-off requirements, contractual kind restrictions — are not framework rules in this sense: they enter as expressions of present intent on the delegator side of the corpus ([T8](2-intent.md#t8); [overview](README.md#what-this-is)), ranked and superseded like any other expression, not hard-coded as era assumptions.

**Engineering directions:**

#### <span id="d-role-vocabulary">A role vocabulary with defined powers</span>

Frameworks need the explicit, small set of roles — each with stated powers and duties — such that any actor can occupy any role its profile qualifies it for. Include the composition rules: when one actor may hold several roles at once, and when it may not ([T9](#d-gaming-resistance) forbids producer-as-sole-verifier where stakes are high).

#### <span id="d-profile-currency">Profiles as maintained measurements</span>

What is measured, how it is kept current (3d: it moves), and how staleness is noticed — a profile is a record, inheriting [T8](2-intent.md#t8)'s supersession discipline and feeding [T12](#t12)'s calibration.

#### <span id="d-era-audit">Auditing rules for encoded eras</span>

Practices accrete around the profiles they grew among. Frameworks need the standing audit: for each rule, which profile-facts does it silently assume, and are they still true? A rule whose reason has moved is not a tradition; it is an unexamined cost.

### <span id="t12">T12 — Judgment is the scarce budget</span>

**Descends from [3a](#3a) + [3b](#3b) + [3c](#3c) + the [setting](README.md#setting), with [3d](#3d).**

Everything this theory has required — choosing what to check ([T1](1-medium.md#t1)), adjudicating expressions ([T8](2-intent.md#t8)), deciding at the boundary ([T6](2-intent.md#t6)), accepting at crossings ([T5](1-medium.md#t5)) — consumes qualified judgment, and judgment is finite per actor per episode (3a). The setting makes one pool of it decisive: the delegator's. Where delegation is for leverage, it exists to lift work off the delegator; if judging the work costs what doing it would have cost, that conversion bought nothing. So every dyad — and every level of every chain — lives or dies by the same conversion: how much accepted, fit behavior it obtains per unit of its scarcest judgment. A framework's whole design either raises that rate or squanders it.

Two corrections keep the budget honest. Checking errs (3b), so spending more judgment does not automatically buy more assurance — layers of checking pay when their blind spots differ ([3c](#3c)'s decorrelation, extended), and diminishing returns arrive early when they do not. Profiles differ and move (3d), so the budget's allocation cannot be static: it must follow measured reliability — _calibrated trust_ — with one floor that never moves. Calibration estimates rates that are never exactly known and never zero (3b), so for irreversible classes ([T5](1-medium.md#t5)) checking depth may shrink with earned trust but may not reach zero.

**Engineering directions:**

#### <span id="d-risk-routing">Risk-routing as explicit policy</span>

The framework's core allocator: classify work by stakes —

- consequence class ([T5](1-medium.md#d-consequence-classes))
- possible reach ([T3](1-medium.md#d-change-reach))
- novelty

— and route judgment depth accordingly, including the explicit class that receives _no_ fresh judgment and rides on the executable floor alone ([T13](2-intent.md#t13)). The policy must be inspectable and adjustable, not an emergent habit of whoever was busiest.

#### <span id="d-calibrated-trust">Calibrated trust</span>

Maintain track records per profile and per class of task; let sampling depth follow them; never to zero for irreversible classes. Calibration data are records — currency and staleness rules apply ([T8](2-intent.md#t8), [T11](#d-profile-currency)) — and every new actor poses the cold-start problem: what depth to apply before any track record exists (current practice: probation, graduated autonomy).

#### <span id="d-escalation-design">Escalation design</span>

The path by which questions reach costlier judgment:

- what must escalate ([T6](2-intent.md#t6)'s must-surface classes; conflicts under binding marks in a chain, per [T8](2-intent.md#d-expression-authority) — escalation is the enforcement half of that composition mechanism)
- how questions arrive _prepared_ — batched, evidence-attached, decision-ready — so the dearest judgment pays no retrieval costs (3a)
- and how escalation volume is itself watched, since a flood of escalations means the boundary is drawn wrong ([T6](2-intent.md#d-boundary-drawing)) and a silence of them may mean worse

### <span id="t14">T14 — Structure is how bounded actors survive scale</span>

**Junction theorem. Descends from [3a](#3a) + [1c](1-medium.md#1c), with [T4](1-medium.md#t4) and [T7](2-intent.md#t7). Homed here because bounded actors are its subject.**

Systems grow for as long as they live ([T4](1-medium.md#t4), [T7](2-intent.md#t7)), actors are bounded (3a), so the fraction of a system any actor comprehends trends toward zero — while changes must go on being made, in a medium that spreads consequences without regard to anyone's comprehension ([1c](1-medium.md#1c)). The only exit is to impose on the text a property the medium does not supply: structure — a partition of the system such that bounded comprehension of a _part_ suffices for safe change _within_ it. Its instruments:

- constructed boundaries that confine what a change can touch (supplying the reach-arguments [T3](1-medium.md#d-change-reach) required)
- stated promises at the seams, so a part can be _used_ by knowing its promise rather than its insides — this is how an actor safely changes a system a thousand times larger than its comprehension
- conventions, which make unvisited regions guessable

Structure also enables simultaneity: parts let many producers work at once without trampling one another, coordinating through the seams and the shared record ([T10](#t10)).

Two boundaries. Structure is itself text — [1c](1-medium.md#1c) applies to it, boundaries erode and promises drift, so structure is tended, not installed ([T4](1-medium.md#t4)'s discipline extends to it). And structure costs: every seam is a promise to maintain, and indirection taxes comprehension too — over-partitioned systems fail the bounded reader from the opposite direction.

**Engineering directions:**

#### <span id="d-partition-for-change">Partitioning for bounded change</span>

The objective is change-locality: partition so that the changes that actually come fall within single parts — which requires predicting what changes together, and revising the partition as the loop reveals it ([T7](2-intent.md#t7)). (Current practice: modularity, separation of concerns.) Design questions: what evidence drives partition revision, and who or what carries the standing duty to notice a partition gone stale.

#### <span id="d-seam-promises">Promises at the seams</span>

Stated, checkable promises at every boundary (current practice: interfaces, contracts, schemas) — executable where affordable ([T13](2-intent.md#t13)), versioned and superseded like all records ([T8](2-intent.md#t8)), and written for their real audience: a bounded actor who will never read the insides.

#### <span id="d-convention-subsidy">Convention as comprehension subsidy</span>

Uniformity lowers the cost of every region an actor visits: shared idioms, predictable shapes, one way of doing each common thing. Conventions do two jobs — they pre-close residue decisions ([T6](2-intent.md#d-boundary-drawing)) and they subsidize bounded readers here; a framework should maintain them deliberately under both functions.

#### <span id="d-concurrent-production">Concurrent production</span>

Many producers, one text:

- the partition assigns territory
- seam promises govern the frontier
- the shared record carries coordination ([T10](#t10))
- and where partition fails, changes must be serialized or reconciled (current practice: branches, merges, ownership rules)

Peer producers meeting at a seam is the peer case of composition — the [setting](README.md#setting) completes it; conflicts they cannot settle at the seam escalate to their common delegator ([T12](#d-escalation-design)).

## <span id="elsewhere">Descendants homed elsewhere</span>

Clauses of this axiom are co-parents to theorems homed under the companion axioms:

- [3a — Boundedness](#3a) → [T13 — Intent wants to become executable](2-intent.md#t13)
- [3c — No self-certification](#3c) → [T2 — Questions of behavior are settled by running](1-medium.md#t2)
- [3c — No self-certification](#3c) → [T13 — Intent wants to become executable](2-intent.md#t13)

The corpus-wide derivation graph, including theorem-to-theorem uses, is indexed in the [README](README.md).
