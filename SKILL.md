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

## Choose one mode

- Default to **Premium Commercial Illustration** when the user simply asks for a Mad Men or vintage Madison Avenue treatment. Read [prompts/premium.md](prompts/premium.md).
- Use **Editorial Commercial Illustration** when the user asks for a magazine, editorial, lifestyle, or story-page treatment. Read [prompts/editorial.md](prompts/editorial.md).
- Use **Advertising Agency Concept Board** when the user asks for a proposal, campaign direction, internal presentation, or agency concept. Read [prompts/agency.md](prompts/agency.md).

Do not invent a fourth mode. Generate one mode per request unless the user explicitly asks for all three. Do not combine modes into a triptych or comparison sheet by default.

## Context isolation

Use only the subject and requirements in the current request. Do not carry over people, products, backgrounds, props, or creative directions from earlier examples unless the user explicitly asks to continue them.

## Preflight and review

Before generation, determine the subject type and mode, then explicitly preserve the subject count, identity, pose, and defining structure in the image instructions.

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
