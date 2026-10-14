---
name: build-plan
description: Break spec into small buildable drops in order. Use when user says plan, drops, build order, what first, slice it.
---

From to-tickets (tracer bullets + blocking edges). You slice, you do NOT redesign scope.

## Philosophy

- Small deliberate steps. Rate of feedback is speed limit.
- Vertical drops, not horizontal layers. Each drop demoable alone.
- Blocking edges first. Frontier (blockers done) is what can start now.

## Process

### 1. Gather input

Read `./specs/<slug>.md`. If missing, say run `@build-spec` first. Respect its Out of scope.
If user passes a spec path as argument, read that file fully first.

### 2. Slice

Break into 5-7 drops. Each drop:
- cuts schema+API+UI+test (vertical, not one layer)
- demoable/verifiable alone
- fits one fresh session
- declares Blocked by (numbers/titles, or None)

Prefactor first if it makes rest easy ("make change easy, then easy change").
Wide mechanical refactors (rename column, retype shared symbol) use expand -> migrate batches -> contract, not forced drops.
See `references/drop-template.md` for file shape.

### 3. Quiz

Show Title + Delivers + Blocked by numbered list. Ask:
- granularity right? too coarse/fine?
- edges correct? merge/split any?
Iterate till user approves.

### 4. Publish

After approve, save to `./plans/<slug>.md` with checkboxes + acceptance + verify step per drop.
Work frontier first. Do NOT close/modify parent spec.

Wire-out: offer to start first frontier drop with TDD + review. Never auto-implement all.

## Anti-patterns

- Horizontal slices (all schema, then all API, then all UI) - nothing demoable till end.
- Drops with no acceptance or verify step.
- File-path implementation lists that rot.
- Skipping quiz and publishing mush.

## Verification

- [ ] 5-7 vertical drops, each demoable
- [ ] Every drop has Blocked by
- [ ] Acceptance + verify per drop
- [ ] User approved granularity
- [ ] Saved to ./plans/<slug>.md
