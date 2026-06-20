# skills

My personal Claude Code skills library.

## What are skills?

Skills are markdown files that tell Claude how to behave for a specific task. Drop them into `.claude/skills/` in any project (or `~/.claude/skills/` globally) and invoke them with `/skill-name`.

## Skills

| Skill | Description |
|-------|-------------|
| [grill-me](./grill-me.md) | Quizzes you on your current codebase or a topic you specify. One question at a time, scored, with real feedback. |

## Usage

Copy any skill file into your project's `.claude/skills/` directory, then invoke it:

```
/grill-me
/grill-me Python decorators
/grill-me the auth flow in this repo
```
