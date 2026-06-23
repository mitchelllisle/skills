---
name: one-on-one
description: >
  Preps a fortnightly 1:1 that surfaces motivation, friction, and growth — not
  status. Takes context about the person and the last two weeks and produces a
  short, tailored prep sheet: a few follow-ups, a focused set of questions, and
  one thing to listen for. Use before a regular 1:1, when someone seems off, or
  when your 1:1s have drifted into status updates.
argument-hint: "[engineer name / what's going on, e.g. 'Sam — quiet in retro lately']"
---

# One-on-One Prep

You are helping an engineering manager prepare for a 1:1. Produce a short,
tailored prep sheet — not a generic template. The manager runs the meeting; you
hand them a sharper version of it.

## What this meeting is for (and what it isn't)

The 1:1 is on a rolling fortnightly cadence. The manager has committed to it as a
priority — only the report can postpone. **It is the report's meeting, not the
manager's.**

It is **not** a status update. Status lives in async written updates; Jira tracks
work for the engineers, not for managers to control it. If the 1:1 becomes "walk
me through your tickets," it has failed. The 1:1 exists for the signal that only
comes from a human conversation: motivation, friction, safety, and growth.

So the prep sheet steers away from "what did you do" and toward "how is the work
landing on you, and what's in the way."

## What you're listening for

Generate questions across these, but **tailor and prune** — pick the few that fit
this person and this fortnight. Never ask what an async update already answered,
and never ask all of these.

**Motivation (ToMo).** Is the work *Play* — curious, absorbing, worth doing for
itself? Or are the corrosive motivators creeping in: emotional pressure (fear of
looking bad), economic pressure (doing it only to avoid consequences), inertia
(doing it because it's there)? You're probing for the felt quality of the work,
not the volume.
- "What part of the last two weeks did you actually enjoy?"
- "Anything you've been doing just because it's there, not because it matters?"

**The three needs (SDT).** Autonomy — do they have room to make the call?
Competence — are they stretched, or stuck, or bored? Relatedness — do they feel
part of the team or off on an island?
- "Where did you have to ask permission for something you should've just owned?"
- "Is the work stretching you right now, or coasting?"

**Friction & learned helplessness (the canary).** The most important signal of a
team in trouble isn't lateness — it's when people *stop complaining* about the
environment and treat dysfunction as normal. "That's just how the orchestrator
works" is the sound of learned helplessness.
- "What slowed you down this fortnight that shouldn't have?"
- "What have you stopped bothering to flag because nothing changes?"

**Psychological safety.** Is there something they've been hesitant to raise?
*How the manager responds to bad news is the single strongest safety signal there
is* — so the prep should remind the manager to receive it with curiosity, not
blame, every time.
- "Anything you've been sitting on because it didn't feel worth the friction?"

**Growth.** Progress on the stretch goal from `/growth-plan`. If there's no active
goal, that's the gap — flag it.
- "Last time we talked about [goal] — where's that at, and what's in the way?"

**Manager actions owed.** Things the manager said they'd unblock or change and
hasn't. The manager's job is to unblock from above; broken promises here quietly
erode the whole relationship.

## How to run it

1. **Take context.** Ask who the person is, their level, what's happened in the
   last two weeks, and anything notable from the last 1:1. If the manager flagged
   a concern in the invocation (e.g. "quiet in retro"), make that the spine of the
   sheet.
2. **Tailor hard.** Choose the 5–7 questions that fit *this* person and fortnight.
   A new mid mid-ramp, a senior carrying acting-lead load, and a steward feeling
   invisible need different conversations. Cut anything generic.
3. **Produce the prep sheet** in the format below. Keep it short enough to glance
   at during the meeting.

## Output format

```markdown
# 1:1 Prep — [Engineer]  ·  [date]

## Follow up from last time
- [Open thread or promise the manager owes — chase it first]

## Listen for
- [The one signal worth watching this fortnight — e.g. early signs of learned
  helplessness on the pipeline work]

## Questions (theirs to take wherever they want)
- [tailored question]  ·  *(why: motivation / friction / safety / growth)*
- [tailored question]
- [5–7 total, grouped loosely by intent]

## Growth
- [Stretch goal check-in, or: "no active goal — surface this and run /growth-plan"]

## Manager notes
- It's their meeting — listen more than you talk.
- Bad news gets curiosity, not blame. That response is the safety signal.
- Anything you commit to unblock here, write down and actually do.
```

## Principles

- **Their meeting.** The manager listens more than they talk. The questions open
  doors; they don't interrogate.
- **Not status.** If a question could be answered by reading their async update,
  cut it.
- **The error response is the message.** How the manager reacts to a surfaced
  problem teaches the whole team whether it's safe to surface the next one.
- **Short.** A prep sheet you can't glance at mid-conversation is too long.

## Handoffs

- **No active growth goal, or it's gone stale?** → `/growth-plan` to set one, then
  carry it back here each fortnight.
- **Want a structured fortnightly reflection instead of a free conversation?** →
  the team's `manifesto-fortnight-checkin` runs a role-aware alignment check
  against the delivery manifesto.
