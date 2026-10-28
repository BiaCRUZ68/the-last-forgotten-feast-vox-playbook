# The Last Forgotten Feast — Vox-Inspired Documentary Playbook

A reusable production system for **The Last Forgotten Feast**, a historical food documentary channel exploring the hidden stories behind dishes, ingredients, trade routes, food technology, and the people who shaped what humanity eats.

> History isn't made only through wars and coronations — it's served at the table.

This repository adapts the *structure* of Vox-style explanatory documentaries into an original editorial and production workflow for The Last Forgotten Feast. It is an independent project and is not affiliated with Vox.

## Editorial identity

**Channel promise:** Bring lost banquets, forgotten ingredients, and flavors that shaped humanity back to life through evidence-based storytelling and sensory reconstructions.

**Core principles**
1. **A question drives every episode.** Begin with a striking food-related mystery, contradiction, or consequence.
2. **Food remains central.** Politics, class, trade, science, religion, and technology matter because they reveal something about what people ate and why.
3. **Evidence before drama.** Separate documented facts, scholarly interpretations, and plausible reconstructions. Never invent quotations, sources, recipes, measurements, or historical certainty.
4. **Explain visually.** Use maps, timelines, diagrams, annotated objects, ingredient close-ups, process illustrations, and comparisons to make complex ideas clear.
5. **Sensory immersion supports the investigation.** Use ASMR and foley thoughtfully; never let sound design imply an event or detail that the evidence does not support.
6. **Original identity, not imitation.** Use explanatory visual storytelling as a broad model while building a distinct Last Forgotten Feast visual language.

## Repository map

- `SYSTEM_PROMPT.md` — master production-agent instructions.
- `prompts/01_RESEARCH_BRIEF.md` — evidence-first research and claim verification.
- `prompts/02_SCRIPT_PROMPT.md` — long-form documentary script drafting.
- `prompts/03_VISUAL_STORYBOARD_PROMPT.md` — scene-by-scene visual planning.
- `prompts/04_AUDIO_ASMR_PROMPT.md` — a separate sound-design pass.
- `templates/EPISODE_BRIEF.md` — episode planning form.
- `templates/CLAIM_LEDGER.csv` — claim-level evidence tracking.
- `checklists/FINAL_QA.md` — editorial and production quality control.

## Recommended workflow

1. **Choose the question.** Confirm the topic has a compelling food-centered story and enough credible evidence.
2. **Research before scripting.** Build the claim ledger, consult primary evidence where available, and use reputable scholarly sources.
3. **Define the thesis.** Decide what the episode will explain—not just what it will cover.
4. **Write the narration.** Use a clear question-led structure, logical reveals, and visual explanations. Keep production directions out of the narration draft.
5. **Build the visual storyboard.** Map every beat to a narration cue, visual purpose, source/claim IDs, image prompt, and image-to-video prompt.
6. **Design sound separately.** Add ambience, ASMR, foley, and music after the narration and visual logic are stable.
7. **Run final QA.** Check facts, pacing, visual legibility, rights, continuity, sound levels, and the final export.

## Default episode target

Use **10–15 minutes** as the default planning range, adjusting when the subject genuinely calls for a shorter or longer treatment. As an initial narration estimate, plan around 145–155 spoken words per minute, then validate the actual runtime with a timed read.

## First-use instructions

Start with `templates/EPISODE_BRIEF.md`, then run the research prompt. Do not draft the full script until the core thesis and claim ledger are sufficiently developed. For each episode, save the episode-specific files in a separate folder (for example, `episodes/episode-slug/`) so research, script, storyboard, and audio decisions stay traceable.

## Historical accuracy and ethics

- Cite specific claims in working documents with claim IDs and source details.
- Never fabricate source titles, page numbers, archival references, direct quotations, or precise historical recipes.
- Mark uncertainty explicitly and avoid presenting disputed interpretations as settled fact.
- Label reconstructions as reconstructions when they are not directly documented.
- Do not present modern recipes or ingredients as exact historical equivalents without evidence.
- Confirm licenses and usage rights for music, sound effects, archival images, fonts, and other assets.

## Relationship to the source playbook

Use the upstream Vox-style documentary repository as a structural reference only. This repository is a channel-specific adaptation with its own workflow, prompts, and editorial rules; it does not replace or modify the upstream project.
