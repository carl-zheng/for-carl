# Changelog

All notable changes to this repository are documented here.

## KreadoAI production binding 0.1.0 — 2026-08-23

- Bound the dinosaur countdown calendar's provider-neutral handoff to a no-secret KreadoAI Seedance adapter without submitting media.
- Added per-job routing, Seedance duration adaptations, reference-input constraints, polling behavior, and an explicit zero-generation schema-discovery gate.
- Kept JOB-04 and JOB-05 editor-first, limited JOB-02 and JOB-06 to clean generated plates, and preserved every exact commercial-text layer for editing.
- Expanded the local plugin allowlist to the three Seedance submission schemas and one polling schema while retaining prompt approval, one-output cost control, and disabled deletion.
- Added regression invariants that prevent missing assets, unknown pricing, or unapproved settings from becoming executable payloads.

## KreadoAI connection verified 0.1.1 — 2026-08-23

- Verified that the installed KreadoAI plugin loads the credential from the local environment and completes an authenticated MCP tool call.
- Used only the public built-in Seedance label-tree query; no media task, crawl, upload, account-private-data request, resubmission, or deletion was performed.
- Kept every generation and remote-write capability locked behind a future explicit approval, with deletion disabled.
- Updated the no-secret platform profile to record successful read-only verification while leaving generation-schema binding pending.

## KreadoAI connection scaffold 0.1.0 — 2026-08-23

- Added a no-secret KreadoAI MCP platform profile for the user's selected video-production provider.
- Registered the custom `apiToken` header through the local `KREADOAI_API_TOKEN` environment-variable binding; no credential is stored in the repository.
- Recorded Seedance models, resolution and ratio support, 4–15 second clip limits, reference limits, polling rules, and unknown pricing as documented but not yet authenticated.
- Limited the first connection test to one read-only public-label query and kept media submission, account data, remote writes, resubmission, and deletion behind explicit approval or disabled.
- Verified that the MCP endpoint is reachable without using a credential; authenticated initialization remains pending the API key.

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

