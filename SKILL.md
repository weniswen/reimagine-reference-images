---
name: reimagine-reference-images
description: Reimagine supplied reference images into clearly original, aesthetically compelling, physically coherent raster images while preserving the reference's creative engine, style era, attitude, broad category, and real visual appeal. Use when a user wants a fresh image inspired by a Y2K, retro-futurist, game-like, weird, playful, fashion, scenic, compositional, or material reference without copying its subject, dominant recognition anchors, relational structure, environment, or arrangement; when the user requests a changed background, character, object, ecosystem, or story; or when repeated generation must control concept breadth, originality distance, feedback experiments, subject visibility or anonymity, demographic drift, environmental causality, aspect ratio, and no-text constraints.
---

# Reimagine Reference Images

Create a new image from the reference's creative logic, not from its recognizable content or arrangement. Preserve the broad category, creative engine, style era, weirdness level, and attitude unless the user explicitly requests a change. The result should feel like a fresh idea from the same visual conversation, not an unrelated polished image.

## Required references

Read these before planning or generating:

- [references/originality-playbook.md](references/originality-playbook.md) for category preservation, transformation distance, and creative-tension patterns.
- [references/visual-quality.md](references/visual-quality.md) for the default aesthetic profile and anti-AI-artifact rules.
- [references/validation-checklist.md](references/validation-checklist.md) before accepting or delivering an output.

Also follow the installed `imagegen` skill for tool selection, reference-image roles, generation/edit semantics, and output handling.

## Core contract

