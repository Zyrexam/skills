# My Skills

Learning how software-factory skills work by building my own.
Each skill does one job and hands off to the next.

## Chain

```text
vague idea -> @clear-scope -> @build-spec -> @build-plan -> build
stuck      -> @teach <-> @grill-me (learn <-> test loop)
```

| Skill | Job | Output |
|---|---|---|
| `clear-scope/` | vague (twitter clone) -> MVP scope + Not doing | `./scopes/<slug>.md` |
| `build-spec/` | scope -> frozen spec, stops for approval | `./specs/<slug>.md` |
| `build-plan/` | spec -> 5-7 drops with Blocked by | `./plans/<slug>.md` |
| `teach/` | concept -> what/how/why + example + recall Q | chat + `./lessons/0001-<topic>.html` |
| `grill-me/` | topic -> 5 questions easy->tough + score | chat + weakest areas |

Supporting files: `references/` templates + `examples.md` where needed. Paths inside skills are relative to that skill's folder.

## How to use

```text
@clear-scope I want to build a twitter clone
@build-spec on twitter-clone
@build-plan on twitter-clone
@teach teach me JWT auth
@grill-me grill me on REST APIs
```
