# skills

My personal Claude Code skills library.

## What are skills?

Skills are markdown files that tell Claude how to behave for a specific task. Drop them into `.claude/skills/` in any project (or `~/.claude/skills/` globally) and invoke them with `/skill-name`.

## Skills

Skills are organised by the persona they serve.

### Engineering Manager

| Skill | Invoke | Description |
|-------|--------|-------------|
| [growth-plan](./engineering-manager/growth-plan.md) | `/growth-plan` | Builds a development plan for one engineer against the team's role ladder — diagnoses the gap to the next level, sets one quarterly stretch goal framed for intrinsic motivation, and names the support the manager owes. |
| [one-on-one](./engineering-manager/one-on-one.md) | `/one-on-one` | Preps a fortnightly 1:1 that surfaces motivation, friction, and growth instead of status — produces a short, tailored prep sheet of follow-ups, questions, and one thing to listen for. |

### Tech Lead

| Skill | Invoke | Description |
|-------|--------|-------------|
| [initiative-plan](./tech-lead/initiative-plan.md) | `/initiative-plan` | Takes an initiative description, outcome, and date and produces a phased technical plan across the medallion stack. |
| [domain-doc](./tech-lead/domain-doc.md) | `/domain-doc` | Guided DDD session to extract and document a domain's ubiquitous language, bounded contexts, events, and key decisions. |
| [grill-me](./tech-lead/grill-me.md) | `/grill-me` | Quizzes you on your current codebase or a topic you specify. One question at a time, scored, with real feedback. |
| [domain-audit](./tech-lead/domain-audit.md) | `/domain-audit` | Audits a codebase for alignment with domain language — finds naming drift, missing domain concepts, and structural gaps. |

### Engineer

| Skill | Invoke | Description |
|-------|--------|-------------|
| [conduit-core](./engineer/conduit-core.md) | `/conduit-core` | Language-agnostic core of the conduit discipline — the ladder, laziness, security, and intensity levels (lite, full, ultra). Pair with a language skill. |
| [conduit-py](./engineer/conduit-py.md) | `/conduit-py` | Python conduit tooling — Pydantic at boundaries, stdlib-first functional style, Spark/Databricks patterns, Google docstrings, pytest + hypothesis. Reads conduit-core. |
| [conduit-ts](./engineer/conduit-ts.md) | `/conduit-ts` | TypeScript conduit tooling — Zod at boundaries, strict tsconfig, JS→TS on touch, React/Svelte patterns, TSDoc, Vitest + fast-check. Reads conduit-core. |
| [ship-and-watch](./engineer/ship-and-watch.md) | `/ship-and-watch` | Opens a PR with the GitHub CLI, then polls until checks pass, the PR is approved, and every review thread is resolved — gating on thread resolution, not "changes requested" — merges, and summarises what changed and which suggestions were addressed. |

## Usage

Copy any skill file into your project's `.claude/skills/` directory, then invoke it:

```
/grill-me
/grill-me Python generators

/domain-doc
# walks you through building domain documentation interactively

/domain-audit
# point it at a repo and a glossary — get a structured alignment report
```
