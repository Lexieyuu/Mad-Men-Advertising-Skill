# Mad Men Advertising Skill

> Draft / Work in progress — no formal release has been published.

A visual-direction skill for transforming user-supplied people, pets, architecture, food, and products into 1950s–1960s Madison Avenue commercial art while preserving the original subject.

## Core principles

- Preserve the exact subject, identity, pose, structure, and subject count.
- Treat the uploaded image as a subject reference, not a style reference.
- Use hand-painted mid-century advertising language rather than a modern AI look or a simple vintage filter.
- Never add people, animals, or characters unless the user explicitly requests them.
- Use one output mode per request by default.

## Three modes

1. **Premium Commercial Illustration** — finished advertising artwork with no typography.
2. **Editorial Commercial Illustration** — a magazine-style story told through setting, props, light, and composition.
3. **Advertising Agency Concept Board** — a black-and-white, hand-drawn internal creative-development presentation with rough sketches, construction lines, studies, and concise notes. Color appears only when explicitly requested.

## Curated style cases

The reference index includes museum and archive examples for the visual foundation and each mode:

- David Klein — bold Jet Age commercial composition
- Stan Galli — direct, resolved premium commercial illustration
- Mac Conner — hand-painted advertising and editorial storytelling
- George Lois archive — concept-first agency development

See [`references/style-cases.md`](references/style-cases.md). These are learning references, not assets to copy.

## Use the skill

Give an Agent the raw Skill URL and ask it to load the instructions:

```text
https://raw.githubusercontent.com/Lexieyuu/Mad-Men-Advertising-Skill/main/SKILL.md
```

Example request:

```text
Load this skill, then transform my uploaded image into a Mad Men-era premium commercial illustration.
```

If no mode is specified, the skill defaults to **Premium Commercial Illustration**.

## Repository structure

```text
Mad-Men-Advertising-Skill/
├── SKILL.md
├── prompts/
│   ├── premium.md
│   ├── editorial.md
│   └── agency.md
├── references/
│   ├── mad-men-visual.md
│   └── style-cases.md
├── examples/
│   ├── subject-directions.md
│   ├── person.md
│   ├── pet.md
│   └── architecture.md
└── tests/
    └── evaluation.md
```

## Status

This repository is an early draft for testing and iteration. There are currently no tags or published releases.
