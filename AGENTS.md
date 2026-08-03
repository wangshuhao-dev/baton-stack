<!--REPOSITORY LAYOUT START-->

# Nonstandard layout — corpus and shared record first, not source code

This repository is full-stack scaffolding for software work under delegation — derived from a living corpus, and built so that humans, agents, and sub-agents in any combination can hand off work reliably when delivery must continue over time. Theory lives in `corpus/`; durable collaboration memory lives under `record/`.

- `corpus/` — the living theory body (axioms → theorems → directions).
- `record/` — the shared record between roles, partitioned by kind:
  - `decisions` — decisions with their reasons (what was decided in the residue)
  - `evidence` — records whose force does not route through the producer's self-assessment
  - `intent` — expressions of intent (what software should do and not do)
  - `leanings` — what the software leans on (borrowed parts, platforms, services, formats, counterparty systems)
  - `text` — software text (the means; the behavior is the point). Conventional monorepo runtime source lives here.

<!--REPOSITORY LAYOUT END-->

<!--VITE PLUS START-->

# Using Vite+, the Unified Toolchain for the Web

This project is using Vite+, a unified toolchain built on top of Vite, Rolldown, Vitest, tsdown, Oxlint, Oxfmt, and Vite Task. Vite+ wraps runtime management, package management, and frontend tooling in a single global CLI called `vp`. Vite+ is distinct from Vite, and it invokes Vite through `vp dev` and `vp build`. Run `vp help` to print a list of commands and `vp <command> --help` for information about a specific command.

Docs are local at `node_modules/vite-plus/docs` or online at https://viteplus.dev/guide/.

## Built-in Commands vs Scripts

`vp <name>` runs a built-in command. `vp run <name>` runs a `package.json` script or a `vite.config.ts` task. Scripts cannot overwrite built-ins, so `vp dev` and `vp run dev` may do different things. Check `package.json` and `vite.config.ts` first, and run `vp run <name>` when the project defines a script or task with that name.

## Review Checklist

- [ ] Run `vp install` after pulling remote changes and before getting started.
- [ ] Run `vp check` and `vp test` to format, lint, type check and test changes.
- [ ] Check if there are `vite.config.ts` tasks or `package.json` scripts necessary for validation, run via `vp run <script>`.
- [ ] If setup, runtime, or package-manager behavior looks wrong, run `vp env doctor` and include its output when asking for help.

<!--VITE PLUS END-->
