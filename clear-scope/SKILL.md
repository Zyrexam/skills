---
name: clear-scope
description: Turn vague build idea into clear scope and MVP. Use when user says vague idea, twitter clone, what to build, features, MVP, scope this.
---

From idea-refine (diverge -> converge) + interview-me. You sharpen BEFORE any spec.

## Philosophy

- Simplicity wins. Smallest version that still solves the real problem.
- Start from user experience, work backwards to tech.
- Say no to 1000 things. The Not doing list is the most valuable output.
- Be honest, not a yes-machine. Weak ideas get kind pushback.

## Process

### 1. Restate + sharpen (max 3 questions)

Restate as `How Might We...` in 1 line: who + problem.
If who/success unclear, ask max 3: who specifically, core action, constraint.
Do not proceed until who + success are clear.

### 2. Diverge lightly (one round)

Propose 3-4 variations using 2-3 lenses: simpler 10x version, audience shift, 10x scale version.
Ask which resonates. One round only - no 20-idea dumps.
See `examples.md` for twitter-clone walkthrough.

### 3. Converge to core loop

Define core loop in 2-3 steps (e.g. post -> follow -> feed). Everything must serve it.
Cut anything that does not serve the loop to Later or Not doing.

### 4. Stress-test

For chosen direction, write 3 lines:
- Value: painkiller or vitamin? Who benefits how much?
- Hardest part: technical/resource cost in 1 line.
- Riskiest assumption + how to test it in 1 day.

### 5. Ship 1-pager

Fill `references/scope-template.md` and save to `./scopes/<slug>.md`.
Not doing list is mandatory with why for each.

Ask approve, then offer `@build-spec on <slug>`. Do not write spec here.

## Anti-patterns

- 20 shallow ideas instead of 3-4 considered ones.
- Skipping who-is-it-for.
- No assumptions surfaced.
- Yes-machining a weak clone idea ("twitter but better" with no edge).
- Jumping to features before core loop.

## Verification

- [ ] HMW problem statement exists
- [ ] User + success defined
- [ ] Core loop 2-3 steps
- [ ] MVP max 5, Later + Not doing with reasons
- [ ] Riskiest assumption + 1-day test
- [ ] Saved to ./scopes/<slug>.md, user approved
