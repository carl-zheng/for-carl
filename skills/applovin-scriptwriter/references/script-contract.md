# Script Output Contract

Use the lightest form that preserves timing, spoken language, proof, and handoff clarity.

## 1. Script lock

- Script ID and version
- Approved concept
- Target market and language
- Target duration
- Dominant memory
- Allowed proof
- Offer snapshot and verification requirement
- Claims excluded from this script

## 2. Beat script

Use one row per persuasion beat:

| Beat | Time budget | Purpose | Voiceover / dialogue | On-screen copy | Demonstration dependency | Evidence note |
|---|---:|---|---|---|---|---|

Rules:

- Time budgets should fit within the approved duration but remain estimates until performed.
- `Voiceover / dialogue` contains the final spoken copy, not a summary.
- `On-screen copy` should be concise and may be blank.
- `Demonstration dependency` names what must be visibly true without specifying shots, lenses, camera moves, editing, or model prompts.
- `Evidence note` points to Product Truth, an allowed claim, or a clearly unresolved requirement.

## 3. Clean read-through

Provide the spoken copy as one uninterrupted read so cadence, repetition, and duration can be evaluated. Do not include production notes inside it.

## 4. Timing estimate

Report:

- spoken word count
- target duration
- implied words per minute before pauses
- planned allowance for demonstrations, reactions, or silence
- status: `FITS`, `TIGHT`, or `TOO LONG`

Do not claim exact runtime without an actual timed performance.

## 5. Claim and offer audit

List each material factual or commercial statement with:

- script wording
- supporting Product Truth field or policy
- status: `CLEARED`, `PAGE-CLEARED`, `PUFFERY`, `VERIFY BEFORE LAUNCH`, or `REMOVE`

Use `PAGE-CLEARED` for claims explicitly published on the advertiser-controlled product page. Use `PUFFERY` only for recognizable subjective or metaphorical language that does not assert a new measurable fact. Dynamic page values should normally be `VERIFY BEFORE LAUNCH` even though the source is page-cleared.

Any `REMOVE` item must be removed before delivery. If removal breaks the concept, return `BRIEF REVISION REQUIRED`.

## 6. Downstream handoff

End with only the unresolved items the storyboard or production team must know, such as required real-product demonstrations or missing approved assets. Do not solve them with invented visuals.

## Repository mode

When the script is saved for an automated pipeline, create:

- `script-v1.md` using this contract
- `script-v1.json` containing the same metadata, beats, clean read-through, timing estimate, claim audit, and unresolved handoff

The Markdown and JSON must agree on every spoken line, offer, duration, and claim status.
