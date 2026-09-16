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

- Treat an input image as a **reference image**, not an edit target, unless the user explicitly asks to preserve and modify that exact image.
- Treat explicit user criticism as a new invariant for the rest of the conversation. Do not defend, soften, or forget a rejected palette, exposure level, face treatment, composition style, or finish. Treat a suggested trial as provisional until the user accepts it; never convert an unsuccessful experiment into a permanent style rule.
- Treat originality, desirability, and execution as independent hard gates. A beautiful, realistic output still fails when its dominant camera-subject relationship or recognizable arrangement remains too close. A structurally original output fails when it is merely normal, aesthetically weaker than the reference, or poorly executed.
- Design the whole image before polishing any person, animal, or product. Establish the thumbnail read, large-shape rhythm, color distribution, depth, and directional force first; a clearly rendered face cannot rescue a weak overall composition.
- Compare against recent outputs before each generation. Avoid repeating the same dominant hue, lighting recipe, setting family, camera relation, facial archetype, or finish unless the reference or user specifically requires it.
- Consider environments beyond the reference before selecting a concept. Water, beach, forest, interior, or studio context is not automatically invariant; preserve it only when it carries the reference's creative engine or appeal.
- Extract a **style fingerprint** of 3–6 traits. Include the creative mechanism and, when present, an era or subculture signal such as Y2K, early digital, retro game hardware, futuristic toy design, punk collage, camp, absurd humor, or editorial fashion attitude.
- Also extract a **visual-force profile**: camera aggression, spatial compression, motion direction, contrast, saturation, subject scale, material energy, and campaign attitude. Translate these forces through new content instead of restoring style with a color filter, particles, or renamed objects.
- Separate the reference's real appeal from incidental execution. A visible blue cast, darkness, grayness, phone-camera look, or generic polish is not automatically part of the style fingerprint.
- Use adaptive originality distance. Change 4–6 major dimensions by default, but do not change a dimension merely to reach a quota. Preserve the traits that explain why the reference is appealing.
- Preserve the broad category by default: landscape stays landscape, animal imagery stays animal-led, portrait stays portrait-led, collage stays collage, and conceptual illustration stays conceptual illustration. Treat this as a default, not an override of explicit iterative feedback: if the user rejects the category-defining subject or relationship and accepts a category-shifted solution, update the category constraint accordingly.
- Do not add people to a landscape reference unless requested. Content richness does not require a human subject.
- Preserve visible human life stage, presentation, fashion attitude, and energy unless the user requests a demographic change. Change identity without using age, gender, or ethnicity as an originality shortcut. Never default to an older person merely to create distance. If age is unclear, use an age-neutral adult consistent with the reference.
- Treat **human-subject design** as its own desirability gate whenever a person is visually important. Judge silhouette, pose rhythm, body-line clarity, gesture, garment shape, camera distortion, and integration with the scene separately from facial attractiveness, anatomy, and whole-image composition. A valid concept with a realistic person still fails when the figure looks cramped, clumsy, bulky without purpose, weakly posed, or aesthetically disconnected.
- Treat **human prominence** and **wardrobe design** as two additional gates, not as consequences of adding a person. In non-portrait imagery, do not make a person the largest, nearest, brightest, or highest-contrast element merely to communicate action. Let the mechanism, environment, path, or material response carry the primary thumbnail read unless a human-led composition is reference-critical or explicitly requested.
- Do not improvise wardrobe from generic prompt shorthand such as `color-blocked technical outfit`, `futuristic suit`, or `stylish sportswear`. Build a coherent wardrobe system from the reference-aligned era, attitude, function, silhouette, layering, fit, material, and restrained palette. A technically plausible outfit still fails when it looks costume-like, randomly color-blocked, cheaply athletic, or aesthetically disconnected from the world.
- Never use a demographic swap, sexualization, flowing hair, a conventionally attractive face, or generic fashion-model styling as a substitute for good human-subject design. Create appeal through reference-aligned energy, coherent proportions, expressive posture, clean limb separation, purposeful clothing, and a camera relation that flatters the action without falsifying anatomy.
- Separate **subject continuity** from **subject visibility**. Preserving life stage, presentation, and attitude does not require preserving a clear face, face-dominant scale, gaze, or identifiability.
- When a user dislikes how clearly an otherwise successful subject is shown, interpret that first as a visibility or prominence request, not permission to infer a preferred ethnicity, age, gender, body type, or beauty standard.
- Check recent outputs in the same conversation. Do not repeatedly choose the same demographic profile without a reference-based or user-specified reason.
- Preserve the reference's emotional intensity, humor, strangeness, playfulness, and visual-tension level without copying its literal symbols.
- Do not sanitize a weird, Y2K, retro-futurist, game-like, camp, rebellious, or deliberately awkward reference into generic premium editorial, serene human-interest photography, or tasteful minimalism.
- Treat scene-level causality as a hard constraint. Attractive color or composition does not excuse contradictory wave propagation, fluid behavior, smoke, fire, wind, support, reflection, or aftermath.
- Treat a copied relationship graph as copying even when the individual objects have been renamed or recolored. Change the action chain, support system, spatial grammar, or object ecology when a recognizable motif bundle remains.
- Require every prominent co-subject to participate in one causal or compositional system. If a person merely stands beside an oversized object, or two focal elements can be separated without changing the idea, redesign the interaction or remove the weaker element.
- Do not confuse originality with ugliness or with arbitrary spectacle. Reject a concept whose novelty depends on harsh industrial clutter, oppressive scale, poor subject visibility, muddy light, or an oversized generic prop unless those qualities are reference-led and intentional.
- Do not use giant replacement objects, demographic swaps, or surreal scale as default originality shortcuts. Unusual scale must create beauty, tension, function, and a coherent relationship—not novelty alone.
- Treat cleanliness as removal of accidental noise, not as a mandate for low-poly geometry, large flat color blocks, plastic smoothing, textureless surfaces, or simplified CGI.
- Render no text, letters, numbers, logos, labels, signs, or watermark unless the user explicitly requests exact text.
- Honor the requested aspect ratio exactly in both planning and the generation prompt.

