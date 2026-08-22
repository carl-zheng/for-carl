# for-carl

Reusable Codex skills and supporting resources.

## Skills

- [`applovin-creative-director`](skills/applovin-creative-director/SKILL.md) — develops evidence-grounded AppLovin ecommerce video concepts before scriptwriting and production.
- [`applovin-scriptwriter`](skills/applovin-scriptwriter/SKILL.md) — turns one approved Creative Brief into a timed, claim-safe AppLovin ecommerce video script.
- [`applovin-storyboard-director`](skills/applovin-storyboard-director/SKILL.md) — converts an approved script into a timed, platform-neutral storyboard and production handoff without generating media.

## Workflow

`Product Truth → Creative Director → Creative Brief → Scriptwriter → Script → Storyboard Director → Platform Binding → Video Producer`

The Creative Director owns the advertising idea and evidence boundaries. The Scriptwriter preserves that approved strategy while converting it into spoken copy and timed narrative beats. The Storyboard Director turns the locked script into visual shots, asset requirements, continuity, and provider-neutral job units. The user's existing video-production platform is bound afterward through a separate adapter, so platform limits do not silently rewrite the approved creative.

For this advertiser's portfolio, content explicitly published on an advertiser-controlled product detail page is approved first-party advertising input. Recognizable subjective or metaphorical advertising exaggeration is also allowed; objective facts must still come from the product page or an explicit user-approved input.

## Regression tests

- [`dinosaur-countdown-calendar`](tests/dinosaur-countdown-calendar/) — complete Product Truth → Creative Brief → Script → Storyboard → platform-neutral production handoff test for the United States market, with Markdown and JSON artifacts plus explicit claim, offer, timing, continuity, and platform-binding invariants.