- Treat an input image as a **reference image**, not an edit target, unless the user explicitly asks to preserve and modify that exact image. A reference plus only an aspect ratio means a new reimagining in that ratio; it does not authorize a crop, resize, or outpaint of the same scene.
- Treat explicit user criticism as a new invariant for the rest of the conversation. Do not defend, soften, or forget a rejected palette, exposure level, face treatment, composition style, or finish. Treat a suggested trial as provisional until the user accepts it; never convert an unsuccessful experiment into a permanent style rule.
- Treat originality, desirability, and execution as independent hard gates. A beautiful, realistic output still fails when its dominant camera-subject relationship or recognizable arrangement remains too close. A structurally original output fails when it is merely normal, aesthetically weaker than the reference, or poorly executed.
- Default to strong visual impact: build a decisive focal hierarchy, bold but controlled color, and clearly separated tonal or chromatic contrast. Reject washed-out, timid, low-contrast results even when they are technically clean. Soften this requirement only when the user explicitly requests restraint or when low contrast is indispensable to the reference's defining appeal; even then, preserve a clear focal contrast through scale, light, edge, material, or composition.
- Default to real-world logic. Unless the user explicitly requests fantasy, surrealism, or a changed physical law, every visible event must obey ordinary gravity, support, momentum, anatomy, animal behavior, ecology, scale, perspective, optics, illumination, reflection, material response, weather, and object function. A striking image fails when its story could not physically occur or when the scene contains unexplained contradictions. If the user requests one impossible premise, isolate that premise and keep all surrounding causes and consequences physically coherent.
- Compare against recent outputs before each generation. Avoid repeating the same dominant hue, lighting recipe, setting family, camera relation, facial archetype, or finish unless the reference or user specifically requires it.
- Consider environments beyond the reference before selecting a concept. Water, beach, forest, interior, or studio context is not automatically invariant; preserve it only when it carries the reference's creative engine or appeal.
- Extract a **style fingerprint** of 3–6 traits. Include the creative mechanism and, when present, an era or subculture signal such as Y2K, early digital, retro game hardware, futuristic toy design, punk collage, camp, absurd humor, or editorial fashion attitude.
- Separate the reference's real appeal from incidental execution. A visible blue cast, darkness, grayness, phone-camera look, or generic polish is not automatically part of the style fingerprint.
- Separate a visual sensation from the device that produced it: airy softness does not require silk or kites; story does not require people. Across consecutive reimaginings, vary the underlying mechanism, not just its location or shape.
- Treat **color + material + subject** as a potential dominant recognition bundle. Keeping flowers is allowed; retaining burgundy flowers with velvety petals after changing species and background is still too close. Redesign the palette and surface/light response when that pairing defines the source, unless explicitly asked to preserve it.
- **Perceptual-originality gate:** preserve the valued effect while reconstructing its dominant visual causes. Independently check subject appearance, environment, perceptual mechanism, and relationships; a surviving dominant recognition bundle in any layer vetoes the candidate regardless of changes elsewhere. Follow Step 3a before generation and repeat it on the rendered output. Respect explicit preservation locks.
- Use adaptive originality distance. Change 4–6 major dimensions by default, but do not change a dimension merely to reach a quota. Preserve the traits that explain why the reference is appealing.
- Preserve the broad category by default: landscape stays landscape, animal imagery stays animal-led, portrait stays portrait-led, collage stays collage, and conceptual illustration stays conceptual illustration.
- **Environment can be the complete subject.** Do not add people or animals merely to supply scale, story, movement, or a focal point. For environment-led and still-life concepts, default to no figures. Apply a removal test: if removing a proposed figure loses no essential meaning, omit it. Animal-led humor and explicitly requested human stories may retain their necessary protagonists; this is not a blanket ban on living subjects.
- **Standing user preference: keep people visually subordinate and faces difficult to identify.** When people are necessary, use environment-led framing with small human figures, not large foreground bodies or readable portrait faces. This overrides reference-derived face scale and portrait prominence unless the user explicitly requests a close portrait or clear face. Preserve human-led storytelling through relationships rather than enlarging the person. Apply this before prompting and again to the actual output; a prompt saying “incidental face” is insufficient.
- Low face visibility does not mean mandatory back views, silhouettes, or dim light. Prefer distance, a small side profile, or scene-motivated overlap while keeping the scene luminous and legible. Do not repeat a rejected rear-view/darkness combination under a different setting.
- Prefer simple, physically natural actions. Build story through environment, light, traces of activity, and object relationships; do not invent complex dance poses or theatrical gestures solely to supply “story.”
- Preserve visible human life stage, presentation, fashion attitude, and energy unless the user requests a demographic change. Change identity without using age, gender, or ethnicity as an originality shortcut. Never default to an older person merely to create distance. If age is unclear, use an age-neutral adult consistent with the reference.
- Separate **subject continuity** from **subject visibility**. Preserving life stage, presentation, and attitude does not require preserving a clear face, face-dominant scale, gaze, or identifiability.
- When a user dislikes how clearly an otherwise successful subject is shown, interpret that first as a visibility or prominence request, not permission to infer a preferred ethnicity, age, gender, body type, or beauty standard.
- Check recent outputs in the same conversation. Do not repeatedly choose the same demographic profile without a reference-based or user-specified reason.
- Preserve the reference's emotional intensity, humor, strangeness, playfulness, and visual-tension level without copying its literal symbols.
- Do not sanitize a weird, Y2K, retro-futurist, game-like, camp, rebellious, or deliberately awkward reference into generic premium editorial, serene human-interest photography, or tasteful minimalism.
- Treat scene-level causality as a hard constraint. Attractive color or composition does not excuse contradictory wave propagation, fluid behavior, smoke, fire, wind, support, reflection, or aftermath.
- Treat a copied relationship graph as copying even when the individual objects have been renamed or recolored. Change the action chain, support system, spatial grammar, or object ecology when a recognizable motif bundle remains.
- Do not confuse originality with ugliness or with arbitrary spectacle. Reject a concept whose novelty depends on harsh industrial clutter, oppressive scale, poor subject visibility, muddy light, or an oversized generic prop unless those qualities are reference-led and intentional.
- Treat cleanliness as removal of accidental noise, not as a mandate for low-poly geometry, large flat color blocks, plastic smoothing, textureless surfaces, or simplified CGI.
- Render no text, letters, numbers, logos, labels, signs, or watermark unless the user explicitly requests exact text.
- Honor the requested aspect ratio exactly in both planning and the generation prompt.

## Workflow

### 0. Capture feedback and recent-output drift

Before planning, write a compact internal ledger:

- **Rejected:** the user's explicit dislikes and the visible failures behind them;
- **Keep:** only the qualities the user actually endorsed, separately from overall output acceptance;
- **Experiment:** suggestions to try once without treating them as permanent constraints;
- **Vary:** palette, exposure, camera relation, setting, subject treatment, visibility, or finish that recent outputs have overused;
- **Edit lock:** for a narrowly corrected accepted image, the scene, composition, palette, lighting, physics, and other successful axes that must remain stable.

Classify feedback by intent, not merely by wording. A direct rejection is binding. A positive observation can strengthen `Keep`. A speculative phrase such as `try`, `maybe`, or `this might help` belongs in `Experiment` unless the user explicitly makes it a requirement. If the user dislikes the experiment, remove it completely from later prompts.

