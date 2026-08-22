# AppLovin Storyboard — Dinosaur Adventure Countdown Calendar

## 1. Visual lock

- **Storyboard:** `dac-us-24-mornings-storyboard-v1` / `1.0.0`
- **Source script:** `dac-us-24-mornings-script-v1` / `1.1.0`
- **Approved concept:** 24 Mornings of Dino Excitement
- **Dominant memory:** 24 mornings, 24 dinosaur surprises.
- **Market and language:** United States; English (US)
- **Total duration:** 50 seconds
- **Delivery format:** `PLATFORM-NEUTRAL`; aspect ratio, resolution, and frame rate are `UNBOUND`
- **Platform binding:** `PENDING_USER_PLATFORM`
- **Handoff target:** `READY_FOR_PLATFORM_BINDING`

Visuals may use `PAGE-CLEARED` product-page claims and recognizable `PUFFERY`, but may not create a new measurable product fact. The `$35.90` price and other dynamic values require a launch-time recheck. Free standard shipping must remain qualified as applying to orders `$49+`; returns remain 30 days unless the user supplies an explicit exception.

## 2. Asset inventory

| Asset ID | Requirement | Access | Inspection | Origin | Description and role |
|---|---|---|---|---|---|
| `ASSET-P01` | `REQUIRED` | `OBSERVED_NOT_SUPPLIED` | `PARTIALLY_INSPECTED` | Product page | Nine static product-page images observed in Product Truth; exact file-to-role mapping still needs export. Master source set for identity and continuity. |
| `ASSET-R01` | `REQUIRED` | `NOT_SUPPLIED` | `NOT_INSPECTED` | Product-page selection | Clean full-calendar reference selected from `ASSET-P01`; master product and motion reference. |
| `ASSET-R02` | `REQUIRED` | `NOT_SUPPLIED` | `NOT_INSPECTED` | Product page or real capture | Page-consistent close-up of a numbered door and reveal interaction; motion reference and proof. |
| `ASSET-R03` | `REQUIRED` | `NOT_SUPPLIED` | `NOT_INSPECTED` | Product page or real capture | Visibly different figures and, if available, a complete 24-figure lineup; identity reference and proof. |
| `ASSET-R04` | `REQUIRED_WITH_FALLBACK` | `NOT_SUPPLIED` | `NOT_INSPECTED` | Product page or real capture | Faithful ornament-use visual; static, motion-reference, and proof role. |
| `ASSET-G01` | `OPTIONAL` | `NOT_SUPPLIED` | `NOT_APPLICABLE` | Editor or generated candidate | Generic December-morning environment with no customer-reaction implication. |
| `ASSET-G02` | `REQUIRED` | `NOT_SUPPLIED` | `NOT_APPLICABLE` | Editor-created graphic | Exact editable price, free-shipping, and return overlays. |
| `ASSET-A01` | `REQUIRED` | `NOT_SUPPLIED` | `NOT_APPLICABLE` | Downstream audio production | Final approved US English voiceover recording. |
| `ASSET-A02` | `OPTIONAL` | `NOT_SUPPLIED` | `NOT_APPLICABLE` | Downstream audio production | Music and light reveal sound effects that add no product claim. |

## 3. Shot plan

