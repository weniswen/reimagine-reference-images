# 🎨 Reimagine Reference Images

*Last updated: September 21, 2026*

An AI skill for turning reference images into fresh visual concepts. It draws inspiration from their style, camera angles, lens characteristics, color relationships, lighting, and composition, then reinterprets those qualities through new subjects, settings, and visual stories.

Start with an image that catches your eye. The workflow helps identify what makes it compelling and turns that inspiration into a new creative direction, with guidance for generating images and refining the results.

Use it for content creation, creative exploration, marketing visuals, wallpapers, and everyday image needs. Whether you are planning a campaign or looking for your next visual idea, a reference image gives you a starting point.

## ✨ What it does

- **Finds the creative idea behind the reference.** Identifies the style, mood, and visual relationships worth preserving.
- **Rebuilds recognizable content and composition.** Checks subject appearance, environment, visual effects, and relationships independently, including distinctive combinations of color, material, and subject.
- **Balances originality with visual appeal.** Reviews the concept, composition, and physical coherence separately, so novelty alone does not determine success.
- **Carries feedback through revisions.** Tracks what you want to keep, what you reject, and what you only want to try.

For example, a playful image of a miniature character navigating oversized everyday objects might inspire a new scene with a different activity, environment, and camera angle. The sense of scale and playful discovery can remain while the visual story changes.

## 🖼️ Examples

Each pair shows the reference preview on the left and the reimagined result on the right. The goal is to carry forward the reference's visual appeal while rebuilding its subject, action, environment, and recognizable arrangement.

### Storybook watercolor

| Reference | Reimagined result |
| --- | --- |
| <img src="examples/storybook-watercolor-reference.png" alt="Reference: cozy illustrated domestic scene" height="200"> | <img src="examples/storybook-watercolor-result.png" alt="Result: mother goose pulling goslings through a spring garden" height="200"> |

### Macro nature photography

| Reference | Reimagined result |
| --- | --- |
| <img src="examples/macro-nature-reference.png" alt="Reference: close-up of dew-covered grass" height="200"> | <img src="examples/macro-nature-result.png" alt="Result: glass frog leaping between wet red leaves" height="200"> |

### Group motion in nature

| Reference | Reimagined result |
| --- | --- |
| <img src="examples/underwater-motion-reference.png" alt="Reference: flock of pink birds in flight" height="200"> | <img src="examples/underwater-motion-result.png" alt="Result: sea lions swimming through a kelp forest" height="200"> |

### Playful animal action

| Reference | Reimagined result |
| --- | --- |
| <img src="examples/playful-animals-reference.png" alt="Reference: lively animal scene in a colorful interior" height="200"> | <img src="examples/playful-animals-result.png" alt="Result: two fox cubs having a pillow fight in a retro motel room" height="200"> |

See the [example gallery](examples/README.md) for a short explanation of what each reimagining preserves and changes.

## 💡 Application scenarios

| Who it's for | What you can create |
| --- | --- |
| Marketers and social media managers | Campaign visuals, promotional backgrounds, and social post imagery inspired by a chosen mood or aesthetic. |
| Content creators and bloggers | Article covers, video thumbnail artwork, and illustrations that give a topic a distinctive visual direction. |
| Anyone personalizing their screens | Phone and desktop wallpapers built around favorite colors, atmospheres, or visual themes. |
| Designers and creative teams | Visual explorations and concept images to develop an idea before committing to a direction. |
| Small business owners | Seasonal visuals, website banners, and imagery for brand storytelling. |
| Educators and presenters | Conceptual illustrations and presentation backgrounds that help communicate an idea. |
| Hobbyists and visual explorers | New scenes, imaginative worlds, and personal artwork when inspiration is running low. |

The skill focuses on image artwork. Add final headlines, captions, and layout elements in your preferred design tool, or explicitly request text when generating.

## 🧰 Compatibility and requirements

The creative workflow can be adapted to agents that support the [Agent Skills format](https://agentskills.io/home), including [Claude Code](https://code.claude.com/docs/en/skills). Format support alone does not provide image-generation capabilities.

**The current integration targets Codex.** `SKILL.md` refers to the installed `imagegen` skill and a built-in image-generation tool; `agents/openai.yaml` supplies Codex interface metadata. Other agents require equivalent image tools and adaptations to those tool-specific instructions. End-to-end generation in other agents has not been verified for this repository.

To run the full workflow, you need:

- An agent that can read the skill and its reference files, inspect input images, and review generated results.
- An image-generation/editing tool connected to that agent. For the current Codex integration, the `imagegen` skill must also be available; it is not included here.
- At least one reference image, attached to the conversation or accessible as a local file.

Installing this repository adds workflow instructions; it does not install an image model or enable image-generation access. Output quality and supported image dimensions depend on the connected tool.

## 📦 Installation

### Codex

For a personal installation on macOS or Linux, clone this repository into your user skills directory:

```sh
mkdir -p ~/.agents/skills
git clone https://github.com/weniswen/reimagine-reference-images.git \
  ~/.agents/skills/reimagine-reference-images
```

Alternatively, download the repository and place its contents in a folder named `reimagine-reference-images` under `~/.agents/skills/`. Keep `SKILL.md`, `agents/`, and `references/` together.

For a project-specific installation, use `.agents/skills/reimagine-reference-images/` inside that project instead. See the [official Codex skills documentation](https://learn.chatgpt.com/docs/build-skills) for supported skill locations and setup details.

### Other agents

Place the skill folder in the location supported by your agent and keep `SKILL.md` and `references/` together. Adapt the `imagegen` dependency and built-in generation instructions to your agent's actual image tools before running the full workflow. Use that agent's own skill invocation syntax; the examples below use Codex's `$reimagine-reference-images` syntax.

## 🚀 How to use

### 1. Add a reference image

Attach an image or provide its local file path. Tell your agent what you like about it and any requirements for the new image, such as aspect ratio, subject matter, or intended use.

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

## 🔄 How the workflow works

1. **Read the reference:** identify its category, style, visual energy, and central creative idea.
2. **Choose what to preserve:** define a small set of traits that explain its appeal.
3. **Design a new concept:** explore different subjects, relationships, environments, and compositions.
4. **Generate and review:** assess structural difference, aesthetic appeal, and execution quality.
5. **Revise with feedback:** address the cause of a weak result and retain accepted decisions.

The default workflow preserves the broad image category and lets environments and still-life scenes stand on their own, without adding people or animals just to provide scale or story. When people are needed, it favors small, visually subordinate figures with faces that are difficult to identify. Ask explicitly for a close portrait or clear face to override this preference.

Text and logos are omitted unless requested. Providing a reference with only an aspect ratio requests a fresh reimagining in that format; it does not request a crop, resize, or outpaint of the original scene.

## 📂 Repository guide

| File | Purpose |
| --- | --- |
| [SKILL.md](SKILL.md) | Core instructions and the complete creative workflow. |
| [agents/openai.yaml](agents/openai.yaml) | Codex display name and default invocation prompt. |
| [references/originality-playbook.md](references/originality-playbook.md) | Guidance for transforming concepts and recognizable relationships. |
| [references/visual-quality.md](references/visual-quality.md) | Aesthetic defaults, composition guidance, and physical coherence checks. |
| [references/validation-checklist.md](references/validation-checklist.md) | Review criteria for generated images. |
| [examples/](examples/) | Reference-to-result examples from real skill use. |
