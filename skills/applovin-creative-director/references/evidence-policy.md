# Evidence Policy

Use this reference when a recommendation depends on platform guidance, product claims, customer evidence, performance data, practitioner observations, or internal methods.

## Evidence levels

### A — Official

Directly supported by current AppLovin documentation, official product guidance, or verified platform specifications.

- Confidence: high for the fact actually stated by the source.
- Use: platform baseline or constraint.
- Caution: confirm recency when compliance, availability, or exact specifications matter.

### B — First-party

Supported by the advertiser's product documentation, approved claims, customer research, reviews, surveys, winning or losing creatives, sales data, or AppLovin performance data.

- Confidence: high to very high when the sample and attribution are sound.
- Use: default source for product truth and account-specific decisions.
- Caution: distinguish correlation from causation and Creative Set results from asset-level results.

### C — Practitioner

Supported by agencies, media buyers, operators, case observations, or third-party field reports.

- Confidence: medium.
- Use: `TEST PRIORITY`, not universal truth.
- Caution: record market, product, offer, date, and test conditions when known.

### D — Internal hypothesis

Derived from creative reasoning, analogy, the team's methods, or an untested combination.

- Confidence: unknown until tested.
- Use: `EXPERIMENT`.
- Caution: state the causal belief and the result that would disconfirm it.

## Conflict rule

Resolve conflicts using context, not a blind universal ranking. For account decisions, the normal priority is:

1. valid first-party performance evidence from a comparable test
2. current official AppLovin guidance or hard specification
3. strong first-party customer and product evidence
4. practitioner insight
5. internal hypothesis

Hard platform constraints always override creative preference. Do not let a small or confounded first-party test overrule a reliable official constraint. State material disagreements and recommend a test when neither source settles the question.

## Claim handling

For each material claim, record:

- claim
- evidence level
- source or source type
- confidence
- status: `USE`, `TEST PRIORITY`, `EXPERIMENT`, `CLAIM REQUIRED`, or `PROOF GAP`

Do not convert an observed pattern into a causal rule. Do not use a third-party statistic merely because it sounds precise. Never cite a source as supporting a stronger statement than it actually makes.

## Testing rule

Translate uncertain guidance into a falsifiable test:

- variable being changed
- what remains controlled
- expected mechanism
- primary success metric
- guardrail metric
- decision threshold or review rule

When reporting is aggregated above the individual asset, acknowledge the attribution limit and design the Creative Set or naming structure accordingly.