| Shot | Time | Beat | Voiceover mapping | On-screen copy | Visual action and composition | Product state | Source / assets | Claim and continuity |
|---|---:|---|---|---|---|---|---|---|
| `S01` | 0–3 sec | Opening | What if every December morning could roar with dinosaur excitement? | Make December roar | Seasonal morning light with a playful dinosaur-shaped shadow or graphic motif; wide, center-safe opening composition. | `OFFSCREEN` | `AI_GENERATION_CANDIDATE`; `ASSET-G01` | `PUFFERY`, not a physical product feature. Seasonal light carries into S02. |
| `S02` | 3–6 sec | Opening | `CONTINUES` — no new words | — | Closed calendar settles into the same seasonal setting; centered hero framing with the real design unobstructed. | `CLOSED_CALENDAR_ALL_DOORS_INTACT` | `MOTION_FROM_REFERENCE`; `ASSET-R01`, `ASSET-G01` | `PAGE-CLEARED` product appearance. Establishes the master product reference. |
| `S03` | 6–10 sec | Product reveal | The Dinosaur Adventure Countdown Calendar turns one Christmas gift into a 24-day ritual. | 24-day dinosaur countdown | Full calendar centered with the numbered-door structure clear and short-title overlay space. | `CLOSED_CALENDAR_ALL_DOORS_INTACT` | `MOTION_FROM_REFERENCE`; `ASSET-R01` | `PAGE-CLEARED` 24-day structure; same identity and door state as S02. |
| `S04` | 10–13 sec | Product reveal | `CONTINUES` — no new words | — | Editor callouts trace representative numbers over the real calendar without changing its layout. | `CLOSED_CALENDAR_ALL_DOORS_INTACT` | `EDITOR_GRAPHIC`; `ASSET-R01` | `PAGE-CLEARED` 24 numbered doors; prepares first interaction. |
| `S05` | 13–18 sec | Daily ritual | Open one numbered door each day and discover a unique dinosaur waiting inside—24 surprises, no repeats. | 24 unique dinosaurs · No repeats | Generic hand opens one numbered door and reveals the first page-consistent figure; close interaction framing. | `ONE_DOOR_OPEN_ONE_FIGURE_REVEALED` | `MOTION_FROM_REFERENCE`; `ASSET-R01`, `ASSET-R02`, `ASSET-R03` | `PAGE-CLEARED`; the hand is not a customer testimonial. One open door and figure carry forward. |
| `S06` | 18–21 sec | Daily ritual | `CONTINUES` — no new words | — | A second numbered door opens to a visibly different page-consistent dinosaur in matched framing. | `TWO_DOORS_OPEN_TWO_DIFFERENT_FIGURES_REVEALED` | `MOTION_FROM_REFERENCE`; `ASSET-R01`, `ASSET-R02`, `ASSET-R03` | `PAGE-CLEARED` no-repeat claim; preserve S05 door and figure state. |
| `S07` | 21–23 sec | Daily ritual | `CONTINUES` — no new words | — | Third quick reveal resolves on three visibly different figures together. | `THREE_DOORS_OPEN_THREE_DIFFERENT_FIGURES_REVEALED` | `MOTION_FROM_REFERENCE`; `ASSET-R01`, `ASSET-R02`, `ASSET-R03` | `PAGE-CLEARED` variety; three-figure lineup begins collection growth. |
| `S08` | 23–27 sec | Collection growth | Morning by morning, the collection grows, all the way to day twenty-four. | 24 mornings. 24 dinosaur surprises. | Editor-controlled increments grow the display from three figures into a larger page-consistent collection without labeling an unsupported intermediate count. | `GROWING_COLLECTION` | `EDITOR_GRAPHIC`; `ASSET-R03` | `PAGE-CLEARED` 24-day accumulation; figure identity stays stable. |
| `S09` | 27–31 sec | Collection growth | `CONTINUES` — no new words | — | Resolve on all 24 figures only when a faithful source exists; otherwise retain a clearly growing collection without inventing unseen designs. | `COMPLETE_24_FIGURE_LINEUP_IF_SOURCE_AVAILABLE_OTHERWISE_GROWING_COLLECTION` | `UNRESOLVED`; `ASSET-R03` | `PAGE-CLEARED` claim with a truthful fallback; displayed figures carry into S10. |
| `S10` | 31–35 sec | After-countdown value | After the countdown, collect them, display them, play with them, or hang them as dinosaur Christmas ornaments. | Collect · Display · Play · Hang | Editor-controlled panels show page-consistent figures collected, displayed, and in generic play, without a testimonial reaction. | `FIGURES_OUTSIDE_CALENDAR_IN_APPROVED_USE_CONTEXTS` | `EDITOR_GRAPHIC`; `ASSET-R03` | `PAGE-CLEARED` use cases; one established figure leads into ornament use. |
| `S11` | 35–38 sec | After-countdown value | `CONTINUES` — no new words | — | Use a supplied faithful ornament-use visual; otherwise use a static page-copy card instead of inventing a hanging mechanism. | `ORNAMENT_USE_IF_SOURCE_AVAILABLE` | `UNRESOLVED`; `ASSET-R04` | `PAGE-CLEARED`; mechanism must match the source. Seasonal styling leads into offer. |
| `S12` | 38–43 sec | Offer and action | One calendar is $35.90. Free standard shipping on orders $49+. Plus, 30-day returns. Tap a door, reveal a dinosaur, and make December roar. | $35.90 each | Calendar and selected figures return in a clean hero composition; price is an editor-owned overlay. | `OFFER_HERO_SINGLE_CALENDAR` | `MOTION_FROM_REFERENCE`; `ASSET-R01`, `ASSET-R03`, `ASSET-G02` | `VERIFY BEFORE LAUNCH`; do not imply single-item free shipping. Same product identity throughout. |
| `S13` | 43–47 sec | Offer and action | `CONTINUES` — no new words | Free standard shipping on orders $49+ · 30-day returns | Editor-owned policy text replaces the price while the hero plate remains stable. | `OFFER_HERO_POLICY_STATE` | `EDITOR_GRAPHIC`; `ASSET-R01`, `ASSET-G02` | User-approved defaults; threshold stays attached to shipping. Overlay remains editable. |
| `S14` | 47–50 sec | Offer and action | `CONTINUES` — no new words | — | Isolate one numbered door with a clear tap target and hold before reveal so the AIP can continue the action. | `AIP_HANDOFF_DOOR_CLOSED_READY_TO_TAP` | `EDITOR_GRAPHIC`; `ASSET-R01` | Cleared AIP continuation; same calendar, one closed door, and one clear tap target. |