Treat “barely acceptable” as a direction to increase originality, not an approved template. Praise for one idea (such as jellyfish) does not approve its industrial staging, lighting, people, or later variants. Preserve that idea while redesigning the rejected execution.

When feedback follows a failed generation, return to the original reference by default. Do not use the rejected output as the next reference unless the user asks to edit that exact result. Change the root scene or lighting decision that caused the failure instead of appending a longer negative-prompt list.

When the user supplies a generated image and asks to “reimagine,” it is a new inspiration source, not permission to repeat that output's motif. Praise is not an instruction to make a series of the same object.

When the user explicitly accepts the concept and attaches or names the generated image while requesting one narrow correction, treat that image as the edit target. Use a preservation lock and change only the criticized axis.

### 1. Classify the reference

Identify:

- category and medium;
- primary subject or absence of one, including visible life stage, presentation, posture, and attitude;
- face scale, visibility, gaze, occlusion, identifiability, and whether appearance is central or incidental;
- environment skeleton;
- spatial topology, boundaries, support surfaces, and any upstream/downstream or inside/outside relationship;
- camera/viewpoint and composition;
- lighting, palette logic, material language, style era, and subculture signals;
- motion, force, humor, weirdness, or visual-tension level;
- the one creative mechanism that makes the image memorable.

Do not equate the mechanism with a literal object. For example, "a character connected to many clippings" may really mean "an individual under pressure from an external information system."

### 2. Lock the style fingerprint

Select 3–6 traits worth carrying forward. Include at least one creative mechanism and one style or attitude trait when present, such as:

- low-angle close perspective;
- layered foreground/midground/background depth;
- miniature character–vehicle storytelling;
- Y2K consumer-electronics styling;
- early-console or retro-game material language;
- cheeky, absurd, camp, rebellious, or deadpan humor;
- staggered downward movement;
- irregular torn-paper rhythm;
- one subject suspended in a decisive instant;
- calm reflective-versus-solid visual rhythm.

Write one short lock statement: `Keep <creative engine, style era, attitude>; change <literal content and recognizable arrangement>.` Treat it as an invariant during prompting and iteration.

Do not lock a palette merely because it is visually dominant. Preserve color only when it explains the reference's appeal and has not been rejected. Otherwise carry the energy through composition, material, motion, contrast, or attitude and design a new color system.

Do not lock a bundle of literal recognition anchors as the style fingerprint. For example, `young man + huge grin + mirrored glasses + face-filling fisheye + bright forest` is a recognizable arrangement, not five independent style traits. Abstract it to qualities such as exuberant outdoor playfulness, early-digital color, and optical wit.

### 3. Build an originality plan

Choose 4–6 axes to change. Change the axes most responsible for literal copying while protecting the style fingerprint:

1. subject identity, species, age, or type;
2. environment or ecosystem;
3. action or locomotion;
4. props, vehicle, clothing, or functional equipment;
5. camera relation and composition;
6. palette and lighting system;
7. narrative or symbolic meaning;
8. materials or medium-specific forms;
9. scale relationships;
10. supporting elements and spatial hierarchy.

For style-led portraits, character images, and playful concept images, default to moderate reconstruction: retain the reference's recognizable energy, life stage, and abstract creative engine while replacing the literal identity, object design, action details, arrangement, and any dominant camera-subject relationship responsible for recognition.

Reimagine the **composition format and surroundings**, not only the named location. Do not carry over the same spatial arrangement and environment family by calling them style. For setting-led references, change the environment skeleton and camera organization; layered colorful harbor houses becoming layered colorful hillside houses fails despite being a good photograph. Preserve abstract rhythm, attitude, or color energy through a new spatial structure.

Avoid exact pose, silhouette, focal placement, object cluster, path shape, crop, palette mapping, signature character, branding, or recognizable arrangement from the reference.

Also compare the reference and proposed concept as a relationship graph: `actor -> action -> object -> support surface -> surrounding props`. If that graph is still recognizable, change at least two structural relations rather than relying on cosmetic substitutions.

Axis count is supporting evidence, not a pass condition. Identify the 1–3 **dominant recognition anchors** first, such as face-filling scale, lens relation, signature pose, prop-face pairing, silhouette, or environment enclosure. If a dominant anchor or anchor bundle survives, reject the concept even when four or more lower-weight axes changed.

