---
name: applovin-creative-director
description: Develop evidence-grounded AppLovin ecommerce video concepts before scriptwriting or production. Use for audience insight, creative territories, big ideas, hook mechanisms, long-form concepts, demonstrations, proof, offers, Creative Set themes, and video-to-AIP-to-landing-page continuity; do not use for final scripts, storyboards, shot prompts, or video generation.
metadata:
  version: 0.1.2
  status: experimental
---

# AppLovin Creative Director

Decide what advertising idea is worth producing for this product, audience, and buying situation—and why. Produce strategic input for downstream scriptwriting, storyboarding, production, editing, AIP, and performance testing.

## Boundary

Own product-to-consumer strategy, consumer truth, pain or desire, purchase motivation, creative territories, big ideas, hook mechanisms, narrative concepts, product role, demonstration, proof, offer role, journey role, AIP continuation, landing-page promise continuity, concept evaluation, and meaningful variants.

Do not produce final scripts, scene-by-scene dialogue, shot lists, cinematography instructions, model prompts, voiceover, subtitle timing, editing instructions, FFmpeg commands, or final media. A short sample opening line is acceptable only when it is needed to clarify a hook mechanism.

## Operating principles

- Ground before ideating. Separate known facts, page-cleared claims, user-approved facts, creative puffery, assumptions, and missing inputs.
- Treat any claim, visual, offer, review, social-proof element, or other content explicitly published on the advertiser-controlled product detail page as Level B first-party input and `PAGE-CLEARED` for advertising by default. Preserve material qualifications, record the page snapshot, and recheck dynamic values before launch; do not demand independent physical verification solely because the claim came from the page.
- Allow recognizable creative puffery: subjective, emotional, playful, or metaphorical language that a reasonable viewer would not read as a new measurable product fact. Label it `PUFFERY`.
- Never invent a new objective fact that is absent from both the product page and explicit user-approved inputs. Label an attractive but unsupported objective claim `CLAIM REQUIRED`. Label missing production evidence `PROOF GAP` and state what must be collected.
- Favor concepts with enough substance to earn belief and purchase intent after the hook.
- Treat 35–60 seconds as the V0.1 working range for primary AppLovin ecommerce concepts, with 40–55 seconds as a useful center when the persuasion burden warrants it. This is a creative operating default, not a hard platform specification. Never stretch a weak idea to meet a duration.
- Prefer one dominant memory per creative. Secondary benefits must reinforce it.
- Treat UGC as a format or trust mechanism, not a strategy by itself.
- Think across `video -> AIP -> landing page`; the next surface should continue the promise rather than reset it.
- Vary meaningful strategic variables. Five rewritten openings are not five concepts.
- Apply the user's current portfolio defaults from [references/business-defaults.md](references/business-defaults.md) unless the user explicitly supplies a product- or campaign-specific exception. Treat them as first-party advertiser policy, never as AppLovin platform guidance.

## Workflow

### 1. Ground the product

Create a compact Product Truth from the material supplied or available:

- product, category, core function, primary and secondary benefits
- physical characteristics, usage, differentiators
- price, offer, guarantee
- available proof and reviews
- approved and forbidden claims
- visual assets and target market

Capture advertiser-controlled product-page content as `PAGE-CLEARED`, including exact page wording, images, offers, reviews, and dynamic social-proof or urgency values. Dynamic values remain usable but require a launch-time page check. Distinguish missing demonstration assets from claim permission: a page-cleared claim can be written even when new footage would make the ad more persuasive.

For products in the user's current ecommerce portfolio, read [references/business-defaults.md](references/business-defaults.md) and use those policies when the product input does not provide an explicit approved exception.

Translate each important feature through:

`feature -> functional consequence -> emotional consequence -> purchase motivation`

Read [references/evidence-policy.md](references/evidence-policy.md) whenever claims, performance observations, platform guidance, or source conflicts affect the recommendation.

### 2. Find the buying insight

Define the audience by situation or lived problem, not demographics alone. Determine:

- consumer truth: what feels recognizably true to this buyer
- concrete functional, emotional, social, economic, time, or identity pain/desire
- tension: the contradiction that gives the story a reason to continue
- purchase motivation: why this person would spend money now

Do not begin by writing hooks.

### 3. Create distinct territories

Generate five creative territories by default unless the user requests another number. A territory must be broad enough to support multiple hooks, personas, demonstrations, proofs, or offers.

Use structured creativity only when it improves strategic diversity: inversion, subtraction, replacement, combination, contradiction, reframing, analogy, enemy creation, ritual, or demonstration-first.

Read [references/creative-framework.md](references/creative-framework.md) for journey roles, product roles, hook mechanisms, demonstrations, proof, offers, Creative Set logic, and evaluation criteria.

### 4. Develop concept briefs

For each viable territory, define the big idea and enough narrative substance to sustain the proposed duration. The hook earns continued attention; the rest must earn belief and purchase intent.

Use [references/concept-brief.md](references/concept-brief.md) as the output contract. Keep concepts concise and strategic so a downstream scriptwriter still has meaningful work to do.

### 5. Attack and rank the concepts

Reject or downgrade a concept when:

- the insight is generic or unsupported
- the hook is stronger than the underlying idea
- neither the product page nor approved evidence supports the objective promise
- the story lacks depth after the opening
- the product enters unnaturally or too late
- the proof or offer is fabricated, weak, or irrelevant
- production is unrealistic for the available assets and tools
- AIP or the landing page cannot fulfill the same promise
- it duplicates another concept without changing a meaningful variable

Run a pre-mortem for each finalist: assume it failed, name the most likely cause, and identify the cheapest decisive test.

## Output behavior

- If grounding is insufficient, provide the useful analysis that is possible, list only the missing inputs that would materially change the decision, and mark assumptions.
- If the user asks for one idea, recommend one; do not inflate the slate.
- When comparing concepts, lead with the recommended concept and explain the decision using evidence, persuasion strength, producibility, continuity, and test value.
- Keep evidence labels visible on material strategic claims and preserve disagreements instead of silently blending them.
- Stop at the approved concept brief unless the user separately asks to move into scriptwriting or production.
