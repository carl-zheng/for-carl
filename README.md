# for-carl

Reusable Codex skills and supporting resources.

## Skills

- [`applovin-creative-director`](skills/applovin-creative-director/SKILL.md) — develops evidence-grounded AppLovin ecommerce video concepts before scriptwriting and production.
- [`applovin-scriptwriter`](skills/applovin-scriptwriter/SKILL.md) — turns one approved Creative Brief into a timed, claim-safe AppLovin ecommerce video script.
- [`applovin-storyboard-director`](skills/applovin-storyboard-director/SKILL.md) — converts an approved script into a timed, platform-neutral storyboard and production handoff without generating media.

## Workflow

`Product Truth → Creative Director → Creative Brief → Scriptwriter → Script → Storyboard Director → KreadoAI Platform Binding → Video Producer`

The Creative Director owns the advertising idea and evidence boundaries. The Scriptwriter preserves that approved strategy while converting it into spoken copy and timed narrative beats. The Storyboard Director turns the locked script into visual shots, asset requirements, continuity, and provider-neutral job units. The user's existing video-production platform is bound afterward through a separate adapter, so platform limits do not silently rewrite the approved creative.

## Integrations

- [`kreadoai`](integrations/kreadoai/) — no-secret MCP connection and Seedance capability profile. Authentication, live video-tool schemas, and primary product-image bindings are verified; generation remains locked until one named payload is explicitly approved.

For this advertiser's portfolio, content explicitly published on an advertiser-controlled product detail page is approved first-party advertising input. Recognizable subjective or metaphorical advertising exaggeration is also allowed; objective facts must still come from the product page or an explicit user-approved input.

## Regression tests

- [`dinosaur-countdown-calendar`](tests/dinosaur-countdown-calendar/) — complete Product Truth → Creative Brief → Script → Storyboard → platform-neutral handoff → KreadoAI binding test for the United States market, with explicit claim, offer, timing, continuity, asset, provider-routing, and approval invariants.

