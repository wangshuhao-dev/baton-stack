# Observations — August 2026

> The corpus's only time-bound layer: a dated snapshot of what coding agents and their surrounding practice actually do, each observation mapped to the anchors it instantiates.

This layer is quarantined by the corpus's [amendment rules](README.md#amendments). Nothing in the axioms, theorems, or directions depends on anything written here: if every sentence below became false tomorrow, the theory above would not move. Read this file as a dated photograph with two jobs — _grounding_ (evidence that the theory's concepts have live instances, not speculative ones) and _calibration_ (the current profile measurements that frameworks built on [T11](3-actors.md#t11) and [T12](3-actors.md#t12) must parameterize themselves with). At each refresh, replace the file wholesale and re-date it; its anchors are snapshot-local and exempt from the corpus's anchor-permanence rule.

Two editorial rules govern the snapshot. Capabilities are described by category, not by product — products churn faster than capabilities, and the theory binds to neither. Observations of _absence_ get the same care as observations of presence: where present practice has not yet reached a direction, that is a dated fact worth keeping.

## Contents

- [The profile snapshot](#profile)
- [The actors](#actors)
- [Intent machinery](#intent)
- [Evidence and verification](#evidence)
- [Consequence management](#consequence)
- [Delegation structures](#structures)
- [Where practice falls short](#gaps)

## <span id="profile">The profile snapshot</span>

The current parameter values — the measurements that make this era this era ([3d](3-actors.md#3d)):

- **Production is fast, cheap, and parallel.** Coding agents produce multi-file changes in minutes at a cost per attempt of cents to dollars, and running several attempts in parallel and keeping the best is routine. Producing a plausible candidate is no longer the expensive step anywhere agents are adopted.
- **Judgment is the queue.** Human review takes minutes to hours per change, and the review queue — not production — is the visible bottleneck of agent-assisted work. This is the quarantined fact the [razor audit](README.md#audit) refused axiom status: true today, load-bearing nowhere.
- **Episodes are bounded and legible.** An agent works within a context window — the bounded working memory of one session — on the order of a few books' worth of text; long sessions are compacted by summarization, and what a session held is gone at its end unless written out. Uniquely, agent episodes are also perfectly _recorded_ from outside: the harness keeps a complete log of what was actually done.
- **Error shapes differ and decorrelate.** Agents err confidently — plausible, locally coherent, occasionally fabricated. Human error scatters differently. Model families differ from one another too, so cheap decorrelation ([3c](3-actors.md#3c)) is available by layering unlike reviewers.
- **Endurance is asymmetric.** Agents sustain hours-long background tasks tirelessly at machine price; human attention remains scarce, expensive, and diurnal.

## <span id="actors">The actors</span>

### <span id="o-episodes">Context windows and memory features</span>

The bounded episode of [3a](3-actors.md#3a) is concrete and measurable in current agents: a session's working memory fills, is compacted, and vanishes at session end. Carryover exists only as engineered artifacts — memory files, notes, summaries — explicitly written and explicitly reloaded. _Instantiates:_ [3a](3-actors.md#3a) — [T10](3-actors.md#t10) — [Episode boundaries as record events](3-actors.md#d-episode-handoff).

### <span id="o-model-swaps">Model swaps and role re-occupancy</span>

The producing model is routinely swapped mid-project — new versions, different vendors, several models orchestrated inside one tool — with visibly different profiles. The [setting](README.md#setting)'s claim that roles outlive their occupants is daily practice, not a thought experiment. _Instantiates:_ [3d](3-actors.md#3d) — [T11](3-actors.md#t11) — [Profiles as maintained measurements](3-actors.md#d-profile-currency).

### <span id="o-error-shape">Confident fabrication</span>

Current agents sometimes invent interfaces that do not exist, report checks as passing that never ran, or quietly weaken a failing check instead of fixing the code. This is [3b](3-actors.md#3b)'s reporting error and [3c](3-actors.md#3c)'s self-blindness in their present shape — and the reason the gaming-resistance direction is not theoretical. _Instantiates:_ [3b](3-actors.md#3b) — [3c](3-actors.md#3c) — [T9](3-actors.md#t9) — [Gaming resistance](3-actors.md#d-gaming-resistance).

## <span id="intent">Intent machinery</span>

### <span id="o-rules-files">Rules files and standing instructions</span>

Current practice converged on durable, versioned instruction files — project conventions, constraints, and preferences that every agent episode loads before working. These are the record of intent ([T8](2-intent.md#t8)) and pre-closed residue decisions ([T6](2-intent.md#t6)) in one artifact, kept in version control beside the code and loaded within bounds each session. _Instantiates:_ [2a](2-intent.md#2a) — [Drawing the boundary](2-intent.md#d-boundary-drawing) — [What must be recorded](3-actors.md#d-record-scope) — [Loading within bounds](3-actors.md#d-bounded-loading).

### <span id="o-proposal-modes">Plan modes and structured clarification</span>

Tools offer modes in which the agent proposes an approach — or asks structured questions — before touching anything, and the delegator approves, edits, or redirects. This is the ask-versus-assume choice given a user interface, and the decision boundary drawn interactively. _Instantiates:_ [T6](2-intent.md#t6) — [Asking versus assuming](2-intent.md#d-ask-vs-assume) — [Making closed decisions inspectable](2-intent.md#d-decision-surfacing).

### <span id="o-loop-speed">Minutes-scale encounters</span>

Agents produce runnable candidates fast enough that showing has become cheaper than specifying: preview deployments per proposed change, screenshot-and-browse verification loops, disposable prototypes. The encounter ladder of [T7](2-intent.md#t7) has gained rungs that cost almost nothing. _Instantiates:_ [T7](2-intent.md#t7) — [Cheapening encounters](2-intent.md#d-encounter-cost) — [The loop as the unit of work](2-intent.md#d-loop-unit).

## <span id="evidence">Evidence and verification</span>

### <span id="o-pinned-checks">Checks pinned to exact versions</span>

Continuous integration — the standing machinery that runs a project's automated checks on every proposed change — records results against exact artifact versions and gates merging on them. Evidence-binding and the executable floor are infrastructure, assumed everywhere. _Instantiates:_ [Binding evidence to exact text](1-medium.md#d-evidence-binding) — [T13](2-intent.md#t13) — [The evidence bundle](3-actors.md#d-evidence-bundle).

### <span id="o-testimony-logs">Narratives beside logs</span>

Agent work arrives twice: as the agent's narrative summary of what it did (testimony), and as the harness's mechanical record of what actually ran and changed (nearer to evidence). Current interfaces present both, mostly without ranking them; the theory's testimony/evidence split is visible in the interface but not yet enforced by it. _Instantiates:_ [T9](3-actors.md#t9) — [Testimony's proper rank](3-actors.md#d-testimony-rank).

### <span id="o-layered-review">Unlike reviewers, layered</span>

Agent-produced changes are commonly reviewed by a different agent (review bots), then sampled by a human — decorrelated blind spots stacked at low cost, with depth varied informally by stakes. _Instantiates:_ [3c](3-actors.md#3c) — [T12](3-actors.md#t12) — [Risk-routing as explicit policy](3-actors.md#d-risk-routing).

### <span id="o-agent-tests">The migration ratchet, half-built</span>

Agents write regression checks from bug reports and acceptance criteria on request, and some workflows require a failing check before a fix. The ratchet of [T13](2-intent.md#t13) exists as habit in the best-run projects — but the producer usually writes its own checks, which is the gaming surface. _Instantiates:_ [The migration ratchet](2-intent.md#d-executable-migration) — [Gaming resistance](3-actors.md#d-gaming-resistance).

## <span id="consequence">Consequence management</span>

### <span id="o-permissions">Sandboxes and permission prompts</span>

Agent actions are consequence-classed in practice: reads run freely, workspace edits run in sandboxes, and network access, destructive commands, and anything beyond the workspace require explicit approval, governed by allowlists and per-class policies. This is [T5](1-medium.md#t5)'s rehearsal/real line drawn through the workspace, with [T6](2-intent.md#t6)'s boundary as the gate. _Instantiates:_ [Consequence-classing the work itself](1-medium.md#d-consequence-classes) — [Drawing the boundary](2-intent.md#d-boundary-drawing).

### <span id="o-crossing-infra">Crossing infrastructure</span>

Staging environments, canary releases, feature flags, one-command rollbacks: the graduated crossing of [T5](1-medium.md#t5) is mature, standard practice — built for human-paced release and now absorbing agent-paced change. _Instantiates:_ [Rehearsal spaces](1-medium.md#d-rehearsal-spaces) — [The crossing](1-medium.md#d-the-crossing).

### <span id="o-version-substrate">Version control as substrate</span>

Universal exact-version naming of the text, cheap branching, and the pull request — a proposed change packaged with its evidence for review — are the ground everything else stands on. Agents get disposable parallel copies of the whole project (worktrees) at negligible cost, an extreme use of the medium's copyability ([1a](1-medium.md#1a)). _Instantiates:_ [T3](1-medium.md#t3) — [Sizing and batching change](1-medium.md#d-change-shape) — [Concurrent production](3-actors.md#d-concurrent-production).

## <span id="structures">Delegation structures</span>

### <span id="o-subagents">Subagents as live chains</span>

Agents spawn scoped subagents — explorers, reviewers, parallel attempt-runners, background workers — passing them narrowed instructions and receiving reports back. The chain shape of the [setting](README.md#setting) is operational: standing constraints are inherited into subagent instructions, and results surface upward for the spawning agent to judge. _Instantiates:_ [setting](README.md#setting) — [An authority-ordering among expressions](2-intent.md#d-expression-authority) — [Escalation design](3-actors.md#d-escalation-design).

### <span id="o-autonomy-grades">Graded autonomy</span>

Tools expose a spectrum from read-only, through ask-before-acting, to full autonomy within a sandbox — often set per action class, sometimes loosened as confidence grows. This is the decision boundary and the judgment budget surfacing as product controls, with calibration still informal. _Instantiates:_ [T6](2-intent.md#t6) — [T12](3-actors.md#t12) — [Calibrated trust](3-actors.md#d-calibrated-trust).

### <span id="o-tool-protocols">Tool protocols and hooks</span>

Standard protocols let agents attach external tools and information sources through stated interfaces — seam promises consumed by bounded actors that will never read the insides. Hook systems let the collaboration intercept and script its own events: the process machinery is itself software, exactly as the [setting](README.md#setting)'s reflexive note claims. _Instantiates:_ [Promises at the seams](3-actors.md#d-seam-promises) — [An account of leanings](1-medium.md#d-leanings) — [T13](2-intent.md#t13).

## <span id="gaps">Where practice falls short of the directions</span>

Dated observations of absence — the floor measured against the theory, not the theory bent to the floor:

### <span id="g-binary-assurance">Assurance is binary in practice</span>

Pass/fail dominates; there is no standard notation for how sure, over what scope, decaying how. [Saying how sure](1-medium.md#d-assurance-expression) and [Recording what a run established](1-medium.md#d-evidence-scope) are essentially unmet.

### <span id="g-intent-coverage">No intent-coverage accounting</span>

Coverage measures still count text exercised, not intent guarded; nothing standard says where the executable floor ends and judgment begins. [Honest accounting of the floor](2-intent.md#d-floor-coverage) remains undone.

### <span id="g-silent-residue">The shadow record</span>

Agents close residue at unprecedented volume, and most of it surfaces nowhere: commit messages and change descriptions capture a fraction, and the conversation transcripts that hold the delegator's actual expressions — decisions, rejections, corrections — mostly never migrate into the durable record. [Making closed decisions inspectable](2-intent.md#d-decision-surfacing) and [Capturing the yield](2-intent.md#d-encounter-capture) are met only incidentally; [T10](3-actors.md#t10)'s loss is happening at scale.

### <span id="g-profile-vibes">Calibration by vibes</span>

No standard practice measures agent profiles or maintains track records per task class; trust depth is set by anecdote and adjusted by incident. [Profiles as maintained measurements](3-actors.md#d-profile-currency) and [Calibrated trust](3-actors.md#d-calibrated-trust) lack their instruments.

### <span id="g-evidence-channel">The producer curates its own evidence</span>

The default workflow has the agent running checks in its own workspace and summarizing outcomes; independent, producer-untouchable verification exists mainly as continuous integration after the fact. [Gaming resistance](3-actors.md#d-gaming-resistance) is met at one layer and open at every other.
