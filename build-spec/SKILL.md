---
name: build-spec
description: Turn clear scope into buildable spec doc. Use when user says spec, PRD, freeze requirements, what exactly to build.
---

From to-spec + spec-driven-development. You synthesize, you do NOT re-interview.

## Philosophy

- Code without spec is guessing. 15-min spec prevents hours of rework.
- Spec is the shared truth between human and builder. If it is not written, it was not decided.
- Surface assumptions now. Silent guessing is the most expensive bug.

## Process

### 1. Gather input

Read `./scopes/<slug>.md` or current conversation. If neither, say run `@clear-scope` first.
If 1 gap blocks spec, write `ASSUMING: ... -> correct me` and proceed. Never stall on trivia.

### 2. Ground in repo

Skim repo for seams: prefer existing test seams, highest seam possible, ideally one.
Confirm seams with user in 1 line. Respect Out of scope from clear-scope.

### 3. Write spec

Fill `references/spec-template.md`. Rules:
- No file paths or code dumps (they rot fast).
- Exception: tiny snippet only if it encodes a decision (state machine, schema, type shape) better than prose.
- User stories as `As <actor>, I want <feature>, so that <benefit>`, 3-8 stories.
- Testing section says what a good test is (behavior, not implementation) + where tests go.

Save to `./specs/<slug>.md`. Summarize + list Open questions.

### 4. Gate (CRITICAL)

Ask approve or change. Then STOP. Do NOT plan, ticket, or code in same turn.
Planning starts only after human approves in a later turn.

Wire-out: after approve, offer `@build-plan on <slug>`.

## Anti-patterns

- Re-interviewing everything clear-scope already settled.
- Spec with file paths that rot in a week.
- "Simple, no spec needed" - even 2-line acceptance beats none.
- Writing spec after code (that is docs, not spec).
- Spec + plan + code in one turn.

## Verification

- [ ] Problem, Solution, Stories, Implementation, Testing, Out of scope all filled
- [ ] Assumptions listed explicitly
- [ ] No stale file paths
- [ ] Saved to ./specs/<slug>.md
- [ ] Human approved before any plan work
