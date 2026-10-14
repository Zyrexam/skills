---
name: teach
description: Teach a concept simply with example and check understanding. Use when user says teach me, explain, learn this.
---

Derived from Matt teach + pstack how/why + Osmani patterns.

## Philosophy

- Knowledge first (make it easy), skills second (make it stick with effort).
- Fluency is not mastery. Retrieval + spacing build real retention.
- Tie everything to the mission. Abstract lessons do not stick.

## Process

### 1. Mission

If goal/level unclear, ask 1 line: "What will you use this for?"
Record it at top of the lesson file. If mission changes mid-way, note the change.

### 2. Explain (what / how / why)

- What: 2 lines plain English, every jargon defined on first use.
- How: runtime flow + 1 tiny snippet, prefer real project code over toy code. Check files first, never invent APIs.
- Why: problem it solves + 1 alternative and when to pick which.
- Cite 1 trusted source (docs, not memory).

### 3. Osmani layer

1 practical example + pattern name + 1 pitfall + 1 performance/clean-code note.
Same example across lessons when possible (TodoMVC idea: one running example beats five fresh ones).

### 4. Check (desirable difficulty)

End chat lesson with 1 recall question from memory. Wait for answer, correct in 2 lines.
Quiz hygiene: answers same length, correct position varied, no format clues.

### 5. Save lesson

Write `./lessons/0001-<topic>.html` from `references/lesson-template.html`:
summary + example + 3 questions + source link. Reuse `./lessons/assets/` stylesheet if present, else create one.
Link file, offer to open (never auto-open).

Wire-out: shaky -> offer `@grill-me on <topic>`. Ready -> offer next level.

## Anti-patterns

- Lecturing without a check question.
- Toy examples when project code exists.
- 5 questions at once (working memory is tiny).
- Trusting parametric memory for API facts.

## Verification

- [ ] Mission recorded
- [ ] What/how/why all present
- [ ] 1 example + pitfall + source link
- [ ] 1 recall Q asked and corrected
- [ ] Lesson file saved and linked
