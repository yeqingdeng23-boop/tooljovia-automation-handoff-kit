# Workflow branch test coverage

Declared branches: 3
Branches with a matching pass: 1
Matching-pass coverage (%): 33.333333333333333333…
Uncovered branches: 2
Review gate: HOLD

Path comparison: Exact case-sensitive ordered node labels; &gt; is the separator

## Branch coverage

| Branch | Expected path | Matching-pass scenario IDs | Finding |
| --- | --- | --- | --- |
| normal | start&gt;validate&gt;review&gt;queue | S1 | Covered by supplied matching pass |
| fallback | start&gt;validate&gt;manual&gt;hold |  | No matching pass supplied |
| duplicate | start&gt;validate&gt;dedupe&gt;hold |  | No matching pass supplied |

## Scenario findings

| Scenario | Branch | Observed path | Declared status | Finding |
| --- | --- | --- | --- | --- |
| S1 | normal | start&gt;validate&gt;review&gt;queue | pass | Recorded matching pass |
| S2 | fallback | start&gt;validate&gt;queue | pass | Observed path differs from expected branch |
| S3 | duplicate |  | unrun | Not executed |

## Entered source — Branches

| branch\_id | expected\_path |
| --- | --- |
| normal | start&gt;validate&gt;review&gt;queue |
| fallback | start&gt;validate&gt;manual&gt;hold |
| duplicate | start&gt;validate&gt;dedupe&gt;hold |

## Entered source — Scenarios

| scenario\_id | branch\_id | observed\_path | status |
| --- | --- | --- | --- |
| S1 | normal | start&gt;validate&gt;review&gt;queue | pass |
| S2 | fallback | start&gt;validate&gt;queue | pass |
| S3 | duplicate |  | unrun |

Coverage is evidence in entered fixtures, not execution of a real workflow. Conditions are not parsed or evaluated; repeated nodes are permitted as explicit path visits. A matching pass counts coverage, while failed/unrun/unknown/mismatched records still hold the review. Missing scenarios are not successful branches.

Only supplied declarations are reconciled locally. No AI, vendor account, network request, upload, execution, persistence, source-truth verification, approval, payment, publication or customer/income forecast occurs. Inspect source records and the real external workflow before acting.