## Workflow

### 0. Capture feedback and recent-output drift

Before planning, write a compact internal ledger:

- **Rejected:** the user's explicit dislikes and the visible failures behind them;
- **Keep:** the qualities the user still wants;
- **Experiment:** suggestions to try once without treating them as permanent constraints;
- **Vary:** palette, exposure, camera relation, setting, subject treatment, visibility, or finish that recent outputs have overused;
- **Edit lock:** for a narrowly corrected accepted image, the scene, composition, palette, lighting, physics, and other successful axes that must remain stable.

Classify feedback by intent, not merely by wording. A direct rejection is binding. A positive observation can strengthen `Keep`. A speculative phrase such as `try`, `maybe`, or `this might help` belongs in `Experiment` unless the user explicitly makes it a requirement. If the user dislikes the experiment, remove it completely from later prompts.

Treat a partially accepted output as evidence about transferable properties—such as saturation, perspective, subject salience, interaction clarity, or overall rhythm—not as a new literal template. Do not repeatedly reuse its exact animal, corridor, object, palette, or mechanism unless the user asks for continuity.

When feedback follows a failed generation, return to the original reference by default. Do not use the rejected output as the next reference unless the user asks to edit that exact result. Change the root scene or lighting decision that caused the failure instead of appending a longer negative-prompt list.

Treat `ugly`, `ordinary`, `disconnected`, `wrong overall`, or `opposite style` as root-level diagnoses when they describe the concept rather than one local detail. Do not rescue a rejected root concept with recoloring, more particles, new clothing, or another decorative effect. Rebuild from the original reference with a different mechanism and scene family.

When the user says the **person** lacks beauty or appeal while accepting the surrounding concept, classify the failure before regenerating: `silhouette`, `pose phase`, `body-line rhythm`, `gesture`, `garment design`, `camera distortion/overlap`, `face rendering`, or `subject-to-scene integration`. Do not interpret this feedback as permission to change demographics or merely make the face more conventionally attractive.

When repeated feedback says that people dominate the image and their clothing lacks taste, classify the joint root cause as `subject salience + wardrobe system`. Rebuild the composition so the environment, mechanism, or action trace leads; recast people as active participants or secondary anchors; then redesign the entire outfit logic. Do not keep a foreground hero and merely swap colors, jackets, or pants.

When the user explicitly accepts the concept and attaches or names the generated image while requesting one narrow correction, treat that image as the edit target. Use a preservation lock and change only the criticized axis.

