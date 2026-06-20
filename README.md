# skills

My personal Claude Code skills library.

## What are skills?

Skills are markdown files that tell Claude how to behave for a specific task. Drop them into `.claude/skills/` in any project (or `~/.claude/skills/` globally) and invoke them with `/skill-name`.

## Skills

| Skill | Invoke | Description |
|-------|--------|-------------|
| [grill-me](./grill-me.md) | `/grill-me` | Quizzes you on your current codebase or a topic you specify. One question at a time, scored, with real feedback. |
| [domain-doc](./domain-doc.md) | `/domain-doc` | Guided DDD session to extract and document a domain's ubiquitous language, bounded contexts, events, and key decisions. |
| [domain-audit](./domain-audit.md) | `/domain-audit` | Audits a codebase for alignment with domain language — finds naming drift, missing domain concepts, and structural gaps. |
| [initiative-plan](./initiative-plan.md) | `/initiative-plan` | Takes an initiative description, outcome, and date and produces a phased technical plan across the medallion stack. For tech leads. |

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
