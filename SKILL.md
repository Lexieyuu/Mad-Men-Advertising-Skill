---
name: mad-men-advertising
description: "Transform an uploaded photo into one of three distinct mid-century commercial illustration modes: Bernie Fuchs premium illustration, Al Parker editorial page, or Austin Briggs black-and-white development drawing. Use when the user asks for Mad Men-era advertising illustration while retaining the real subject."
---

# Mad Men Advertising

This file is the complete runtime instruction set. Do not depend on linked prompt files or reference files to decide how to generate. The uploaded image supplies subject facts; this skill supplies the visual language.

## Output contract

Generate exactly one selected mode per image. If the user asks for all three, make three independent images, never a triptych or comparison sheet.

If the user does not specify a mode, use **Editorial Commercial Illustration / 编辑式商业插画** by default.

Match the generated image to the uploaded source image's exact pixel width and height whenever the image tool supports custom dimensions. The artwork itself must fill that canvas: do not add an outer background, letterbox, pillarbox, border, blank margin or solid-color extension merely to reach the target dimensions. Preserve the source orientation. If the tool only offers preset sizes or a different aspect ratio, recompose the artwork inside the target frame and use a deliberate, safe crop or scene extension within the artwork; never stretch, pad or frame a smaller image to fake the source dimensions. Identity-defining and relationship-defining content must remain complete and readable.

The three fixed modes are:

1. **Premium Commercial Illustration / 精致商业插画** — Bernie Fuchs direction; finished color commercial illustration; no text by default.
2. **Editorial Commercial Illustration / 编辑式商业插画** — Al Parker direction; illustrated magazine page; typography is required by default.
3. **Advertising Agency Concept Board / 广告公司提案稿** — Austin Briggs direction; black-and-white, step-by-step advertising development board.

Do not create a fourth mode and do not blend modes.

## Before generating: separate facts from the photograph

Extract and lock only these facts from the uploaded image:

- exact number of people, animals, products and primary objects;
- each person’s recognizable face, apparent age, hairstyle, clothing, body proportion, pose, gesture and hand action;
- the identity and functional structure of products, animals, food and architecture;
- key person-to-person, person-to-object and object-to-space relationships.

Do **not** lock the original camera angle, crop, full background detail, lighting, color grading, negative space or visual hierarchy. The result must not be the same photograph painted over. Rebuild those choices in the selected mode.

Never add, remove, duplicate, merge, replace or beautify people. Never add animals, brands, logos, signatures, endorsements, prices or unsupported product claims. If the source contains readable brand text, retain it only when the chosen mode explicitly allows source text; otherwise convert it to unreadable graphic detail.

Cropping is allowed only when the remaining face, body, hand-object connection, product structure, animal feature or architectural node stays complete and readable. Do not crop through faces, joints, hands holding objects or essential structural connections.

## Generation order

1. Write the subject locks from the source image.
2. Select one mode.
3. Replace the photograph’s composition, surface and reading order with that mode’s module below.
4. Set the output canvas to the source image's exact width and height, or use the closest aspect-ratio preset and recompose/crop within the artwork when exact dimensions are unavailable; do not pad the image with an outer background.
5. Generate the image and verify its final pixel dimensions.
6. Reject and regenerate if it reads first as a movie still, a photo filter, generic AI oil painting, or the wrong mode.

## 1. Premium Commercial Illustration / 精致商业插画

### Role

Create a finished commercial or story illustration in the Bernie Fuchs direction. The first impression is a resolved mid-century printed illustration with clear graphic organization, not a cinematic scene and not an oil painting.

### Required visual construction