Write both relational signatures before generation:

`reference: actor -> action -> focal object -> support -> surroundings -> camera relation`

`proposal: actor -> action -> focal object -> support -> surroundings -> camera relation`

If both sentences still describe the same image at a glance, redesign the camera relation, action consequence, support system, or spatial grammar.

### 3a. Check perceptual originality before selecting a concept

Follow the general decision process in `references/originality-playbook.md` under **Perceptual originality**. Record `valued effect -> original cause -> dominant recognition bundles -> alternative cause -> visible evidence`, keeping explicit user locks separate. Diagnose subject appearance, environment, perceptual mechanism, and relationships independently. Develop candidate mechanisms first, then choose compatible subjects and settings. No changed layer compensates for an unchanged dominant bundle in another layer. Re-run the same checks on the actual output before delivery.

### 4. Design the new concept

Before choosing, generate 3–5 compact internal candidates that differ in structural premise, not only nouns. When the reference environment is incidental, span at least three setting families, such as natural, constructed, domestic, aerial, subterranean, ceremonial, or surreal. Include at least one cross-environment candidate and compare each candidate with both the reference and recent outputs.

For each candidate, record:

- the new relational signature and environment skeleton;
- the creative mechanism or causal event;
- the reference appeal it preserves;
- the main originality risk;
- the main aesthetic risk;
- whether figures are necessary, which color/material bundle changes, and whether the mechanism repeats a recent output.

Choose the candidate that best balances structural distance, reference fidelity, visual appeal, and generative feasibility. Do not choose the strangest candidate by default. Reject a mere location swap—such as the same portrait or action transplanted into an impressive place—when it lacks a new relationship, consequence, or visual rule.

Write a one-sentence concept before prompting. It must specify:

- what is new;
- which creative engine, style-era signal, and attitude remain;
- why the result is visually compelling;
- how it differs structurally from the reference.

For concept-driven references, retain an equivalent level of joke, contradiction, transformation, awkwardness, unusual scale, or directional force. Reject concepts that reduce a playful or eccentric reference to a conventional portrait. For calm landscapes, create discovery and layered rhythm rather than forcing in people or artificial drama.

Apply a **not-merely-normal gate**. The concept must contain at least one meaningful mechanism appropriate to the source: interaction, contradiction, transformation, directional force, discovery, causal event, or unusual spatial rule. Do not force surrealism or melodrama when a quieter visual mechanism would preserve the reference better.

Apply an **appeal-preservation gate**. Name what made the reference attractive—such as luminosity, intimacy, subject scale, facial charm, softness, palette elegance, tactile medium, playfulness, or scenic openness—and carry an equivalent quality into the new setting. Cross-environment imagination should expand the world without sacrificing the image's emotional and aesthetic payoff. Unless the user explicitly asks for restraint, strengthen the new image with a dominant visual event, saturated focal color, and clear value or hue separation rather than reproducing a weak or washed-out rendering.

For photographic references, name the intentional photographic decision: decisive light, camera relation, foreground anchor, motion behavior, spatial compression, or another clear point of view. Reject concepts whose only claim to realism is that they resemble a casual phone snapshot.

### 4a. Control subject visibility without demographic substitution

First apply the figure-necessity test. If people are needed, apply the standing small-figure, low-identifiability preference even when the latest request only gives a ratio. Define the person-to-environment scale and face visibility before choosing the camera. Do not invent a fixed percentage as a user requirement; judge the rendered composition.

When reducing visibility while keeping an accepted concept:

- preserve the accepted action, palette, environment, lighting, realism, and compositional energy unless the requested visibility change requires a local adjustment;
- reduce identifiability through a physically motivated side/back angle, smaller face scale, hair, gesture, crop, shadow, reflection, refraction, foreground overlap, or a concept-relevant prop;
- keep the person expressive through posture, action, clothing, color, and force response rather than relying on a readable face;
- prefer designed occlusion over censor bars, mosaic pixelation, arbitrary blur, masks, or face replacement unless the user explicitly requests one;
- do not translate `not my type` into an assumed demographic preference. Ask only if the user actually wants a different appearance rather than lower visibility.

For a narrow edit of an accepted image, use the supplied generated image as the edit target and state invariants explicitly: `change only face presentation; keep scene, framing, pose, clothing, palette, light, materials, shadows, and physics unchanged.` Make the correction visibly meaningful without letting the whole image drift.

