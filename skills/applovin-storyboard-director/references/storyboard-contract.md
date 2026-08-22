# Storyboard Output Contract

Use the lightest structure that preserves timing, visual proof, asset traceability, and downstream execution.

## 1. Visual lock

- Storyboard ID and version
- Source script ID and version
- Approved concept and dominant memory
- Target market and language
- Exact total duration
- Delivery format: verified platform values or `UNBOUND`
- Claim and offer constraints
- Platform-binding status

## 2. Asset inventory

For each known or required asset record:

- stable asset ID
- description without inventing uninspected details
- requirement status: `REQUIRED`, `REQUIRED_WITH_FALLBACK`, or `OPTIONAL`
- access state: `IN_WORKSPACE`, `CONNECTED_SOURCE`, `OBSERVED_NOT_SUPPLIED`, `NOT_SUPPLIED`, or `UNKNOWN`
- inspection state: `INSPECTED`, `PARTIALLY_INSPECTED`, `NOT_INSPECTED`, or `NOT_APPLICABLE`
- origin: product page, real capture, editor-created graphic, or generated candidate
- usable roles: identity reference, static use, motion reference, proof, background, overlay, or audio
- claim or continuity relevance

Do not use requirement status as a proxy for access. An asset can be required while not yet supplied, and an image observed on a page is not `IN_WORKSPACE` until the actual file or a usable connected-source reference is available. Never describe an uninspected asset as showing a specific feature.

## 3. Shot plan

Use one row or object per shot:

| Field | Requirement |
|---|---|
| Shot ID | Stable sequential identifier |
| Time | Start, end, and duration; no gaps or overlaps |
| Parent beat | Exact source-script beat |
| Visual purpose | Why this shot exists in the persuasion sequence |
| Voiceover mapping | Exact approved words heard during the shot, or `CONTINUES` when the line spans adjacent shots |
| On-screen copy | Exact approved copy, blank, or an audited addition |
| Visual action | What the viewer sees happen, without model-specific prompt syntax |
| Framing / composition | Useful production framing without lens or provider-specific settings unless supplied |
| Product state | Closed, door opened, figure revealed, lineup count, offer state, or other continuity state |
| Source strategy | One of the six allowed source strategies |
| Asset requirement | Stable asset IDs needed for the shot |
| Claim / proof note | Product Truth, `PAGE-CLEARED`, `PUFFERY`, policy, or `NO CLAIM` |
| Continuity in / out | State that must match adjacent shots |
| Capability need | Provider-neutral need such as still-to-motion, reference consistency, compositing, or overlay |

Do not split words merely to force a visual cut. When exact word-to-frame timing is unavailable, map the full line to its parent shot group and keep the sequence order stable.

## 4. Continuity map

Lock only details that matter across shots:

- product identity and packaging
- calendar layout and numbered doors
- figure appearance, collection count, and scale relationships
- hand, environment, lighting, and seasonal styling when repeated
- offer, policy, and CTA text
- AIP transition state

## 5. Asset and production gaps

Distinguish:

- `BLOCKING`: no truthful or coherent visual can be produced
- `REQUIRED_PRODUCTION_ASSET`: the storyboard is valid, but a planned capture, source file, voice recording, or other required input must be supplied or created before its production job can run
- `PLATFORM-BINDING`: the visual plan is complete but provider capability is unknown
- `QUALITY-UPGRADE`: an optional asset would make the proof more convincing
- `LAUNCH-GATE`: the storyboard is valid, but final export must wait for a current commercial value, policy, permission, or other time-sensitive check

Do not turn a required production asset or quality upgrade into a claim-permission requirement. Use `BLOCKING` only when the storyboard itself cannot remain truthful or coherent.

## 6. Final checks

Report:

- total shot count and total duration
- timeline integrity
- script-copy integrity
- visual-claim audit
- asset coverage
- continuity risks
- platform-binding status
- handoff status

## Repository mode

Create `storyboard-v1.md` and `storyboard-v1.json`. They must agree on all shot-level fields, visual locks, asset IDs, unresolved items, and final status.