## 4. Continuity map

- **Product identity:** `ASSET-R01` is the master calendar reference; `ASSET-R03` is the master figure reference. Do not redesign packaging, colors, layout, numbering, or figures.
- **Door state:** S02–S04 all intact → S05 one open → S06 two open → S07 three open.
- **Collection state:** Three figures at S07 expand through S08; S09 shows all 24 only when the faithful source exists.
- **Generic hand:** If used in S05–S07, keep its general appearance and interaction direction consistent; it does not represent a customer.
- **Seasonal styling:** Carry the same December light and restrained seasonal colors from S01–S02 into S11–S12.
- **Commercial copy:** Price, shipping threshold, returns, logo, and subtitles stay editable and outside generated in-scene typography.
- **AIP transition:** S14 ends on the same calendar with one closed numbered door ready to tap.

## 5. Gaps

- `GAP-01` — `PLATFORM-BINDING`: provider, aspect ratio, resolution, frame rate, clip limits, reference limits, and audio capabilities are not yet supplied.
- `GAP-02` — `REQUIRED_PRODUCTION_ASSET`: export and map `ASSET-P01`, select the clean `ASSET-R01` master reference, and select or capture `ASSET-R02` before their production jobs run.
- `GAP-03` — `QUALITY-UPGRADE`: select a faithful 24-figure lineup for S09; otherwise use the approved growing-collection fallback.
- `GAP-04` — `QUALITY-UPGRADE`: select product-page ornament imagery or a faithful real capture for S11; otherwise use the static claim-card fallback.
- `GAP-05` — `LAUNCH-GATE`: recheck price, bundle savings, destination copy, shipping threshold, returns, and dynamic page content before final export.

## 6. Final checks

- **Shots:** 14
- **Duration:** 50 seconds
- **Timeline integrity:** `PASS`
- **Script-copy integrity:** `PASS`
- **Visual-claim audit:** `PASS`
- **Asset coverage:** `PASS_WITH_NAMED_GAPS`
- **Continuity risk:** `MANAGEABLE_WITH_REFERENCE_LOCKS`
- **Platform binding:** `PENDING_USER_PLATFORM`
- **Final status:** `READY_FOR_PLATFORM_BINDING`