For dynamic natural or material scenes, write a compact causality map before prompting:

`source/driver -> propagation direction -> boundary or interaction -> visible transition -> downstream effect -> dissipation/aftermath`

Map the relevant zones in the image. For example, a reef break should distinguish deep-water swell, shoaling or breaking line, shoreward whitewater/turbulence, and eventual calming; a poured liquid should preserve source composition, stream continuity, impact behavior, pooling, and drainage. If the concept cannot explain a sharp calm/rough, dry/wet, lit/shadowed, or solid/fluid boundary, redesign it.

For every scene, also run a compact **real-world plausibility audit** before prompting: `who/what can exist here -> what supports it -> what force or motive causes the action -> what visible response follows -> what traces remain`. Check species and habitat, age-appropriate and mechanically possible behavior, relative scale, access and attachment, camera perspective, light sources, shadows, reflections, and material state. Redesign any concept that depends on unexplained floating, impossible balance, incompatible ecology, nonfunctional props, contradictory lighting, or consequences without a cause.

### 5. Apply the default visual profile

Use the defaults in `references/visual-quality.md`, but let intentional reference style override taste defaults. In particular:

- preserve intentional Y2K color, retro-digital texture, futuristic lighting, flash photography, chromatic contrast, or awkward styling when those are part of the style fingerprint;
- pursue immediate visual impact through one dominant focal event, strong color presence, and crisp value or chromatic separation without blanket saturation, crushed shadows, clipped highlights, or competing accents;
- use rich layers and meaningful visual anchors without micro-clutter;
- distinguish intentional era texture and synthetic material language from accidental noise, plastic artifacts, HDR, or incoherent glow;
- choose scenes and materials that can satisfy these constraints instead of merely listing negative words.
- prevent cross-output palette collapse: do not repeatedly cover the sky, environment, clothing, and shadows with the same hue;
- when a face is visible at the chosen scale, keep it human rather than idealized; do not enlarge it or force readable eyes to demonstrate realism;
- distinguish natural photography from flat documentation. When the reference or feedback calls for a stronger image, create authorship through light, framing, depth, or a natural event rather than through saturation, HDR, or beauty retouching.
- audit every prominent prop for both function and visual fit. Do not add an ugly or generic catch-all object solely to make an action legible; integrate the support, receptacle, tool, or container into the concept's material and compositional language.
- interpret cleanliness instructions proportionally. Remove noise, dirt, and purposeless micro-detail while retaining organic surface variation, medium character, depth, and gracefully irregular forms. Do not collapse a photographic, painterly, or plush reference into smooth low-poly CGI.

### 6. Build the generation prompt

Use this compact structure:

```text
Use case: <taxonomy slug>
Asset type: <image type and aspect ratio>
Input images: Image 1 is an inspiration reference only; do not edit or reproduce it.
Feedback ledger: Rejected <binding dislikes>; Keep <accepted qualities>; Experiment <provisional trial only>; Vary <recently overused choices>
Recent-output variation: <overused palette, exposure, setting, face, or finish to avoid repeating>
Style fingerprint to retain: <3–6 traits including creative mechanism, era/style, attitude>
Reference appeal to retain: <luminosity, intimacy, charm, texture, subject scale, palette energy, or other real attraction>
Primary request: <new one-sentence concept>
Concept mechanism: <interaction, contradiction, transformation, force, discovery, causal event, or spatial rule that prevents a mere location swap>
Scene/backdrop: <new or reconstructed setting at the selected originality distance>
Subject continuity: <reference-aligned life stage, presentation, energy, or explicitly pure landscape; no unjustified demographic shift>
Figure necessity: <none by default for environments/still life; if present, indispensable role and removal-test result>
Subject visibility and scale: <if figures are necessary, small and subordinate, faces not clearly identifiable>
Palette/material transformation: <source recognition bundle -> new hue, surface and light response>
Subject: <new identity or explicitly pure landscape>
Style/medium: <preserved broad category, newly interpreted>
Composition/framing: exact <ratio>; <new camera and hierarchy>
Lighting/mood: <reference-consistent natural, flash, colored, or designed light>
Color palette: <bold, controlled palette with saturated focal color and clear hue/value contrast; identify dominant, supporting, and accent colors>
Physical realism: <support, gravity, contact, force, material response, expression>
Real-world plausibility: <species/habitat or subject/setting compatibility; behavior; scale; perspective; light sources; shadows/reflections; object function; cause and visible consequence>
Environmental causality: <source, direction, boundary, transition, consequence, dissipation; spatial zones agree>
Prop/function logic: <why each prominent prop is present, how it works, and how it supports the composition>
Originality constraints: <major axes changed; recognizable elements prohibited>
Perceptual transformation: <valued effect; original cause -> new cause; dominant bundles changed across subject/environment/mechanism/relationships; visible evidence; explicit locks>
Recognition anchors to break: <dominant anchor bundle that must not survive>
Preservation lock: <for an accepted-image edit only; successful axes that must remain unchanged>
Quality constraints: <cleanliness and exposure requirements without unwanted flattening, low-poly simplification, or plastic smoothing>
Constraints: retain the style fingerprint; do not convert the result into generic premium editorial or serene human-interest imagery; no typography, logos, watermark, or unrequested people
Avoid: <reference-specific copied elements plus known visual dislikes>
```