When the user accepts the composition but says the style is wrong, preserve the accepted spatial structure and change structural style carriers—camera relation, contrast, saturation, directional light, motion behavior, material response, and spatial compression. Do not merely apply a warm/cool grade or scatter motion effects over the scene.

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
- the visual-force profile: camera aggression, spatial compression, directionality, saturation, contrast, scale, material energy, and ad/editorial attitude;
- the subject's intended salience role: hero, active participant, secondary anchor, scale cue, or absent;
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

Add a force statement: `Carry <camera energy, direction, contrast, saturation, scale tension, material response>; realize them through <new mechanism and content>.` This prevents both literal copying and stylistic drift into an attractive but opposite image.

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

Require a change to the **environment skeleton** when the setting itself is central to recognition or when stronger reconstruction is requested. Do not force a cross-ecosystem change when it would erase the reference's appeal.

Avoid exact pose, silhouette, focal placement, object cluster, path shape, crop, palette mapping, signature character, branding, or recognizable arrangement from the reference.

Also compare the reference and proposed concept as a relationship graph: `actor -> action -> object -> support surface -> surrounding props`. If that graph is still recognizable, change at least two structural relations rather than relying on cosmetic substitutions.

For proposals with multiple prominent elements, write an interaction graph: `driver -> affected element -> visible response -> consequence`. Reject a passive adjacency graph such as `person beside giant object` unless the disconnection is the intentional joke and is aesthetically strong.

Axis count is supporting evidence, not a pass condition. Identify the 1–3 **dominant recognition anchors** first, such as face-filling scale, lens relation, signature pose, prop-face pairing, silhouette, or environment enclosure. If a dominant anchor or anchor bundle survives, reject the concept even when four or more lower-weight axes changed.

Write both relational signatures before generation:

`reference: actor -> action -> focal object -> support -> surroundings -> camera relation`

`proposal: actor -> action -> focal object -> support -> surroundings -> camera relation`

If both sentences still describe the same image at a glance, redesign the camera relation, action consequence, support system, or spatial grammar.

### 4. Design the new concept

Before choosing, generate 3–5 compact internal candidates that differ in structural premise, not only nouns. When the reference environment is incidental, span at least three setting families, such as natural, constructed, domestic, aerial, subterranean, ceremonial, or surreal. Include at least one cross-environment candidate and compare each candidate with both the reference and recent outputs.

For each candidate, record:

- the new relational signature and environment skeleton;
- the creative mechanism or causal event;
- the reference appeal it preserves;
- the visual-force profile it carries forward;
- the whole-image thumbnail read and large-shape hierarchy;
- each subject's salience role and interaction with the rest of the scene;
- for every hero or active human, the subject-design read: silhouette, action phase, line of force, limb separation, garment shape, and camera-flattering angle;
- the main originality risk;
- the main aesthetic risk.

Choose the candidate that best balances structural distance, reference fidelity, visual appeal, and generative feasibility. Do not choose the strangest candidate by default. Reject a mere location swap—such as the same portrait or action transplanted into an impressive place—when it lacks a new relationship, consequence, or visual rule.

Apply a **whole-image-first gate** before selecting a candidate. Mentally remove any face, figure, animal, or product: the remaining composition should still have intentional shape rhythm, color relationships, depth, and direction. Then restore only subjects that strengthen the system. Do not add a tiny person merely as a scale marker when the image is more harmonious without one.

Apply an **interaction-and-scale gate**. Every hero-scale element must either drive, resist, transform, support, or reveal another important element. Reject giant-object spectacle, passive bystanders, and disconnected focal pairs whose relationship is only proximity.

Write a one-sentence concept before prompting. It must specify:

- what is new;
- which creative engine, style-era signal, and attitude remain;
- why the result is visually compelling;
- how it differs structurally from the reference.

For concept-driven references, retain an equivalent level of joke, contradiction, transformation, awkwardness, unusual scale, or directional force. Reject concepts that reduce a playful or eccentric reference to a conventional portrait. For calm landscapes, create discovery and layered rhythm rather than forcing in people or artificial drama.

Apply a **not-merely-normal gate**. The concept must contain at least one meaningful mechanism appropriate to the source: interaction, contradiction, transformation, directional force, discovery, causal event, or unusual spatial rule. Do not force surrealism or melodrama when a quieter visual mechanism would preserve the reference better.

