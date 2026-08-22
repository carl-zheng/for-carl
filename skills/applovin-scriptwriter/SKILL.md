---
name: applovin-scriptwriter
description: Write claim-safe AppLovin ecommerce video scripts from an approved Creative Brief. Use after strategy, audience, product truth, proof, offer, duration, AIP, and landing promise are defined; do not use to choose the creative strategy, invent claims, create storyboards, shot lists, generation prompts, or final media.
metadata:
  version: 0.1.1
  status: experimental
---

# AppLovin Scriptwriter

Turn one approved creative concept into a persuasive, speakable AppLovin ecommerce video script while preserving the strategy, evidence boundaries, and video-to-AIP-to-landing-page promise.

## Boundary

Own the final voiceover or dialogue, beat-level pacing, transitions, concise on-screen copy, product explanation, proof language, offer wording, CTA, duration estimate, and script-level claim audit.

Do not select the audience, replace the Big Idea, generate additional territories, rewrite product truth, invent proof, create a storyboard or shot list, specify camera or editing instructions, write image/video model prompts, or produce media. If the approved strategy is weak or internally inconsistent, return it for revision instead of silently repairing it through copy.

## Required input

Require one approved Creative Brief plus its Product Truth and claim boundaries. The input must identify:

- one concept and dominant memory
- target market and script language
- audience situation, consumer truth, tension, and purchase motivation
- hook mechanism and product role
- narrative spine
- demonstration and proof strategy
- page-cleared, user-approved, puffery, conditional, missing, and forbidden claims
- offer role and current verified offer
- target duration
- AIP continuation and landing-page promise

If a material element is missing or multiple concepts remain unresolved, output `BRIEF REVISION REQUIRED` with the smallest set of corrections needed. Do not fill strategic gaps by inventing a new concept.

## Writing principles

- Preserve the brief's Big Idea and one dominant memory. Every beat should strengthen that memory or move the viewer toward action.
- Write natural, speakable language for the specified market. For United States scripts, default to conversational US English without forced slang.
- The hook must be repaid by the body. Do not use a sensational opening that the product, proof, and offer cannot support.
- Let visible proof carry persuasion when possible. Narration should clarify what the viewer can verify, not claim more than the demonstration shows.
- Treat content explicitly published on the advertiser-controlled product detail page as `PAGE-CLEARED` first-party advertising input. Page-published reviews, quotations, counts, social proof, urgency, scarcity, and performance statements may be used when Product Truth records them; copy their meaning faithfully and recheck dynamic values before launch.
- Allow recognizable `PUFFERY`: subjective, emotional, playful, or metaphorical language that intensifies an approved benefit without creating a new measurable fact.
- Never fabricate a customer, quotation, reaction, authority, count, event, offer, product capability, or other objective fact that is absent from both the product page and explicit user-approved inputs.
- Use claims marked `PAGE-CLEARED`, `USER-APPROVED`, `USE`, or `PUFFERY`. Omit `CLAIM REQUIRED`, unresolved `PROOF GAP`, conditional, or forbidden claims until their conditions are satisfied.
- Use exact offer and policy values from the approved brief. If price, discount, shipping, returns, AIP, or landing-page information conflicts, output `OFFER CONFLICT` and identify the mismatch.
- Treat duration as a constraint on persuasion, not a reason to pad. As a starting estimate, allow roughly 2.1–2.4 spoken words per second, then reduce the word budget for pauses, reactions, demonstrations, or dialogue. Verify with a read-through.
- Keep on-screen copy shorter than voiceover and avoid duplicating every spoken line.
- Preserve space for downstream visual storytelling. Do not turn the script into production directions.

## Workflow

### 1. Lock the brief

Summarize the concept, dominant memory, duration, allowed proof, offer, and forbidden claims in a compact script lock. If this summary contradicts the brief, stop and request a brief revision.

### 2. Allocate persuasion beats

Map the approved narrative spine into beat-level time budgets. Use only as many beats as the concept needs. The combined time budget must fit the approved duration and leave room for demonstrations or pauses.

### 3. Draft for speech and screen

Write voiceover or dialogue that sounds natural when spoken. Add on-screen copy only where it improves silent comprehension, benefit retention, proof, offer clarity, or CTA.

### 4. Audit claims and continuity

Classify every material line as page-cleared, user-approved, puffery, or unsupported. Check factual sentences against Product Truth and claim boundaries. Confirm that offer wording and CTA can continue unchanged into AIP and the landing page.

### 5. Deliver the script

Use [references/script-contract.md](references/script-contract.md). Produce a human-readable Markdown script by default; when saving into a repository or handing off to an automated pipeline, also provide a structurally equivalent JSON artifact.

## Quality gate

Before finalizing, confirm:

- the first beat earns attention without overpromising
- the product and mechanism enter naturally enough to repay the hook
- the body contains real persuasion rather than repeated Hook copy
- the dominant memory remains clear
- every important line is page-cleared, user-approved, recognizable puffery, or otherwise supportable
- the offer is exact and current according to the supplied brief
- estimated speech plus visual pauses fits the duration
- the CTA continues into the specified AIP and landing promise
- no storyboard, camera, model-prompt, or editing work has leaked into the script

If any check fails, revise once. If revision would require changing strategy or inventing evidence, return `BRIEF REVISION REQUIRED` instead.