- Recompose the source as a complete story scene: keep the important people, props and environment, but create a new commercial visual hierarchy instead of tracing the source camera view. A scene may be spatially compressed, selectively cropped or joined by large color fields; it does not need continuous cinematic perspective.
- Use opaque color fields and selective ink contours as the main structure. Major background planes, garments, pavement and architecture should read as deliberately simplified print shapes, not continuously modelled photographic surfaces.
- Use a controlled, limited print palette. Let one or two large color fields establish the scene, then use a few decisive accents; warm yellow, red, blue, green, brown and black may be used when they serve the story. Avoid a uniformly detailed rainbow of local color, a muddy brown wash or sepia filtering.
- Preserve a person's likeness through their silhouette, hairline, face proportion, age cues, clothing and a few decisive facial marks. Faces must be recognizable but **low in descriptive resolution**: use simplified planes of light and shadow and sparse eye, nose and mouth marks; do not render pores, eyelashes, individual hair strands, glossy skin, detailed teeth or photographic expression modelling. The result must not be blurry—only selectively described.
- Use an explicit hierarchy of finish. The primary face, hand-to-object connection and story-bearing props get the clearest marks; secondary people, distant faces, background objects and architectural detail may collapse into silhouettes, partial contours, color shapes or open paper. Never give every figure and object the same polished level of detail.
- Build readable foreground, middle ground and background through overlap, scale, flattened depth, diagonals and color fields rather than through fully rendered perspective, photographic focus falloff or uniform environmental detail.
- Vary edge treatment deliberately: firm contours at important identity and action nodes; broken, omitted or partly overpainted edges elsewhere; occasional dry opaque coverage and visible paper at transitions are welcome. The medium is printed ink-and-opaque-gouache/casein illustration, not a pristine vector render: no thick oil bristles, wet paint, canvas weave, impasto, soft digital airbrushing or aged-photo filtering.

### Hard output rules

- One finished image only.
- No readable text, title, caption, signature, watermark, logo, border, label or decorative lettering.
- If the source includes a newspaper, sign or package text, render it as unreadable graphic print texture.

### Reject if

- it is a photorealistic movie still, photo colorization, any visible oil-paint/canvas/bristle texture, soft blended digital painting or a brown wash;
- it has high-definition, fully modelled photographic faces, equally polished background detail, uniformly closed outlines or sterile vector-like edge precision;
- it reduces a multi-person or multi-prop scene to an empty hero poster;
- it looks like an Editorial page, Agency sketch, grid or proposal board.

## 2. Editorial Commercial Illustration / 编辑式商业插画

### Role

Create a finished Al Parker direction magazine cover, illustrated feature page or commercial story page. The first impression must be an intentionally designed image-and-type page, not a Premium illustration with one headline pasted onto it.

### Required visual construction

- Recompose around a magazine reading route. Use asymmetric placement, open cream or white space, selective crop, overlap, diagonal movement and decorative line accents.
- Design the figures into expressive, readable illustrated forms: crisp ink-like contours, flat opaque color shapes, selective clothing patterns and bold accent colors. Preserve identity, but do not preserve the source’s photographic lighting or camera framing.
- Use clothing, shoes, hands, tools, furniture, products and architectural fragments as story devices. Space may be compressed, partially abstracted or interrupted by white space; it does not need full cinematic perspective.
- The image must have obvious editorial rhythm: unequal visual weights, purposeful empty space and text placed along movement, props and page edges.
- Typography is part of the illustration, not a clean software layout: use custom hand-drawn display lettering, show-card lettering, expressive serif forms, casual script or condensed hand-lettered print as the page needs. Let letters vary in scale, baseline, stroke and placement while remaining readable.

### Typography rules

Typography is required by default. Use one readable main title, one short supporting line and **five to ten** short, positive, scene-specific descriptions. The text should describe only visible actions, objects, environments, care, craft, energy or experience.

- The main title must be bespoke display lettering, not a default computer font. Give it a visible hand-drawn character: expressive serif, brush-like, show-card, calligraphic or playful letterforms selected to match the scene.
- Use two or three complementary lettering voices across the page: for example a large display title, a more intimate script or italic supporting line, and small hand-lettered print for short descriptions. Do not use one uniform font family everywhere.
- Keep phrases short and readable; distribute them along curves, diagonals, props, figure movement and page edges instead of setting them in a rigid left-aligned list. Slightly irregular baselines, spacing and printed imperfections are welcome when they serve the composition.
- Do not cover identity-defining faces, hands, shoes, product forms or key actions.
- Do not invent brands, clients, prices, guarantees, endorsements, technical claims or fake article body copy.
- If legible typography cannot be achieved, regenerate; do not silently collapse the mode into a textless Premium image.

