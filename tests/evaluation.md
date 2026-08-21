# Evaluation

This file defines the evaluation rules and current validation scope for `v0.1.0-beta`. Score the retained showcase from 1 to 5 and require at least 4 for acceptance, while treating every hard failure as an automatic regeneration.

## Current validation scope

Retain one representative visual case:

- **Case 01 — People ensemble:** eleven-person ensemble; completed and retained as the sole showcase case, with the [original reference](../examples/people/case-01-people-ensemble-original.jpeg) and three fixed-mode outputs:
  - [Premium Commercial Illustration](../examples/people/case-01-people-ensemble-premium.png)
  - [Editorial Commercial Illustration](../examples/people/case-01-people-ensemble-editorial.png)
  - [Advertising Agency Concept Board](../examples/people/case-01-people-ensemble-agency-concept.png)

No additional person, pet, architecture, product, or food case is required for this beta draft. Those subject types remain supported directions in the Skill instructions, but they have not been validated by retained case images.

Case 01 demonstrates the intended visual system across all three fixed modes; it does not prove stable performance across every supported subject category. Describe `v0.1.0-beta` as an experimental beta with limited validation.

## Hard failures

Regenerate if any of these occur:

- a person, pet, product, building, or food subject loses its identity
- a person's face, pose, gesture, or body position changes materially
- a product's form, package, label structure, or construction is redesigned
- a pet's breed, coat, markings, or distinguishing features change
- any unrequested person, animal, character, model, or duplicate subject appears
- Premium mode contains any text
- multiple modes are mixed without an explicit request
- Agency mode contains a colored or polished hero image when color exploration was not explicitly requested
- the output looks like modern AI art or only a vintage photo filter
- unrelated content from a previous request appears

## Subject-preservation hard failures

The output also fails automatically if:

- subject count changes
- either identity in a multi-person image is replaced, blended, or swapped
- left and right placement or front and back depth changes
- a held object disappears, changes hands, or moves to another subject
- an accessory is removed or replaced
- pose, gesture, or interaction meaning changes
- a new advertising character, background figure, or reflected figure appears
- typography, a product, a prop, or decoration obscures a face or identity-defining feature
- a supplied logo is altered
- an unsupported brand or logo is invented

## Mode checks

### Premium

- one clear hero subject
- clean, elegant, finished commercial artwork
- no typography of any kind

### Editorial

- magazine-story atmosphere
- narrative comes from setting, props, light, and space
- optional typography is concise and period-appropriate
- no additional people or characters are used to manufacture story

### Agency

- visibly exploratory rather than final
- entirely hand-drawn in black-and-white pencil, charcoal, ink, or marker by default
- includes unfinished lines, thumbnails, layout or crop studies, arrows, corrections, and concise creative notes
- contains no colored or polished hero image; limited color studies appear only when explicitly requested
- contains no invented brand, logo, endorsement, or unsupported claim

## Subject matrix

- **Person:** same identity, face, hairstyle, apparent age, pose, gesture, and count.
- **Product:** same silhouette, packaging, construction, proportions, and recognizable identity.
- **Food:** same food identity and defining preparation; appetizing commercial treatment without substitution.
- **Architecture:** same building structure and defining geometry; not merely an aged-photo effect.
- **Pet:** same species or breed, coat, markings, proportions, pose, and count; never add an owner by default.

## Retained-case record

Use this structure only when documenting the retained Case 01 results.

```markdown
# Case 01 — People Ensemble

## Input

Describe the original input image and its subject count.

Current retained input count: 11 people.

## Expected Preservation

Record the attributes that must remain unchanged:

- subject count
- identity
- pose and gesture
- held objects and accessories
- spatial relationships
- defining structure

## Failure Type

Record one or more:

- identity drift
- subject count error
- pose mutation
- object mutation
- extra character
- composition change
- spatial relationship change
- subject obstruction
- structural change
- typography violation
- mode violation

## Correction

Record the exact rule or prompt constraint used to correct the failure.

## Result

Record the result after correction for each fixed mode and note the original/output evidence.

## Decision

PASS / REGENERATE
```
