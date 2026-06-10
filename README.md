# coding-dojo

[![skills.sh](https://skills.sh/b/rannieo/coding-dojo)](https://skills.sh/rannieo/coding-dojo)

An agent skill that turns your AI pair into a **coach instead of an autocomplete**. Works with any coding agent that supports the [Agent Skills](https://skills.sh) format.

When you're feeling rusty, over-reliant on AI, or just want to *keep* your hands-on coding skill, `coding-dojo` flips the agent's default. Instead of writing the code for you, it enforces a **keyboard split**: you write the decision-bearing code — the core function, the tricky condition, the schema, the algorithm — and the agent is allowed to type only boilerplate (imports, scaffolding, fixtures, config, plumbing).

It's deliberate practice, built into your workflow.

## Why

Agents amplify experience. But experience decays when you stop doing the hard parts yourself. This skill is a structured way to keep doing the reps that matter — without giving up the agent for the boilerplate that doesn't.

It's built on the principles in Drew Breunig's [*10 Lessons for Agentic Coding*](https://www.dbreunig.com/2026/05/04/10-lessons-for-agentic-coding.html).

## The loop

1. **Sketch first** — state your approach in 3–5 lines; the agent critiques, doesn't replace it.
2. **Tests as contract** — you name the behaviors to assert; the agent can type the mechanics.
3. **You write the core** — the agent stays silent until asked, then reviews like a senior peer (names what's wrong and why; doesn't paste the fix).
4. **Taste reps** — when multiple approaches exist, the agent shows them *unlabeled*; you pick and justify.
5. **Comprehension gate** — anything the agent wrote, you explain back before it's accepted.
6. **Intent log** — one line per decision: what and why.
7. **The 2am question** — end each session with "what breaks at 2am, and how would you know?"

## The escape hatch

Say **`ship-mode`** on any task and the dojo fully steps aside — the agent just builds it. Use it for incidents, hotfixes, deadlines, or anything customer-impacting. Practice later.

## Install

```bash
npx skills add rannieo/coding-dojo
```

Your agent picks it up automatically when you say you want to practice or write something yourself. You can also invoke the `coding-dojo` skill explicitly — the exact syntax depends on your agent (e.g. a slash command in some, a skill mention in others).

## Pairs well with

The comprehension gate (step 5) gets sharper alongside a relentless-questioning skill. [**grill-me**](https://github.com/mattpocock/skills/tree/main/skills/productivity/grill-me) by Matt Pocock is a natural fit — it interviews you down each branch of your design until there's shared understanding:

```bash
npx skills add mattpocock/skills --skill grill-me
```

It's a separate, independently-licensed skill (not bundled here) — install it directly from its source.

## License

The skill content adapts principles from Drew Breunig's *10 Lessons for Agentic Coding*, which is published under **CC BY-NC 4.0**. This package is released under the same license — Attribution-NonCommercial 4.0 International. See [LICENSE](LICENSE).
