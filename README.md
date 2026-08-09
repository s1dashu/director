<h1 align="center">director</h1>

<p align="center">
  <strong>English</strong> · <a href="./README_CN.md">简体中文</a>
</p>

<p align="center">
  <strong>Direct complete videos—from the first idea to production-ready media.</strong>
</p>

<p align="center">
  <img src="./repository-assets/repository-covers/director-cover.png" alt="director — a multi-mode Agent skill for directing and producing videos" width="100%">
</p>

<p align="center">
  <a href="./SKILL.md"><img alt="Agent Skill" src="https://img.shields.io/badge/Agent-Skill-111111"></a>
  <a href="#what-it-can-do-for-you"><img alt="Animated Explainer: production validated" src="https://img.shields.io/badge/Explainer-validated-2EA44F"></a>
  <a href="./LICENSE"><img alt="MIT License" src="https://img.shields.io/badge/license-MIT-2EA44F"></a>
</p>

<p align="center">
  <a href="#what-it-can-do-for-you">Core Capabilities</a> ·
  <a href="#built-in-visual-styles">Visual Styles</a> ·
  <a href="#installation">Installation</a> ·
  <a href="#start-with-a-single-sentence">Get Started</a>
</p>

`director` is an Agent skill for directing and producing complete videos, from the initial idea and script to shot design, media generation, and delivery.

- **Animated Explainer** — Explain concepts, ideas, history, or knowledge through clear narration and animated scenes.

https://github.com/user-attachments/assets/60e7e51f-8d3e-4004-a88d-f80f6f209d4d

- **Storytime Animation** — Turn first-person experiences into animated stories that combine direct-to-camera narration with reenacted moments.

https://github.com/user-attachments/assets/2c78454b-4c2e-42f9-ade9-3fbfb083dc5b

- **Cinematic Drama** — Turn confirmed worldbuilding, characters, and scripts into action-, dialogue-, and conflict-driven AI films, AI motion comics, short dramas, or micro-films.

https://github.com/user-attachments/assets/d7f23943-4fce-4c39-8815-3515fc354f87

- **Visual Journalism** — Cover current affairs, business, industry, and other real-world topics through evidence-led storytelling that combines documentary footage, explanatory animation, maps, charts, and motion graphics.

## What It Can Do for You

- **Choose the right directing grammar.** Match the workflow to the force driving the video: personal experience, concept explanation, real-world evidence, or dramatic action.
- **Make complex ideas easy to follow.** From topic research and editorial decisions to narration structure, it helps you build a line your audience can understand and wants to keep watching.
- **Turn a script into a production-ready directing plan.** It breaks the narrative into workable units, directs shots and performances, and produces generation-ready prompts for the selected Mode.
- **Keep the entire video consistent.** Prompt-defined styles, required character references, and voice anchors reduce character drift, style shifts, and voice inconsistency across clips.
- **Go from idea to editable clips.** Beyond writing, it can continue through reference planning, clip generation, and task tracking, then hand the generated clips to your editor for final assembly and light cleanup.

## Built-in Visual Styles

The Skill manages validated and candidate visual languages by Mode: Animated Explainer has six validated styles plus two candidate hand-drawn styles, Storytime Animation has one dedicated style, Clay Stop-Motion has one candidate handcrafted miniature style, and Cinematic Drama has two candidate styles. Users are not offered unvalidated cross-Mode combinations. A style can become cross-Mode only after it succeeds in real productions across those Modes.

These styles are starting points, not templates. The Skill redesigns the setting, characters, and shots around each new topic. You can also provide a custom textual style for the selected Mode; visual style references are not image assets.

