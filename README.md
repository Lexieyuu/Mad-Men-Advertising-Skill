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
3. **Advertising Agency Concept Board** — an internal creative-development presentation with sketches, studies, and concise notes.

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
│   └── mad-men-visual.md
└── tests/
    └── evaluation.md
```

## Status

This repository is an early draft for testing and iteration. There are currently no tags or published releases.