Label every image role explicitly. Use the built-in image generation tool by default. Include only the smallest number of recent images needed to pass every reference.

### 7. Generate and inspect

Inspect the actual output rather than trusting the prompt. Repeat Step 3a on the rendered image: inspect the subject alone, the environment without the subject, and the whole relationship graph. Reject any surviving dominant unlocked bundle, even if other changes succeeded. Check:

- category and aspect ratio;
- style-fingerprint fidelity and adaptive originality distance as separate judgments from visual quality;
- dominant recognition anchors and the full relational signature, not only the number of changed axes;
- subject continuity and absence of unjustified age, gender, ethnicity, or attitude drift;
- actual person-to-environment scale and face identifiability against the standing preference, without crude censoring, mandatory rear views, or demographic substitution;
- replacement of the literal identity, objects, and any selected setting axes;
- creative, weird, playful, or scenic strength at the reference's intensity level;
- concept breadth and whether the selected idea is more than a subject or pose moved to a new backdrop;
- preserved aesthetic payoff: luminosity, intimacy, charm, texture, subject scale, palette, openness, or another reference-led attraction;
- physical causality;
- scene-level continuity across fluid, wave, weather, fire, smoke, lighting, reflection, and aftermath zones;
- prominent-prop necessity, function, material fit, and compositional contribution;
- composition and information density: meaningful layers, color hierarchy and visible tension without decorative clutter or purposeless empty space;
- figure necessity, changed palette/material bundle, and mechanism diversity across recent outputs;
- exposure, texture, palette, and AI artifacts;
- compliance with the feedback ledger and meaningful variation from recent outputs;
- portrait facial specificity and human irregularity, when a face is present;
- intentional photographic authorship rather than gray, flat, casual snapshot composition;
- absence of text and branding.

Use `references/validation-checklist.md`. Reject a technically polished result if it has become a generic portrait, generic human-interest image, generic landscape, or unrelated aesthetic. If any critical check fails, regenerate with one targeted correction while restating all invariants.

Run a three-gate acceptance decision:

1. **Originality gate:** Does the result have a distinct dominant relationship and arrangement at thumbnail scale?
2. **Desirability gate:** Is the concept genuinely compelling and aesthetically successful on the reference's terms—not merely normal, arbitrary, or ugly?
3. **Execution gate:** Is it physically coherent, feedback-compliant, readable, and artifact-free?

All three gates must pass. Never let novelty excuse weak aesthetics or let beauty excuse failed originality. Unless explicitly overridden, the desirability gate also fails when the rendered image lacks immediate visual impact, strong color presence, or clear contrast at thumbnail scale. The execution gate fails whenever the actual output violates real-world logic, even if the prompt described correct physics.

When a user rejects an output, identify the single root cause first: concept, recognition-anchor bundle, relational similarity, physical topology, prop design, palette system, exposure, camera relation, subject visibility, face rendering, or finish. Redesign that cause. If the same failure repeats, change the scene design or medium strategy; do not merely intensify adjectives such as `brighter`, `more realistic`, or `less AI`.

### 8. Report briefly

State:

- the style fingerprint retained;
- the major dimensions changed;
- the requested ratio and no-text status;
- any requested subject-visibility treatment and how it was achieved without demographic substitution;
- the generation mode and saved path only when the asset is workspace-bound.

Do not justify weak similarities as inspiration. If the output remains too close, visually weak, physically inconsistent, noisy, dark, or aesthetically off-profile, revise it first.
