# SNS growth skill verification

## Setup

Three creator-growth prompts were run without the skill before initial authoring. The revised skill was exercised on all six eval cases; retention-curve and TikTok transfer cases were also compared with no-skill controls. These are qualitative single-run tests, not a statistically powered benchmark.

## Audit changes

- Condensed `SKILL.md` from 790 to 465 words while retaining its core loop, source limits, and response contract.
- Made the source-specific five-second video promise test explicit.
- Clarified that ratios may be calculated from available counts; require numerator, denominator, and period, and don't invent unavailable data.
- Added a Threads text-only eval so non-video advice is checked against YouTube-only retention guidance.
- Added a retention-curve case and a TikTok timing/volume-transfer case to test source-scope boundaries.

## Final regression results

| Scenario | Result | Evidence observed |
|---|---|---|
| New creator stuck preparing | Pass | Sustainable 30-day cadence, starts with current tools, one-change learning loop, and no growth guarantee. |
| Weak 30-second retention | Pass | Explicitly tests the five-second promise delivery, changes the intro, compares similar posts, and avoids treating one result as causal. |
| Part-time solo creator | Pass | Preserves two posts per month, captures immediate and later feedback, uses platform metrics, and shares peer learnings with consent. |
| Threads text-only follow conversion | Pass | Uses follows ÷ profile views with a stated review period, notes limits on post-level attribution, and does not apply video-retention thresholds. |
| YouTube retention-curve segment | Pass | Located the specific 0:14–0:38 drop, changed only that story segment, and preserved the already-working first five seconds. |
| TikTok timing and 100-video transfer | Pass | Treated five seconds as a YouTube heuristic, adapted to the 1.5-second TikTok drop, and described 100 videos as practice rather than an algorithm quota. |

No-skill controls also produced competent answers, including for the retention-curve and TikTok cases. These runs confirm that the revised skill handles the tested boundaries, but they do not establish a statistically reliable skill uplift or predict growth outcomes.

`evals.json` contains six reusable prompts and observable criteria. JSON syntax was validated with `jq empty`; `SKILL.md` is 465 words.