Apply an **appeal-preservation gate**. Name what made the reference attractive—such as luminosity, intimacy, subject scale, facial charm, softness, palette elegance, tactile medium, playfulness, or scenic openness—and carry an equivalent quality into the new setting. Cross-environment imagination should expand the world without sacrificing the image's emotional and aesthetic payoff.

For photographic references, name the intentional photographic decision: decisive light, camera relation, foreground anchor, motion behavior, spatial compression, or another clear point of view. Reject concepts whose only claim to realism is that they resemble a casual phone snapshot.

### 4a. Control subject prominence and visibility without demographic substitution

Choose the subject role before describing appearance: `hero`, `active participant`, `secondary anchor`, `scale cue`, or `absent`. Match framing and face visibility to that role. When the user prioritizes the overall image, default to secondary, scale-cue, or absent treatment unless the reference category requires a human-led result.

For non-portrait conceptual, action, scenic, product, or animal-led images, default to `active participant`, `secondary anchor`, or `absent`, not `hero`. Avoid near-lens bodies, foreground backs, large torsos, or high-contrast clothing that accidentally consume the frame. A person may remain causally essential while the image's primary read belongs to the trajectory, environment, interacting objects, or natural event.

When the user wants the person less clearly shown while keeping the concept:

- preserve the accepted action, palette, environment, lighting, realism, and compositional energy unless the requested visibility change requires a local adjustment;
- reduce identifiability through a physically motivated side/back angle, smaller face scale, hair, gesture, crop, shadow, reflection, refraction, foreground overlap, or a concept-relevant prop;
- keep the person expressive through posture, action, clothing, color, and force response rather than relying on a readable face;
- prefer designed occlusion over censor bars, mosaic pixelation, arbitrary blur, masks, or face replacement unless the user explicitly requests one;
- do not translate `not my type` into an assumed demographic preference. Ask only if the user actually wants a different appearance rather than lower visibility.
- avoid camera instructions that accidentally make the face dominant, such as running toward camera, frontal close perspective, centered eye contact, or face-led lighting;
- if a small anonymous figure still disrupts the color rhythm, scale hierarchy, or emotional tone, remove it rather than repeatedly restyling its clothes or face.

For a narrow edit of an accepted image, use the supplied generated image as the edit target and state invariants explicitly: `change only face presentation; keep scene, framing, pose, clothing, palette, light, materials, shadows, and physics unchanged.` Make the correction visibly meaningful without letting the whole image drift.

### 4b. Design human subjects for aesthetic coherence

When a person is a hero or active participant, write a compact **body-line plan** before prompting:

`action phase -> head/neck/torso line -> weight-bearing limb -> counterbalancing limbs -> negative spaces -> garment silhouette -> camera effect`

Also write a compact **wardrobe plan** before naming garment pieces:

`reference-aligned attitude/era -> silhouette family -> layering and fit -> functional needs -> material response -> one dominant garment color + neutrals + optional accent -> accessories/gear`

- Choose a decisive action phase that shows both force and grace. Avoid transitional instants that collapse the torso, stack limbs into one mass, hide the support path, or create an accidental squat unless that compression is essential and visually strong.
- Build one dominant line of action plus one or two supporting counter-lines. Keep readable negative spaces between arms, torso, and legs where the action permits; prevent tangencies that make limbs merge with the body, equipment, or background.
- Preserve plausible proportions while checking the projected silhouette at the chosen lens and angle. Foreshortening may be energetic, but it must not enlarge hands, feet, shoulders, hips, or the head into an awkward visual hierarchy.
- Treat clothing as shape design as well as function. Use fit, volume, seams, material response, and color blocking to clarify the pose and attitude. Avoid generic bulky sportswear, arbitrary armor, featureless bodysuits, or decorative styling that obscures the body mechanics.
- Design one coherent look, not a list of individually vivid garments. Unless the reference supports maximalism, use one dominant garment color, one or two neutrals, and at most one controlled accent; let cut, proportion, layering, and material create interest. Do not assign a different saturated color to every jacket, trouser leg, panel, helmet, and prop.
- Preserve the reference's fashion attitude without copying its literal outfit. Choose a recognizable silhouette family—such as understated athletic separates, relaxed outdoor layers, tailored streetwear, or practical workwear—and keep every piece within that system. Reject novelty sportswear, cropped technical jackets, loud contrast panels, tight superhero-like suits, mismatched primary colors, or bulky safety gear when they are not reference-led.
- Integrate necessary protective or technical equipment with low visual weight. Helmets, harnesses, pads, and fasteners should be coherent in shape and finish, should not dominate the body, and should not make the subject look like a generic commercial-sports mannequin.
- Apply a standalone wardrobe desirability test: imagine the person paused outside the action. The outfit should still look intentional, flattering to the body line, culturally and era coherent, and appropriate to the world. If it reads as costume, rental gear, random AI styling, or cheap campaign wardrobe, redesign it before generation.
- Use face, hair, and styling only in support of the body-line plan. A flowing hairstyle, exposed profile, or attractive face cannot rescue a cramped pose or incoherent silhouette.
- Keep the subject aesthetically integrated with the scene through shared direction, light, palette, and material response. The person should not look pasted in, photographed from a mismatched lens, or styled for a different visual world.
- Evaluate subject appeal at both thumbnail and full view. At thumbnail scale the silhouette and gesture must read; at full view anatomy, hands, face fragments, clothing construction, and equipment attachment must remain credible.

