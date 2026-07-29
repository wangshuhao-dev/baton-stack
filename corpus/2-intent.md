# Axiom 2 — Intent

> **What software should do exists only as finite expressions of intent; every expression leaves most behavior undecided, and no expression is final.**

This is one of three foundation documents. Each characterizes one element of software work: the medium ([Axiom 1 — The Medium](1-medium.md)), the wanting (this document), and the participants ([Axiom 3 — Actors](3-actors.md)). The overview and full index live in the [README](README.md).

## Contents

- [Statement](#statement)
- [Commentary](#commentary)
- [Consequences](#consequences)
- [Descendants homed elsewhere](#elsewhere)

## <span id="statement">Statement</span>

The axiom is stated in three clauses. Together they characterize the wanting: the form in which it exists inside software work, the reach of any statement of it, and its life in time. These are facts about wanting software as such — they hold whoever, or whatever, wants, and whoever, or whatever, builds.

### <span id="2a">2a — Expression-boundedness</span>

Intent — what software should do and not do — enters software work only as expressions: statements, documents, examples, demonstrations pointed at, reactions to what exists. This holds for every party, including intent's own holder: whatever wanting may be inwardly, the work can meet it only in expressed, finite form.

### <span id="2b">2b — Underdetermination</span>

Every expression of intent, and every finite collection of them, is compatible with many different behaviors — among them many that intent's holder would reject on sight. Expressions delimit behavior; they do not determine it. What they leave open is the residue.

### <span id="2c">2c — Motion and present authority</span>

Intent moves. Expressions made at different times need not agree, and later expressions presumptively supersede earlier ones — the presumption strong, but examinable. What behavior must fit, at any moment, is intent as it stands at that moment — not any record, however careful, of what it once was.

## <span id="commentary">Commentary</span>

This section fixes what the axiom means, what its words cover, and what it does not claim. As in the companion documents, analogies appear with their breaking points marked; the breaks are the content.

### <span id="terms">Terms used in this document</span>

Terms defined in [Axiom 1](1-medium.md#terms) — text, behavior, running, checking and assurance, bedrock — are used unchanged. New terms:

- **Intent.** The wanting itself — what some party would accept, prefer, or reject in software's behavior — as distinct from any statement of it. By clause 2a, the work never meets intent directly; the word names what expressions are expressions _of_.
- **Expression.** Any act or artifact offered as evidence of intent: a request, a document, an example, a pointed-at precedent ("like that one, but…"), a sketch, an executable check, a reaction to candidate behavior — approval, rejection, "yes, but." Rejections are expressions too, and unusually cheap, precise ones.
- **Residue.** The behavior-determining questions that a body of expressions leaves open.
- **Delegator / producer.** The two roles present in any piece of software work: the _delegator_ holds authority over whether the result fits; the _producer_ does the work of production. These are roles, not kinds of being — either may be a person, a group, or software itself, and one party may hold both roles in different relations at once: a producer that delegates part of the work onward is the delegator of that further relation. The full setting is given in the [overview](README.md#setting).
- **Fit.** Acceptability of behavior to the delegator's present intent. Fit is judged — and the judgment is itself an expression, with everything that implies.

### <span id="2a-commentary">On 2a — Expression-boundedness</span>

This clause does no psychology. It does not say what wanting is made of, where it lives, or how it feels — questions belonging to other disciplines, taken here as given and outside this theory's domain. It locates something narrower: the only form in which intent ever _participates_ in software work. No party — the holder included — brings wanting itself to the table. What arrives is expressions: finite, made, inspectable things. Communication between parties never guarantees identical understanding (bedrock), so what would otherwise be assumed shared must be carried by those expressions, or remain residue.

Law found the same footing long ago: courts do not weigh souls; they weigh testimony, documents, and conduct. The analogy breaks in an instructive place. Law must still reason _about_ inner states — it asks what a person must have intended — because its verdicts attach to persons. This theory never has to. Everything built later — boundaries of decision, loops of discovery, records and their upkeep — operates on expressions alone. Even the final "yes, this is what I wanted" is one more expression, carrying an expression's limits: fallible (a fact about participants — [Axiom 3](3-actors.md)) and not final ([2c](#2c)).

Note the breadth the term is given: examples, counter-examples, pointed-at precedents, and _reactions_ all count. Reactions matter most later ([T7](#t7)): confronted with candidate behavior, a holder's "no — not that" is as much an expression as any document, and often a sharper one.

One economic fact belongs at the root: expressions cost something to make — attention, time, care. Any advice that reduces to "the delegator should simply say everything" fails twice: once against this clause's finitude, and once against the price of saying ([T6](#t6) prices the asking; [T7](#t7) prices the eliciting).

### <span id="2b-commentary">On 2b — Underdetermination</span>

"A steak, medium-rare." The kitchen decides the rest — the salt, the plate, the timing, whether the vegetables touch the meat. Most of those decisions never surface; a few would be rejected if they did. Every expression of intent works this way: it fixes what its maker was attending to and leaves the rest to whoever acts on it. The analogy's break measures the danger. Diner and kitchen share centuries of convention about what dinner is, so the residue rarely goes badly wrong. A software producer may share far less context with the delegator — and the machine that finally executes shares none at all ([1a — the literal reader](1-medium.md#1a)). In software the residue is larger, stranger, and less padded by shared habit.

The obvious escape is generality: can't one rule cover infinitely many cases? "For every number entered, show its double" — complete, over an endless domain. It is complete only along the dimensions its maker was considering. What if the number arrives malformed? While another request is mid-flight? On a screen too small for the answer? A general rule quietly answers every question of the kinds its maker thought of, and no question of any other kind. This is why the clause is not a counting trick about finite texts and infinite cases: the residue of real systems lives mostly in _dimensions nobody was weighing_ when the expression was made, not in cases a rule failed to reach.

It helps to split the residue into two provinces. One is the _unsaid-but-decided_: questions the holder could answer at once if asked — preferences already formed, merely never transcribed. The other is the _never-considered_: questions the holder has no stored answer to. The first province shrinks under interrogation. The second resists interrogation twice over: no list of questions reaches the dimensions nobody thought to weigh, and where a question does land, asking retrieves no decision — it forces a fresh one into existence, made in the abstract, before any behavior has been met. What shrinks this province is encounter — [T7](#t7)'s subject — and for software of any consequence it is by far the larger province.

Keep this clause distinct from [1d — Opacity](1-medium.md#1d); the two gaps differ in kind. Software's text _determines_ behavior completely — given the situation, exactly one thing happens — it merely fails to _disclose_ it to readers. Expressions of intent are weaker in a further way: they do not even determine. They delimit a region of acceptability and stop. Production is the forced march between the two: it begins from expressions that determine nothing completely and must end in text that determines everything, because the medium grants no third option. That march is made of decisions — which is [T6](#t6).

The boundary of the clause: it denies completion, not usefulness. Expressions do real work — each good one shrinks the residue, rules out families of wrong behavior, and aims later judgment. What no quantity of them ever does is finish.

### <span id="2c-commentary">On 2c — Motion and present authority</span>

Three separate facts stand behind the motion, and none requires a theory of why minds change. The world moves (bedrock), and wanting tracks circumstance: what fit last year's rules, prices, and platforms does not fit this year's. Encounter elicits: confronted with actual behavior, holders produce expressions they could not have produced before ([T7](#t7)). And expressions accumulate: any long-lived collaboration holds early and late expressions side by side, and they disagree — about what is wanted and about what matters.

The clause's supersession rule should be read the way a lawyer reads one. A later will revokes an earlier; the latest is taken as the standing word. The presumption here is the same — and like the legal one, it is a _presumption_: strong, but examinable.

Expressions differ in deliberateness and scope; a considered document and a hasty aside may conflict, and recency alone need not settle which better witnesses present intent. How conflicts are adjudicated is engineering, treated at [T8](#t8); the axiom fixes only what adjudication is _about_ — present intent, of which every record is at best evidence.

The will analogy also breaks in the most useful place: a will is read because its maker can no longer be asked. Software's intent-holder usually can be. The record is a stand-in between askings, never a replacement for asking.

The clause also draws a line that commitments cannot cross. Parties do freeze _obligations_: a specification is agreed, a change is priced, a deadline is set (current practice: _spec freeze_, _change requests_). Freezing obligation does not freeze wanting. A delegator can owe acceptance of what they no longer want, and the divergence shows up in the world as compliance without satisfaction. The theory keeps the two ledgers separate: fit-to-record can be contracted; fit-to-intent cannot — and treating the first as settling the second is how delivered-and-resented systems happen.

Finally, this clause pulls against the later need for durable shared records ([T10 — What is not in the shared record is lost](3-actors.md#t10)), and the tension is productive rather than embarrassing. Records must be kept — and kept _cheap to supersede_. A record too costly or too ceremonious to override stops witnessing present intent and starts impersonating it. The design consequences are [T8](#t8)'s.

### <span id="clause-audit">Why these three clauses</span>

The test for each clause is what becomes underivable if it is cut, and whether any clause can be derived from the others.

- **Cut 2a**, and the work could meet wanting directly: fit could be judged against intent itself, and every mechanism this theory builds on expressions — elicitation, records, their upkeep — loses its reason in principle.
- **Cut 2b**, and some finite body of expressions could determine behavior completely: one-shot specification becomes available, production stops being decision-making ([T6](#t6) collapses), the loop becomes mere inefficiency ([T7](#t7)), and a finished suite of checks could equal intent ([T13](#t13)'s floor becomes the whole building).
- **Cut 2c**, and a record once right is right forever: no adjudication between old and new expressions is needed, acceptance is final, and the record of intent needs writing but never tending ([T8](#t8) reduces to filing).

None follows from the rest. Expressions-only (2a) does not entail incompleteness — the generality objection above had to be answered on its own ground, not by counting. Incompleteness (2b) does not entail motion: a wanting could be underdetermined yet fixed — the stubborn holder is logically possible, which is exactly why motion is asserted rather than derived. And motion (2c) presumes nothing about completeness: even a holder whose every expression were somehow complete would still change, and the precedence rule would still be needed.

## <span id="consequences">Consequences</span>

Four theorems are homed under this axiom: three descend primarily from it, and one — [T13](#t13) — is a junction theorem, drawing equally on the companion axioms but homed here because intent is its subject. (T1–T5 are homed under [Axiom 1](1-medium.md#consequences), T9–T12 and T14 under [Axiom 3](3-actors.md#consequences); numbering is corpus-wide and indexed in the [README](README.md).) As throughout: _theorem_ means an argued consequence, not a formal proof; **engineering directions** state problems a framework must solve, not designs; names from current practice appear in parentheses as labels, never as authorities.

### <span id="t6">T6 — Every act of production decides unstated things</span>

**Descends from [2b](#2b) + the [setting](README.md#setting), with [1a](1-medium.md#1a).**

Expressions delimit; they do not determine (2b). But finished software determines everything: whatever situation arrives, the machine follows the text and exactly one behavior happens ([1a](1-medium.md#1a)) — the medium has no way to abstain. So every question in the residue is closed by the time software runs, and closed by production itself. **Producing software is not transcription with occasional decisions mixed in; it is decision-making as a continuous condition** — residue questions closed by the hundred, mostly without ceremony, many without notice.

In a delegation this has a structural consequence. Authority over fit belongs to the delegator (setting), yet the residue's closure defaults to the producer — silently. Delegation therefore transfers, along with the work, a mass of unexamined deciding. Neither party chose that transfer; the medium imposed it. What _can_ be chosen is the boundary: which classes of residue decision the producer may close alone, which it must surface before acting, which it must never close. The boundary exists in every delegation — undrawn, it still operates, as pure default. A framework's job is to make it an object: drawn, visible, adjustable.

And it is an economic object, not only a rights object. Surfacing a decision spends the delegator's attention — the scarce input delegation exists to conserve (the [setting](README.md#setting)'s leverage motive; the economics are developed at [T12 — Judgment is the scarce budget](3-actors.md#t12)). A boundary that surfaces everything reproduces the burden delegation was meant to lift; one that surfaces nothing transfers authority wholesale. Everything interesting lies between — and moves, with stakes, with track record, and with how costly a wrong silent closure would be to undo ([T5 — Some runs are rehearsals; some are real](1-medium.md#t5)).

**Engineering directions:**

#### <span id="d-boundary-drawing">Drawing the boundary</span>

A framework must give a collaboration the vocabulary and mechanism to state its boundary explicitly — which decision classes the producer closes alone, which it surfaces first, which are closed to it entirely — and to adjust the statement as stakes and track record change. The oldest instrument here is the _convention_ (current practice: style guides, house standards): a batch of residue decisions closed in advance, once, for everyone — the cheapest boundary-drawing there is. Where instructions reach the producer from beyond the dyad, precedence questions arise; those are treated under [T8's authority-ordering](#d-expression-authority).

#### <span id="d-decision-surfacing">Making closed decisions inspectable</span>

Most closures will be silent; silence must not mean invisible. Frameworks need the record of what was decided in the residue — what was assumed, what was chosen, at which moment — kept cheaply enough that keeping it does not dominate the work, and structured enough that review can sample it afterward (current practice: decision records, the explanatory commit message, the "why" comment). How far such self-reports can be trusted is [T9](3-actors.md#t9)'s question.

#### <span id="d-ask-vs-assume">Asking versus assuming</span>

At the boundary's edge the producer has three moves:

- _ask now_ — spends delegator attention, and may force a fresh decision the holder is not ready to make, since the never-considered province resists interrogation ([2b commentary](#2b-commentary))
- _assume and flag_ — cheap now, bills later if wrong
- _build and show_ — turns the question into an encounter ([T7](#t7))

A framework must say when each move is right, and how assumptions-in-force stay visible instead of fossilizing into fact.

### <span id="t7">T7 — Intent is discovered through the loop</span>

**Descends from [2a](#2a) + [2b](#2b) + [2c](#2c), with [1d](1-medium.md#1d).**

Call it an _encounter_ when intent's holder confronts candidate behavior — a sketch walked through, a prototype poked at, a demonstration watched, the real system used. The residue's larger province, the never-considered, does not yield to interrogation: there is no stored answer to retrieve (2b), and expressions cannot be summoned for questions never yet faced (2a). What converts never-considered into expressed is encounter. Confronted with behavior, holders produce expressions they could not have produced in advance — most cheaply, the precise and load-bearing _"no — not that."_ And since behavior can only be known by running ([1d](1-medium.md#1d)), encounters must be _had_; they cannot be deduced.

So the loop — build something showable, show it, harvest the reactions, go again — is not a modern taste or a concession to indiscipline. **It is the only mechanism that reaches the residue's larger province.** And because intent also moves on its own (2c), the loop never runs dry: even a hypothetically perfected record of wanting would date.

This does not abolish forethought; it bounds and re-prices it. Deliberation is itself a weak encounter — imagining a case is confronting it, at low cost and low fidelity. From there a ladder rises — each rung dearer and truer than the last:

1. the considered case
2. the sketch
3. the mockup
4. the prototype in a rehearsal space ([T5](1-medium.md#t5))
5. the staged release
6. the system in earnest

Planning is not the loop's rival; it is the loop's cheapest rung. The theorem claims only that no rung, however carefully climbed, substitutes for the ones above it (current practice remembers the costs of denying this under the name _waterfall_).

**Engineering directions:**

#### <span id="d-loop-unit">The loop as the unit of work</span>

Frameworks should shape work as encounter-cycles rather than one-way hand-offs: each cycle scoped by which residue it means to expose, and obliged to produce fresh expression, not only artifact (current practice: iterations, demos, prototypes). Design questions: what sets cycle length; what a cycle must yield to count as complete; and what "done" can even mean under 2c — an answer a framework must give explicitly rather than inherit.

#### <span id="d-encounter-cost">Cheapening encounters</span>

Discovery rate is bounded by the cost of the next encounter. Frameworks must drive that cost down — fast paths from idea to showable candidate, rehearsal spaces ready to hand ([T5](1-medium.md#t5)) — and aim encounters where they pay: at residue whose wrong silent closure would cost most ([T1's weighting](1-medium.md#t1), [T12's budget](3-actors.md#t12)). The failure mode to design against: encounters so dear they are rationed into vanishing, leaving the residue to close silently at full scale.

#### <span id="d-encounter-capture">Capturing the yield</span>

An encounter's product is expression — the "not that," the "yes, but," the "oh, and also." Reaction that stays conversational evaporates, and the encounter's cost buys nothing durable. Frameworks must make turning reactions into keepable expressions a step _of the loop itself_, not optional hygiene afterward — with rejections captured most carefully, since they are the sharpest delimiters (2b) and the easiest to lose. Durability and shared reach of what is captured are [T10](3-actors.md#t10)'s subject.

### <span id="t8">T8 — The record of intent is maintained, never finished</span>

**Descends from [2a](#2a) + [2c](#2c).**

Because intent enters the work only as expressions (2a), a collaboration of any age holds a _corpus_ of them:

- requests
- documents
- examples
- executable checks
- captured reactions

Because intent moves (2c), the corpus disagrees with itself: early expressions sit beside late ones, considered beside hasty, general beside specific — and behavior cannot fit them all. Three obligations follow.

The corpus must be **tended**. Superseded expressions must be retired or marked, or they go on testifying: stale documents and stale checks do not fall silent on their own — they mislead with perfect confidence. Tending the record of intent is the same kind of standing work as tending the software ([T4](1-medium.md#t4) is the medium-side twin), and neglecting it has the same character of consequence.

Conflicts must be **adjudicated**. When the check asserts one thing, the document another, and the latest conversation a third, something must say which governs — before the producer closes residue against the wrong witness ([T6](#t6)). The axiom supplies the principle: every record is evidence of present intent; later presumptively outweighs earlier (2c); and the presumption is examinable — deliberateness, specificity, and source all bear on which expression better witnesses the intent that now stands. The final appeal, available whenever the holder can be asked, is fresh expression.

And the corpus must stay **subordinate**. However well tended, it is testimony about wanting, not wanting itself. A record too authoritative — too costly or too ceremonious to override — begins impersonating the thing it witnesses. The corpus must be strong enough to work from and weak enough to overrule.

**Engineering directions:**

#### <span id="d-expression-authority">An authority-ordering among expressions</span>

A framework must supply the precedence rules:

- how recency, deliberateness, specificity, and source rank against one another when expressions conflict
- when conflict triggers asking instead of ranking
- and how an adjudication is itself recorded — it is a decision, so [T6's surfacing](#d-decision-surfacing) applies

Source matters because expressions reach a dyad from beyond it. In a delegation chain, a producer may hold the near delegator's fresh instruction _and_ a standing constraint from further up the chain, in conflict.

The composition rule the dyadic frame requires: expressions from beyond the dyad bind as part of the delegator side of _this_ dyad, carrying explicit precedence marks —

- some marked _binding_ (the far constraint prevails, and the conflict is surfaced upward rather than resolved locally)
- some _advisory_ (the near instruction prevails)

Which marks exist, who may set them, and what surfacing upward costs are framework design; the compositional setting is completed in the [overview](README.md#setting) and [Axiom 3](3-actors.md). (Current practice holds fragments of such an ordering — the ticket outranks the wiki, the contract outranks both — rarely stated, always operating.)

#### <span id="d-record-reconciliation">Reconciliation as standing work</span>

Retiring and marking superseded expressions needs a routine trigger, not an annual resolve: encounters ([T7](#t7)) and adjudications should each end with corpus edits. And disagreement must be _detectable_ — conflicts between prose, checks, and code surface today mostly by accident; what machinery would surface them on purpose? (The corpus's durability and shared reach are [T10](3-actors.md#t10)'s subject.)

#### <span id="d-cheap-supersession">Cheap, visible supersession</span>

Overriding the record must be low-ceremony, or present intent stops flowing through the record and routes around it — the corpus decaying into a false front. But cheap must not mean silent: a supersession leaves a trace — what stood, what stands, since when — because other participants have been relying on what stood ([Axiom 3](3-actors.md) grounds this), and because the trace is what makes the presumption of recency workable at all. The design question: where does ceremony belong — at writing, at overriding, or at relying?

### <span id="t13">T13 — Intent wants to become executable</span>

**Junction theorem: descends from [2b](#2b) + [2c](#2c) + [1d](1-medium.md#1d) + [3a](3-actors.md#3a) + [3c](3-actors.md#3c), with bedrock (machines run text exactly, fast, at negligible cost). Homed here because intent is its subject.**

Expressions of intent differ in a property that turns out to organize everything: whether conformance to them can be checked by a machine. "Feels trustworthy" must be checked by judgment. "Given this exact situation, this exact behavior" can be phrased so that a machine arranges the situation, runs the software, and compares the outcome against the expression — an _executable expression_ (current practice: an automated test — a small program whose only job is to stage a situation, run the software in it, and compare what happens with what was wanted).

Executable expressions have three properties no other kind of expression matches:

- They are checked at machine price — tirelessly, identically, as often as wanted (bedrock) — which matters because assurance must be re-earned after every change ([T3](1-medium.md#t3)): a judgment-checked expression bills its full cost at every re-check, while an executable one, once written, re-verifies for near-nothing, forever.
- Their verdict does not depend on who asks ([T2](1-medium.md#t2); co-parent [3c](3-actors.md#3c)).
- And they keep testifying without anyone's attention or memory ([3a](3-actors.md#3a): judgment and recall are finite per episode).

Hence the gradient this theorem's name states: over a system's life there is standing pressure — economic, not moral — for intent to migrate into executable form wherever migration is affordable. The yield of encounters ([T7](#t7)), the closures surfaced at the boundary ([T6](#t6)), the lessons of escaped failures ([T1](1-medium.md#t1)) — each is worth more re-expressed executably, because it then guards without being attended to.

Three boundaries keep the theorem honest:

1. Not all intent can migrate: taste, tone, and judgment-of-the-whole resist mechanization, and pretending otherwise replaces intent with whatever was easy to check. The executable corpus is a _floor_ — it catches what it catches with no one watching, and everything above it still rests on judgment.
2. Executable expressions are still expressions: a finite suite delimits and does not determine (2b applies in full), so passing every check never means fitting — the floor is not the building.
3. They are still _records_: they age (2c), they conflict, and a failing check sometimes means the check is superseded rather than the software broken — [T8](#t8)'s adjudication, arriving with unusual sharpness because this witness is a machine and cannot soften its testimony. A check is also produced text, made by some fallible participant; whether it deserves belief is [T9](3-actors.md#t9)'s question.

**Engineering directions:**

#### <span id="d-executable-migration">The migration ratchet</span>

Frameworks should build the one-way mechanism: whenever discovery or failure produces fresh expression, the default next act is executable re-expression where affordable — every escaped defect becomes a check, every sharpened rejection becomes a check (current practice: regression tests written from failures; acceptance criteria turned into tests). Design questions: where the affordability line sits; who or what moves expressions across it; and how a migration is checked against the expression it translates — a mistranslated check guards the wrong thing with machine confidence.

#### <span id="d-floor-coverage">Honest accounting of the floor</span>

Since the floor is not the building, frameworks must keep visible where the checked region ends: which expressed intent is executably guarded, which rests on judgment, and which residue neither reaches. (Current practice's _coverage_ measures gesture at this but measure text exercised, not intent guarded; the accounting asked for here does not yet exist as a standard practice.) This is [T1's "saying how sure"](1-medium.md#d-assurance-expression) specialized to the intent side.

#### <span id="d-check-maintenance">Checks as tended intent</span>

The executable corpus is part of the record of intent and inherits [T8](#t8) entire: retirement with the same care as enactment, supersession cheap and visible, staleness treated as false testimony. The sharpness is special here: a stale document misleads whoever happens to read it, but a stale check _acts_ — it blocks, gates, and alarms with authority it no longer carries. Current practice knows the endpoint: the failing test everyone has learned to ignore.

## <span id="elsewhere">Descendants homed elsewhere</span>

No clause of this axiom currently serves as co-parent to a theorem homed under a companion axiom: the wanting's consequences concentrate here. The corpus-wide derivation graph, including theorem-to-theorem uses, is indexed in the [README](README.md).
