# Reimagine Reference Images

An AI skill for reimagining reference images while preserving their style and creative appeal.

Turn a visual reference into a fresh concept with new subjects, interactions, and compositions. The skill helps an image-capable agent identify what makes a reference compelling—its humor, visual energy, material language, or sense of discovery—and carry those qualities into a different image.

Built for Codex, this repository contains a creative workflow, prompting guidance, and visual review checklists. Image generation is handled by the tools available in your environment.

## What it does

- **Finds the creative idea behind the reference.** Identifies the style, mood, and visual relationships worth preserving.
- **Rebuilds recognizable content and composition.** Goes beyond changing colors or swapping objects by reconsidering the action, setting, viewpoint, and arrangement.
- **Balances originality with visual appeal.** Reviews the concept, composition, and physical coherence separately, so novelty alone does not determine success.
- **Carries feedback through revisions.** Tracks what you want to keep, what you reject, and what you only want to try.

For example, a playful image of a miniature character navigating oversized everyday objects might inspire a new scene with a different activity, environment, and camera angle. The sense of scale and playful discovery can remain while the visual story changes.

## Use cases

| Use case | How the skill helps |
| --- | --- |
| Campaign and editorial concept exploration | Develop new visual stories that retain a reference's energy and attitude. |
| Y2K, retro-futurist, and playful imagery | Preserve an era's materials, humor, and visual character while redesigning the scene. |
| Landscapes and animal imagery | Explore new environments and interactions while retaining scenic appeal or behavioral interest. |
| Portraits and fashion concepts | Rethink staging, pose, wardrobe, and composition while preserving the intended mood. |
| Illustration and collage | Translate shape rhythm, layering, and conceptual tension into a new arrangement. |
| Iterative art direction | Refine color, lighting, subject prominence, or other details while preserving accepted choices. |

## Requirements

- A Codex environment that can inspect reference images and generate or edit images.
- An installed `imagegen` skill, which this skill uses for generation and editing instructions. It is not included in this repository.
- At least one reference image, attached to the conversation or accessible as a local file.

Installing this repository adds the workflow instructions; it does not install an image model or enable image-generation access. Output quality and supported image dimensions depend on the available generation tool.

## Installation

For a personal installation on macOS or Linux, clone this repository into your user skills directory:

```sh
mkdir -p ~/.agents/skills
git clone https://github.com/weniswen/reimagine-reference-images.git \
  ~/.agents/skills/reimagine-reference-images
```

Alternatively, download the repository and place its contents in a folder named `reimagine-reference-images` under `~/.agents/skills/`. Keep `SKILL.md`, `agents/`, and `references/` together.

For a project-specific installation, use `.agents/skills/reimagine-reference-images/` inside that project instead. See the [official Codex skills documentation](https://learn.chatgpt.com/docs/build-skills) for supported skill locations and setup details.

## How to use

### 1. Add a reference image

Attach an image or provide its local file path. Tell Codex what you like about it and any requirements for the new image, such as aspect ratio, subject matter, or intended use.

### 2. Invoke the skill

Start with a simple request:

```text
Use $reimagine-reference-images to create a new image inspired by the
attached reference. Keep its playful mood and visual energy, but
reimagine the subject, setting, and composition. Use a 16:9 aspect
ratio and include no text.
```

For more control, specify what should stay and what should change:

```text
Use $reimagine-reference-images with the attached reference.

Purpose: an editorial illustration.
Keep: the Y2K attitude, tactile materials, and absurd humor.
Change: the main subject, its interaction with the environment,
and the camera angle.
Avoid: the original prop arrangement and recognizable silhouette.
Format: 4:5, with no text or logos.
```

You do not need to write a detailed generation prompt. The skill guides the agent through reference analysis, concept selection, prompting, generation, and visual review.

### 3. Refine the result

Give concrete feedback about what works and what needs to change:

```text
Keep the color palette and sense of motion. The person dominates
the frame too much. Make the environment the main visual focus
and keep the person as a smaller, active participant.
```

When you like an image and want a narrow edit, attach or identify that result explicitly:

```text
Edit this generated image. Keep the composition, lighting, and
colors. Only reduce how clearly the face is visible, using a
natural side angle or occlusion.
```

By default, the original reference guides a fresh interpretation. Explicitly selecting a generated result for editing tells the agent to preserve its successful elements while making the requested correction.

## How the workflow works

1. **Read the reference:** identify its category, style, visual energy, and central creative idea.
2. **Choose what to preserve:** define a small set of traits that explain its appeal.
3. **Design a new concept:** explore different subjects, relationships, environments, and compositions.
4. **Generate and review:** assess structural difference, aesthetic appeal, and execution quality.
5. **Revise with feedback:** address the cause of a weak result and retain accepted decisions.

The default workflow preserves the broad image category, avoids adding people to landscapes, and omits text and logos unless requested. You can override these defaults in your prompt.

## Repository guide

| File | Purpose |
| --- | --- |
| [SKILL.md](SKILL.md) | Core instructions and the complete creative workflow. |
| [agents/openai.yaml](agents/openai.yaml) | Display name and default invocation prompt. |
| [references/originality-playbook.md](references/originality-playbook.md) | Guidance for transforming concepts and recognizable relationships. |
| [references/visual-quality.md](references/visual-quality.md) | Aesthetic defaults, composition guidance, and physical coherence checks. |
| [references/validation-checklist.md](references/validation-checklist.md) | Review criteria for generated images. |