<table>
  <tr>
    <td width="50%" align="center" valign="top">
      <a href="./repository-assets/style-previews/cinematic-3d-animation-nietzsche-16x9-v3.webp"><img src="./repository-assets/style-previews/cinematic-3d-animation-nietzsche-16x9-v3.webp" alt="Cinematic 3D animation preview" height="220"></a><br>
      <b>Cinematic 3D Animation</b><br>
      <sub>Painterly surfaces, restrained color, and story-rich cinematic lighting</sub><br>
      <a href="./modes/animated-explainer/styles/cinematic-3d-animation.md">View style guide</a>
    </td>
    <td width="50%" align="center" valign="top">
      <a href="./repository-assets/style-previews/clay-stop-motion.webp"><img src="./repository-assets/style-previews/clay-stop-motion.webp" alt="Clay stop-motion preview" height="220"></a><br>
      <b>Clay Stop-Motion</b><br>
      <sub>Handmade clay figures, miniature sets, and tactile frame-by-frame motion</sub><br>
      <a href="./modes/clay-stop-motion/styles/handcrafted-clay-fable-stop-motion.md">View style guide</a>
    </td>
  </tr>
  <tr>
    <td width="50%" align="center" valign="top">
      <a href="./repository-assets/style-previews/melancholic-blue-simple-line-animation.webp"><img src="./repository-assets/style-previews/melancholic-blue-simple-line-animation.webp" alt="Melancholic blue line animation preview" height="220"></a><br>
      <b>Melancholic Blue Line Animation</b><br>
      <sub>Cool blue-gray paper, awkward pencil lines, and a quiet introspective mood</sub><br>
      <a href="./modes/animated-explainer/styles/melancholic-blue-simple-line-animation.md">View style guide</a>
    </td>
    <td width="50%" align="center" valign="top">
      <a href="./repository-assets/style-previews/soft-colored-pencil-cute-animation.webp"><img src="./repository-assets/style-previews/soft-colored-pencil-cute-animation.webp" alt="Soft colored-pencil cute animation preview" height="220"></a><br>
      <b>Soft Colored-Pencil Animation</b><br>
      <sub>Gentle outlines, warm paper texture, and an approachable playful tone</sub><br>
      <a href="./modes/animated-explainer/styles/soft-colored-pencil-cute-animation.md">View style guide</a>
    </td>
  </tr>
  <tr>
    <td width="50%" align="center" valign="top">
      <a href="./repository-assets/style-previews/clean-line-crayon-animation.webp"><img src="./repository-assets/style-previews/clean-line-crayon-animation.webp" alt="Clean-line crayon animation preview" height="220"></a><br>
      <b>Clean-Line Crayon Animation</b><br>
      <sub>Bright color blocks, clear hand-drawn lines, and an orderly 2D world</sub><br>
      <a href="./modes/animated-explainer/styles/clean-line-crayon-animation.md">View style guide</a>
    </td>
    <td width="50%" align="center" valign="top">
      <a href="./repository-assets/style-previews/dopamine-cute-3d-animation-16x9-v2.webp"><img src="./repository-assets/style-previews/dopamine-cute-3d-animation-16x9-v2.webp" alt="Dopamine cute 3D animation preview" height="220"></a><br>
      <b>Dopamine Cute 3D Animation</b><br>
      <sub>Bouncy characters, vibrant colors, and energetic layered compositions</sub><br>
      <a href="./modes/animated-explainer/styles/dopamine-cute-3d-animation.md">View style guide</a>
    </td>
  </tr>
</table>

Storytime Animation has its own [Clean White-Character Storytime Animation](./modes/storytime-animation/styles/clean-white-character-storytime-animation.md): rounded white 2D characters, crisp black outlines, limited flat colors, expressive performance, and environments that are more detailed than the cast.

Clay Stop-Motion promotes clay animation from a surface treatment into a dedicated story workflow. Its candidate [Handcrafted Clay Fable Stop-Motion](./modes/clay-stop-motion/styles/handcrafted-clay-fable-stop-motion.md) style combines handmade puppets, material-specific deformation, miniature-set photography, and readable frame-by-frame poses; it still awaits a full sample validation.

Cinematic Drama initially offers two candidate styles: [Semi-Realistic 3D Chinese Animation Film](./modes/cinematic-drama/styles/semi-realistic-3d-chinese-animation-film.md) and [Semi-Realistic Eastern Dark-Fantasy 3D Film](./modes/cinematic-drama/styles/semi-realistic-eastern-dark-fantasy-3d-film.md). Both remain candidates until an end-to-end sample is validated.

## More Than a Look: Reusable Voices

Alongside its Mode-owned prompt-defined styles, the Skill includes multiple standardized Chinese and English voices.

You can use one of these voices directly, or create a dedicated voice for the current production from the first clip. The Skill asks you to make the choice—it never silently decides the style or voice for you.

Cinematic Drama instead selects or creates a separate confirmed voice reference for every speaking character before formal video generation.

See the complete [built-in voice library](./references/reference-asset-library.md).

## Workflow Status

Storytime Animation adds first-person story collection, a reusable Storytime-only [character library](./modes/storytime-animation/characters/character-library.md), conversational character co-design, narrator performance, and flexible movement between direct address and reenactment. Animated Explainer retains the production workflow that existed before the Mode architecture.

Clay Stop-Motion now has a complete candidate workflow for developing moral premises into fables, planning puppet, recurring-set, and hero-prop references, writing performance-aware narration, and directing Seedance with explicit key poses, physical contact, material response, camera paths, and end states. It still awaits its first end-to-end sample validation.

Cinematic Drama now has a complete candidate workflow. It starts from confirmed worldbuilding, characters, and a script; gives every lead and recurring supporting character an identity reference and a per-character voice, adds 16:9 text-free multi-view cards for leads and important supporting characters when needed, and establishes continuity-critical scene references before generating 15-second dramatic clips. Extras do not require fixed identity or voice assets. It still awaits its first end-to-end sample validation.

