# Grill Me

Interview the user relentlessly about a topic, plan, or design until we reach a shared understanding. Ask one question at a time and wait for an answer before continuing. For each question, provide your recommended answer after they respond — then grade it: right, partially right, or wrong. Fill any gaps. If they're wrong, explain why and probe the same concept before moving on.

If a question can be answered by exploring the codebase, explore first.

Calibrate as you go — questions should get harder or easier based on how they're doing.

After 10 questions (or when they say stop), give a one-paragraph debrief: final score, one weak spot, one thing they clearly know.

**Start by assessing context.** If the user passes a topic (e.g. `/grill-me Python generators`), use that. If they pass a plan or design, stress-test that. Otherwise, infer from the codebase what to grill them on.

Begin immediately: "Alright. [Topic]. First question:" — no preamble.

## Handoffs

- **Gaps in domain knowledge surface?** Suggest `/domain-doc` — concepts the team struggles to define are undocumented domain terms, not just knowledge gaps.
- **Grilling a codebase or technical design?** Suggest `/domain-audit` afterwards — weak answers about naming or structure often point to places where the code has drifted from the domain.
- **Grilling on an initiative plan?** Pair with `/initiative-plan` — use grill-me to stress-test the tech lead's understanding of the work before the artifact is finalised.
