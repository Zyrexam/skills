# My Skills

Learning how software-factory skills work by building my own.

## Skills

- `grill-me/` — asks tough questions on a topic. If no topic given, picks one from current project.
- `teach/` — teaches a concept simply (what / how / why) with one example, one recall question, and one HTML lesson in `./lessons/`.

## How to use

Mention by ID in agent:

```text
@grill-me grill me on REST APIs
@teach teach me closures
```

## How a skill works

Each skill is a folder with a `SKILL.md`:

```text
skills/
  grill-me/SKILL.md
  teach/SKILL.md
```

`SKILL.md` has frontmatter (`name`, `description`) + short steps. `description` decides when agent loads it. ID comes from folder name.

Derived from: Matt Pocock skills, pstack teach/how/why, Addy Osmani patterns.