1. **Decide what to say.** Research the topic around your audience and target duration, then write a clear, well-structured narration script.
2. **Decide how it should look.** Choose a built-in or custom prompt-defined style, then create references only for characters who must remain recognizable.
3. **Direct the words into scenes.** Break the script into balanced segments and design concrete events, multi-shot direction, and generation-ready prompts for each one.
4. **Validate before scaling.** Produce the first clip, confirm the visual and vocal direction, then lock the voice and required character references before generating the rest.
5. **Finish in an editor.** Download every generated clip, then manually assemble and lightly trim failed edge frames, tiny end-of-clip audio glitches, pacing, and cut points. Automated assembly remains available only when explicitly requested.

The production rhythm validated so far breaks a 1–5 minute video into 15-second clips. Animated Explainer typically targets roughly 60 Chinese characters or about 32 English words and around five shots. English Storytime targets 30 spoken words, normally 28–32, and usually uses 3–5 shots, with about four as the current stable starting point.

The candidate Cinematic Drama rhythm typically uses five shots per 15-second clip, dropping to four or three for longer performance, complex action, or dramatic pauses. Formal clips are locked to Seedance 2.0 Pro at 720p; the workflow does not proactively test Seedance 2.5 Pro or upgrade to 1080p.

Clay Stop-Motion begins sample testing with 3–5 shots per 15-second clip, usually around four, and deliberately leaves more room for stepped key poses, prop contact, material response, and pauses. Narration-density targets remain candidates until a full production validates them.

## Installation

Clone or copy this repository into a skills directory your Agent can access.

If you use Codex, you can also tell it directly:

> Install the `director` skill from `https://github.com/s1dashu/director`.

In Codex, skills are explicitly mentioned with a `$` prefix, so the invocation is `$director`. The skill name itself remains `director`; other Agents should use the invocation convention of their own runtime.

### Migrating from `animated-voiceover`

This project was renamed in place from `animated-voiceover` to `director`. GitHub preserves the repository history, stars, issues, and redirects from the old repository URL, but a copied local skill directory does not rename itself.

- Update existing Git remotes to `https://github.com/s1dashu/director.git`.
- Remove the old local `animated-voiceover` skill directory after installing `director`; keeping both can expose two versions of the same workflow to an Agent.
- Replace explicit Codex mentions of `$animated-voiceover` with `$director`. For other Agents, use their own skill invocation syntax.

## Start with a Single Sentence

Once installed, you can begin with a request like this:

> Use the `director` skill to create a two-minute animated explainer: “Stoicism in Two Minutes.”

Or include more creative direction:

> Use the `director` skill to turn “Why do people procrastinate?” into a 90-second psychology explainer. Use a gentle tone and a hand-drawn style, and confirm the script and visual direction with me first.

To develop a moral story directly in clay stop-motion:

> Use director's Clay Stop-Motion Mode to create a 90-second fable about a young fox who keeps taking shortcuts. Confirm the moral premise and story outline before designing the clay puppets, miniature sets, and Seedance prompts.

With confirmed worldbuilding and a script, you can go straight into dramatic production:

> Use director's Cinematic Drama Mode to produce this approved duel scene as an AI motion comic. Establish the character cards, per-character voices, and scene references first, then give me the prompt for every clip.

The Skill will guide you through the necessary choices. You do not need to understand Seedance prompting, voice anchors, or multimodal asset connections in advance.

## Tools and Scope

`director` currently supports three media-execution CLI paths: [LibTV CLI](./tools/libtv-cli.md), [Higgsfield CLI](./tools/higgsfield-cli.md), and [Jimeng CLI](./tools/jimeng-cli.md). Each has a maintained tool adapter covering its platform's model discovery, asset management, generation tasks, status tracking, and result downloads. LibTV CLI remains the best-supported and most thoroughly production-tested path, so it is still the preferred recommendation when the user has not chosen a platform; Higgsfield CLI and Jimeng CLI are current supported paths, not merely future adaptations.

The current workflow is designed primarily for 1–5 minute videos assembled from multiple 15-second clips. Formal Cinematic Drama clips are locked to Seedance 2.0 Pro at 720p; the workflow does not proactively test Seedance 2.5 Pro or upgrade to 1080p.

For the full execution rules, read [SKILL.md](./SKILL.md). The methods for narration, video prompts, voice references, and cover production are organized under [`references/`](./references/).

## License

Original content in this repository is released under the [MIT License](./LICENSE). Third-party documentation and externally linked content remain subject to their respective licenses and rights.

<p align="center">
  <strong>If you want to direct better videos with Agents, try it, share it, and give the project a Star.</strong>
</p>
