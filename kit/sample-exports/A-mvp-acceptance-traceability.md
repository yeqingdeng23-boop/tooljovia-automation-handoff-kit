# MVP acceptance traceability

Must-have requirements on hold: 3
Uncovered requirements: 1
Failed tests: 2
Unrun tests: 2

| Requirement | Description | Priority | Test IDs | Covered | Failed | Unrun | Entered tests ready |
| --- | --- | --- | --- | --- | --- | --- | --- |
| R1 | Normal branch entered path matches spec | must | T1 | true | 0 | 0 | true |
| R2 | Fallback branch entered path matches spec | must | T2 | true | 1 | 0 | false |
| R3 | Duplicate branch has a matching-pass fixture | must | T3 | true | 0 | 1 | false |
| R4 | Exception demand fits allocated handling hours | must | T4 | true | 1 | 0 | false |
| R5 | Actual authorized operator signoff is recorded | should | T5 | true | 0 | 1 | false |
| R6 | Client-readable file names are reviewed | could |  | false | 0 | 0 | false |

## Test handoff
| Test | Requirement | Procedure | Expected | Observed status |
| --- | --- | --- | --- | --- |
| T1 | R1 | Compare synthetic S1 with normal path | Exact declared ordered path | pass |
| T2 | R2 | Compare synthetic S2 with fallback path | Exact declared ordered path | fail |
| T3 | R3 | Inspect synthetic S3 record | Matching-pass fixture entered | unrun |
| T4 | R4 | Compare 10 exceptions with entered capacity | Capacity is at least 10 exceptions | fail |
| T5 | R5 | Inspect actual authorized signoff record | An accountable human decision exists | unrun |

A requirement is ready only when at least one linked test is entered and every linked status is pass. Only must-priority holds are counted in the headline; review should/could requirements separately. These statuses are your declarations, not tests run by this workbench or proof that the app is safe or market-validated.