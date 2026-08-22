# Changelog

All notable changes to this repository are documented here.

## Storyboard Director 0.1.0 — 2026-08-23

- Added the experimental `applovin-storyboard-director` skill for converting approved scripts into timed visual shot plans, asset maps, continuity locks, and production handoffs.
- Added a platform-neutral binding contract so the user's existing video-production platform can be connected later without rewriting the approved creative, script, claims, offer, or timing.
- Extended the dinosaur regression fixture with matching Markdown and JSON storyboards, 14 continuous shots over 50 seconds, a provider-neutral production handoff, and platform-binding invariants.
- Kept provider prompts and payloads out of the storyboard layer and left unknown delivery specifications explicitly `UNBOUND`.
- Separated asset requirement, access, and inspection states, and added `REQUIRED_PRODUCTION_ASSET` so missing capture inputs are not mislabeled as storyboard or claim blockers.

## Director 0.1.2 / Scriptwriter 0.1.1 — 2026-08-23

- Made advertiser-controlled product-detail-page content `PAGE-CLEARED` for advertising without an additional physical-verification gate.
- Added `PUFFERY` for recognizable subjective, emotional, playful, or metaphorical exaggeration while keeping new objective facts source-bound.
- Updated the dinosaur regression fixture and script to exercise the page-cleared no-repeat and ornament claims plus the “make December roar” puffery line.
- Kept dynamic page values subject to a launch-time recheck and prohibited fabricated customers, quotations, counts, events, and other unsupported objective facts.

## Scriptwriter 0.1.0 — 2026-08-23

- Added the experimental `applovin-scriptwriter` skill for converting one approved Creative Brief into a timed, claim-safe video script.
- Added the first end-to-end Product Truth → Creative Brief → Script regression fixture for the Dinosaur Adventure Countdown Calendar.
- Added matching Markdown and JSON artifacts, explicit offer and claim invariants, and a 45–50 second forward-test script.

## 0.1.1 — 2026-08-22

- Added portfolio-wide United States defaults of free standard shipping at a $49 order subtotal and a 30-day return period.
- Clarified that these are first-party advertiser policies and may be overridden only by an explicit product- or campaign-specific instruction.

## 0.1.0 — 2026-08-22

- Added the experimental `applovin-creative-director` skill.
- Added evidence handling, creative framework, and concept brief references.
- Established a strategy-only boundary before downstream scriptwriting and production.
