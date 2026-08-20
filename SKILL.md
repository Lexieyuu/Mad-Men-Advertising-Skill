---
name: mad-men-advertising
description: Transform user-supplied people, pets, architecture, food, or products into 1950s–1960s Madison Avenue commercial art while preserving the subject. Use for Mad Men-era premium advertisements, magazine-editorial illustrations, and advertising-agency concept boards.
---

# Mad Men Advertising

Create commercial artwork rooted in the 1950s–1960s Madison Avenue advertising era. Treat the uploaded image as the source of subject identity and structure, not as the source of visual style.

## Non-negotiable priorities

Apply these in order:

1. Preserve the exact subject and its identity.
2. Preserve the number of subjects.
3. Preserve the original pose, gesture, and structure.
4. Apply the Mad Men-era visual language in [references/mad-men-visual.md](references/mad-men-visual.md).
5. Use exactly one output mode.
6. Add advertising expression without violating the earlier constraints.

For people, keep the same face, features, hairstyle, apparent age, pose, and body position. Do not replace the person with a model or beautify them into a different identity.

For products and objects, keep the form, packaging, construction, and recognizable identity. For pets, preserve breed, coat, markings, and distinguishing features.

Never add people, animals, or characters unless the user explicitly requests them. Build narrative through environment, props, lighting, and composition instead.

When visual examples are needed to distinguish the period or the three modes, read [references/style-cases.md](references/style-cases.md). Learn only visual logic; do not copy subjects, brands, wording, or exact layouts.

When adapting the system to a person, pet, building, food, or product, read the matching section of [examples/subject-directions.md](examples/subject-directions.md). For detailed person, pet, or architecture cases, follow that file's link to the relevant example document; do not load unrelated case types.

## Subject Preservation Protocol

### Generation Preflight

Complete this Generation Preflight before any creative transformation. Treat every recorded attribute as locked unless the user explicitly requests a change.

### Subject count

Record the exact number of:

- people
- animals
- products
- primary objects

The output must preserve each count.

### Identity lock

For every person, record and preserve:

- facial identity and defining features
- hairstyle and apparent age
- clothing structure
- body proportions

For animals, products, food, architecture, and other primary objects, record and preserve their distinguishing identity and structure.

### Pose lock

Record and preserve:

- body pose and direction
- gesture and action
- hand placement
- seated or standing state

### Object lock

Record and preserve:

- held objects and their hand relationships
- accessories
- distinctive objects
- supplied logos and labels
- product construction and packaging structure

Do not remove, replace, relocate, duplicate, or redesign a locked object.

### Spatial lock

Record and preserve:

- left and right positions
- front and back depth
- distance and relative scale between subjects
- overlap, contact, and occlusion relationships
- the defining relationship between the subject and its environment

Do not begin visual-style transformation until this preflight is complete. If a creative decision conflicts with a locked attribute, preservation wins.

Use this preflight structure in the generation instructions:

```text
Subject count:
Identity locks:
Pose and gesture locks:
Object locks:
Spatial locks:
Selected mode:
Typography rule:
Forbidden changes:
```

## Creative Boundary Protocol

Creative additions may support the selected advertising mode, but must never replace, obscure, duplicate, or materially alter a locked subject, object, or relationship.

Allowed additions include:

- Madison Avenue-era advertising environments
- commercial-illustration elements
- editorial composition
- lighting and material treatments
- unbranded period-appropriate props and decorative elements

Do not invent a brand, logo, endorsement, or product claim. Brand displays are allowed only when supplied by the user or already visible in the input.

Forbidden changes include:

- adding fictional advertising people, models, consumers, salespeople, family members, coworkers, background figures, or reflected figures
- replacing or redesigning the uploaded subject
- changing identity, subject count, pose, gesture, or subject relationships
- swapping left and right positions or changing front and back order
- covering a face or identity-defining feature with typography, products, props, or decoration
- hiding or moving a held object
- modifying a product, package, building, food item, or other locked structure

For a people-based input, use only the people supplied by the user unless the user explicitly requests additional characters.

## Choose one mode

- Default to **Premium Commercial Illustration** when the user simply asks for a Mad Men or vintage Madison Avenue treatment. Read [prompts/premium.md](prompts/premium.md).
- Use **Editorial Commercial Illustration** when the user asks for a magazine, editorial, lifestyle, or story-page treatment. Read [prompts/editorial.md](prompts/editorial.md).
- Use **Advertising Agency Concept Board** when the user asks for a proposal, campaign direction, internal presentation, or agency concept. Read [prompts/agency.md](prompts/agency.md).

Do not invent a fourth mode. Generate one mode per request unless the user explicitly asks for all three. Do not combine modes into a triptych or comparison sheet by default.

The three mode names and roles are fixed:

1. **Premium Commercial Illustration** — 精致商业插画
2. **Editorial Commercial Illustration** — 编辑式商业插画
3. **Advertising Agency Concept Board** — 广告公司提案板

Do not introduce Advertising Photography, rename Editorial mode as photography, or add another output mode.

## Context isolation

Use only the subject and requirements in the current request. Do not carry over people, products, backgrounds, props, or creative directions from earlier examples unless the user explicitly asks to continue them.

## Preflight and review

Before generation, complete the Subject Preservation Protocol, select one mode, and include the resulting locks in the image instructions.

After generation, check:

- The result clearly reads as 1950s–1960s Madison Avenue commercial art rather than a modern AI illustration or a photo with a vintage filter.
- The subject, identity, pose, structure, and count are unchanged.
- No unrelated subject has been added.
- Premium mode contains no typography.
- Editorial mode tells its story through setting and composition.
- Agency mode is a monochrome, hand-drawn internal creative-development board made from rough pencil, charcoal, ink, or marker studies—not a finished advertisement.
- No material from an unrelated previous request appears.

Treat any identity change, pose change, added person, Premium typography, mixed modes, modern AI styling, simple photo filtering, or product redesign as a failed output. Use [tests/evaluation.md](tests/evaluation.md) for broader validation.

## Correct failures narrowly

- If identity drifts, strengthen identity preservation without adding more retro styling.
- If the pose changes, strengthen pose lock.
- If extra subjects appear, strengthen subject-count lock.
- If Premium contains text, strengthen the no-typography constraint.
- If Agency contains a colored or polished hero image, remove the color and finish; restore rough black-and-white hand-drawn studies. Permit limited color only when the user explicitly requests color exploration.
- If the result looks like a filtered photograph, strengthen hand-painted commercial illustration and printed-paper qualities.
- If the composition is busy, simplify the composition without deleting or altering the subject.