### Hard output rules

- One complete illustrated editorial page.
- Text must be part of the composition, not a single footer or a UI card.

### Reject if

- it keeps the source as a realistic scene and merely adds a title;
- it has only one or two text elements, long fake newspaper columns, generic sans-serif typesetting, a mechanically aligned text list, modern dashboard cards or a rigid template;
- it looks like a Premium scene with recolored paint, an Agency sketch or a photo filter.

## 3. Advertising Agency Concept Board / 广告公司提案稿

### Role

Create an Austin Briggs direction black-and-white, step-by-step illustration development board. The first impression is an illustrator showing how a composition is being solved on paper: one dominant working drawing surrounded by unequal studies for grouping, layout, value and light. It should feel like an authentic agency art-direction process page, not a finished advertisement, a comic strip or a polished faux-vintage presentation board.

### Required visual construction

- Work in black graphite, charcoal, lithographic crayon and/or ink on warm white or cream paper. No color accents or colored washes.
- Make contour, gesture, proportion, perspective and structural relationships primary. Use varied line pressure: light searching lines, darker committed contours, selective crosshatching, occasional rubbed gray masses and open unfinished areas.
- Show credible working process through overdrawn corrections, erased passages, broken edges and unresolved construction lines. These marks must clarify an actual pose, object, light or spatial decision; never use random scribbles or a uniform gray filter.
- Build a clear step sequence on one sheet: a large central or slightly off-center overall composition containing the full source situation, plus several smaller studies that visibly test real decisions such as **GROUP STUDY**, **LAYOUT**, **VALUE** and **LIGHT**. These labels are optional, short, hand-written art-direction notes—not slogans, brands or body copy.
- Use 4–7 subordinate studies with unequal scale and finish: rough grouping thumbnails, alternate layout crops, a value mass test, a light/shadow test, and when useful a hand-to-object, foot-to-shoe, face-to-hat or structural-junction study. Each study must derive from the source and support a specific visual decision.
- Arrange studies organically around the main drawing with arrows, crop marks, loose registration lines, taped paper scraps or lightly pinned-looking paper edges. Keep generous paper visible. Never use a perfect grid, equal thumbnails, cards, UI panels or a clean presentation template.
- Make the step order readable through visual progression: exploratory small sketches first, a more resolved central composition next, and focused value/light refinements around it. Do not make every study equally finished.
- Keep natural observed body language. Do not turn subjects into heroic advertising poses.

### Hard output rules

- Strictly monochrome black, charcoal gray and white paper.
- No slogan, brand, logo, signature, watermark, price, endorsement, fake copy or decorative presentation furniture.
- Short functional handwritten labels such as **GROUP STUDY**, **LAYOUT**, **VALUE**, **LIGHT**, **CROP** or **POSE** are allowed when they identify a real study. Keep them sparse, legible, imperfect and subordinate to the drawings; do not add paragraphs or invented client language.
- Tape, paper scraps, arrows and crop marks are allowed only as believable process evidence, never as decorative stickers or a rigid scrapbook collage.
- Warm white/cream paper and unfinished areas must remain visibly present; the output must remain strictly monochrome apart from the paper tone.

### Reject if

- it is a color illustration converted to grayscale, a black-and-white photograph, a polished digital line drawing or a heavily shaded graphite painting;
- it is a perfect concept-board grid, scrapbook collage, UI-like layout or a polished labelled presentation;
- it has only one finished drawing with decorative notes, instead of a readable progression from rough studies to a resolved central composition;
- the crop breaks facial identity, hand-object contact, shoe structure or another essential relationship.

## Final visual QA

Before returning an image, answer all of these:

- Are the subject count, identity, pose and key relations still correct?
- Does Premium have no readable text and obvious opaque print-color construction?
- Does Editorial have a designed image-and-type reading route with one title, one support line and five to ten positive short descriptions?
- Does Agency have warm white paper, varied hand-drawn lines, a readable progression of group/layout/value/light studies, real construction/revision marks and no color or template grid?
- If file names were removed, would a viewer identify the three outputs by role rather than merely by palette?

If any answer is no, correct only that selected mode and regenerate. Do not import visual devices from one mode into another.
