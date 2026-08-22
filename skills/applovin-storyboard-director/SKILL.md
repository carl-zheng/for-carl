---
name: applovin-storyboard-director
description: Convert an approved AppLovin ecommerce video script into a platform-neutral storyboard, timed shot plan, asset map, continuity plan, and production handoff. Use after the Creative Brief and script are locked and before model-specific prompting or video production; do not use to change strategy or copy, generate media, edit the final video, or submit jobs to a production platform.
metadata:
  version: 0.1.0
  status: experimental
---

# AppLovin Storyboard Director

Turn one approved script into a visually executable plan without changing the advertising idea, spoken copy, offer, or claim boundaries. Produce the bridge from scriptwriting to the user's eventual video-production platform.

## Boundary

Own shot segmentation, shot timing, visual purpose, framing and composition, subject action, product state, on-screen-copy placement, asset-source decisions, visual proof, continuity, transition intent, production risks, and a platform-neutral production handoff.

Do not choose a new audience or Big Idea, rewrite voiceover or dialogue, change the offer, introduce an unaudited claim, write model-specific prompts or API payloads, generate images or video, render a timeline, perform final editing, or submit work to a production platform.

## Required input

Require:

- one approved Creative Brief
- Product Truth and claim boundaries
- one final approved script with exact beat timing, spoken copy, on-screen copy, and claim audit
- an inventory of known product-page assets, real footage, and missing assets

A production-platform profile is optional. When it is absent, complete the storyboard in `PLATFORM-NEUTRAL` mode and set `platform_binding.status` to `PENDING_USER_PLATFORM`. Do not guess the provider, aspect ratio, resolution, frame rate, clip limits, prompt syntax, reference-image limits, audio support, or API behavior.

If the script is not final, timing is internally inconsistent, or a required visual would contradict Product Truth, output `STORYBOARD REVISION REQUIRED` with the smallest upstream correction needed.

## Operating rules

- Preserve upstream locks. Every spoken line remains verbatim, the shot timeline stays inside its parent script beat, and all shots form one continuous timeline with no overlap or gap.
- Use only page-cleared, user-approved, or properly classified puffery. A visual metaphor may amplify feeling, but it must not make the physical product appear to have an unsupported feature, quantity, material, safety result, transformation, or performance.
- Treat missing real footage as an asset or persuasion gap, not a permission gate for page-cleared claims.
- Track asset requirement, access, and inspection separately. Being required does not mean a file is available, and observing an image on a page does not mean it has been supplied or fully inspected.
- Assign every shot one primary source strategy: `EXISTING_PAGE_ASSET`, `REAL_CAPTURE`, `MOTION_FROM_REFERENCE`, `AI_GENERATION_CANDIDATE`, `EDITOR_GRAPHIC`, or `UNRESOLVED`.
- Never fabricate a customer, testimonial, product reaction, review, live event, scarcity signal, or visual proof absent from approved inputs. A generic hand or environment may be proposed as production material without implying a customer experience.
- Keep product identity stable across shots. Lock packaging, calendar layout, door numbering, dinosaur appearance, colors, scale relationships, offer text, and any other continuity-critical state supported by the source assets.
- Prefer overlays in the downstream editing layer instead of asking a generative video model to render exact prices, policy text, logos, or small typography unless the eventual platform profile explicitly provides a reliable text workflow.
- Describe capability needs, not provider syntax. Model prompts and job payloads belong to the downstream Video Producer or platform adapter.

## Workflow

### 1. Lock the upstream artifacts

Record script ID and version, concept, dominant memory, duration, exact voiceover, approved on-screen copy, claims, offer, AIP continuation, and landing-page promise. Stop if these sources disagree materially.

### 2. Audit available assets

Map each known asset to a usable role and state whether it is sufficient for static use, motion from reference, continuity reference, proof, or overlay. Do not invent filenames or claim that an uninspected asset shows a specific feature.

### 3. Build the shot plan

Break each script beat into the fewest shots needed for comprehension and persuasion. Use [references/storyboard-contract.md](references/storyboard-contract.md) for the shot fields and output structure.

### 4. Lock visual proof and continuity

For every factual visual, identify the Product Truth or page-cleared source. Track the product state entering and leaving each shot, and identify reference assets that must carry across generated clips.

### 5. Create the production handoff

Read [references/platform-handoff.md](references/platform-handoff.md). When the user's existing production platform is not yet connected, output a provider-neutral capability package and the minimum binding questions. When a verified platform profile is supplied, map requirements to that profile without generating model prompts or submitting jobs.

### 6. Run the quality gate

Confirm timeline integrity, verbatim spoken copy, claim-safe visuals, readable overlay allocation, asset traceability, continuity, AIP handoff, and the absence of provider assumptions or production execution.

## Output behavior

Produce a human-readable Markdown storyboard by default. In repository or automated-pipeline mode, create:

- `storyboard-v1.md`
- `storyboard-v1.json`
- `production-handoff-v1.json`

The Markdown and JSON must agree on shot IDs, timing, spoken-copy mapping, on-screen copy, visual intent, source strategy, claim support, and unresolved assets.

End with one status:

- `READY_FOR_PLATFORM_BINDING` when the storyboard is complete but the production platform is not yet profiled
- `READY_FOR_VIDEO_PRODUCER` when the verified platform profile is mapped
- `STORYBOARD REVISION REQUIRED` when a material upstream inconsistency prevents a truthful executable plan

## Quality gate

Before delivery, confirm:

- shots are continuous, non-overlapping, and sum to the approved duration
- every shot remains within its parent script beat
- spoken copy is verbatim and ordered exactly as approved
- no new objective claim or offer value appears in visuals or overlays
- each shot has one source strategy and a named asset requirement
- continuity-critical product details are locked
- exact commercial text is assigned to an overlay or verified text workflow
- missing platform information is explicit rather than guessed
- no model-specific prompt, API payload, generation call, or final edit has leaked into the output