For dynamic natural or material scenes, write a compact causality map before prompting:

`source/driver -> propagation direction -> boundary or interaction -> visible transition -> downstream effect -> dissipation/aftermath`

Map the relevant zones in the image. For example, a reef break should distinguish deep-water swell, shoaling or breaking line, shoreward whitewater/turbulence, and eventual calming; a poured liquid should preserve source composition, stream continuity, impact behavior, pooling, and drainage. If the concept cannot explain a sharp calm/rough, dry/wet, lit/shadowed, or solid/fluid boundary, redesign it.

### 5. Apply the default visual profile

Use the defaults in `references/visual-quality.md`, but let intentional reference style override taste defaults. In particular:

- preserve intentional Y2K color, retro-digital texture, futuristic lighting, flash photography, chromatic contrast, or awkward styling when those are part of the style fingerprint;
- use rich layers and meaningful visual anchors without micro-clutter;
- judge the thumbnail before local detail: large and medium shapes, color blocks, directional lines, and depth must work even when faces and textures are unreadable;
- distinguish intentional era texture and synthetic material language from accidental noise, plastic artifacts, HDR, or incoherent glow;
- choose scenes and materials that can satisfy these constraints instead of merely listing negative words.
- prevent cross-output palette collapse: do not repeatedly cover the sky, environment, clothing, and shadows with the same hue;
- keep faces human rather than idealized: choose light and camera distance that support natural proportions, skin texture, asymmetry, hairline detail, and readable eyes;
- distinguish natural photography from flat documentation. When the reference or feedback calls for a stronger image, create authorship through light, framing, depth, or a natural event rather than through saturation, HDR, or beauty retouching.
- treat clear color separation as a compositional tool. Do not use grayness, beige/khaki veils, or low saturation as automatic sophistication; when vivid energy is reference-led, use clean local color, neutral highlights, chromatic shadows, and controlled accents without muddying the frame.
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
Visual-force profile: <camera aggression, compression, direction, contrast, saturation, scale tension, material energy>
Reference appeal to retain: <luminosity, intimacy, charm, texture, subject scale, palette energy, or other real attraction>
Primary request: <new one-sentence concept>
Concept mechanism: <interaction, contradiction, transformation, force, discovery, causal event, or spatial rule that prevents a mere location swap>
Whole-image hierarchy: <thumbnail read, dominant large/medium shapes, color distribution, depth, directional path>
Scene/backdrop: <new or reconstructed setting at the selected originality distance>
Subject continuity: <reference-aligned life stage, presentation, energy, or explicitly pure landscape; no unjustified demographic shift>
Subject role/salience: <hero, participant, secondary anchor, scale cue, or absent; relative prominence>
Subject visibility: <clear, incidental, partially obscured, anonymous, back/side view; physically motivated method>
Subject: <new identity or explicitly pure landscape>
Human-subject design: <for a hero/active person: decisive action phase, dominant body line, counterbalance, limb separation, negative spaces, garment silhouette, camera-flattering perspective; no demographic or beauty-template shortcut>
Wardrobe design: <reference-aligned attitude and era; coherent silhouette family, layering, fit, material, restrained palette, integrated gear; prohibit random technical color blocking or costume-like sportswear>
Style/medium: <preserved broad category, newly interpreted>
Composition/framing: exact <ratio>; <new camera and hierarchy>
Lighting/mood: <reference-consistent natural, flash, colored, or designed light>
Color palette: <controlled palette>
Physical realism: <support, gravity, contact, force, material response, expression>
Interaction graph: <driver -> affected element -> visible response -> consequence; explain why each focal element belongs>
Environmental causality: <source, direction, boundary, transition, consequence, dissipation; spatial zones agree>
Prop/function logic: <why each prominent prop is present, how it works, and how it supports the composition>
Originality constraints: <major axes changed; recognizable elements prohibited>
Recognition anchors to break: <dominant anchor bundle that must not survive>
Preservation lock: <for an accepted-image edit only; successful axes that must remain unchanged>
Quality constraints: <cleanliness and exposure requirements without unwanted flattening, low-poly simplification, or plastic smoothing>
Constraints: retain the style fingerprint; do not convert the result into generic premium editorial or serene human-interest imagery; no typography, logos, watermark, or unrequested people
Avoid: <reference-specific copied elements plus known visual dislikes>
```

Label every image role explicitly. Use the built-in image generation tool by default. Include only the smallest number of recent images needed to pass every reference.

### 7. Generate and inspect

Inspect the actual output rather than trusting the prompt. Check:

- category and aspect ratio;
- whole-image thumbnail strength before subject beauty or local detail;
- style-fingerprint fidelity and adaptive originality distance as separate judgments from visual quality;
- visual-force fidelity without copied nouns, palette mapping, particle overlays, or literal motion effects;
- dominant recognition anchors and the full relational signature, not only the number of changed axes;
- subject continuity and absence of unjustified age, gender, ethnicity, or attitude drift;
- requested subject visibility, face prominence, and identifiability without crude censoring or demographic substitution;
- subject role and salience: no accidental face dominance, passive bystander, unnecessary scale figure, or disconnected co-subject;
- human prominence: in non-portrait imagery, no near-lens body, oversized torso, saturated outfit, or foreground placement has displaced the mechanism, environment, action path, or overall composition as the intended primary read;
- human-subject desirability when a person is prominent: elegant and reference-aligned silhouette, decisive pose phase, coherent line of action, clean limb separation, purposeful garment shape, flattering but physically honest camera relation, and integration with scene forces;
- wardrobe desirability: every visible outfit forms one coherent, reference-aligned styling system with intentional silhouette, fit, layering, material, restrained color relationships, and integrated equipment; no random high-saturation separates, generic technical sportswear, costume logic, or featureless bodysuit;
- absence of demographic, sexualization, hairstyle, or generic-model shortcuts used to disguise weak pose or silhouette design;
- replacement of the literal identity, objects, and any selected setting axes;
- creative, weird, playful, or scenic strength at the reference's intensity level;
- concept breadth and whether the selected idea is more than a subject or pose moved to a new backdrop;
- preserved aesthetic payoff: luminosity, intimacy, charm, texture, subject scale, palette, openness, or another reference-led attraction;
- physical causality;
- scene-level continuity across fluid, wave, weather, fire, smoke, lighting, reflection, and aftermath zones;
- prominent-prop necessity, function, material fit, and compositional contribution;
- interaction coherence and whether every focal element participates in the same causal/compositional system;
- composition and information density;
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

All three gates must pass. Never let novelty excuse weak aesthetics or let beauty excuse failed originality.

When a user rejects an output, identify the single root cause first: concept, recognition-anchor bundle, relational similarity, physical topology, prop design, interaction failure, palette system, exposure, camera relation, subject salience, human-subject design, face rendering, or finish. Redesign that cause. If the criticism is root-level or the same failure repeats, abandon the scene family or medium strategy; do not merely intensify adjectives, recolor the scene, add particles, swap clothing, change demographics, or introduce a giant replacement object.

### 8. Report briefly

State:

- the style fingerprint retained;
- the major dimensions changed;
- the requested ratio and no-text status;
- any requested subject-visibility treatment and how it was achieved without demographic substitution;
- the generation mode and saved path only when the asset is workspace-bound.

Do not justify weak similarities as inspiration. If the output remains too close, visually weak, physically inconsistent, noisy, dark, or aesthetically off-profile, revise it first.
