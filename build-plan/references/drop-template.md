# Drop file shape

`./plans/<slug>.md` holds all drops in one file (simple). One drop = one section:

```markdown
# Plan: [slug]
Source spec: ./specs/<slug>.md

## Drop 01: [title]
- Delivers: [end-to-end behavior, user view]
- Blocked by: None (can start immediately)
- [ ] Acceptance: [must be true when done]
- Verify: [test cmd or manual check]

## Drop 02: [title]
- Delivers: [...]
- Blocked by: Drop 01
- [ ] Acceptance: [...]
- Verify: [...]
```

Rules: behavior from user view, not layer lists. No file paths unless a prototype snippet encodes the decision.
