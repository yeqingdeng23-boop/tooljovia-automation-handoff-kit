# Worked example: matching paths, unfinished handoff

**Hypothetical demonstration.** All paths and statuses below are synthetic. This is not a customer project, an execution log, a signoff, or an approved release.

Project reference: DEMO-AUTO-001. The example reviews records in two stages. It shows what a record comparison can establish and what remains outside it.

## Start with the declared paths

| Branch | Expected ordered path |
|---|---|
| normal | start → validate → review → queue |
| fallback | start → validate → manual → hold |
| duplicate | start → validate → dedupe → hold |

## Stage A: one pass label does not match its path

| Scenario | Branch | Supplied observed path | Supplied status | Record review |
|---|---|---|---|---|
| S1 | normal | start → validate → review → queue | pass | Matches the declared path |
| S2 | fallback | start → validate → queue | pass | Path mismatch; the pass label is insufficient |
| S3 | duplicate | No path supplied | unrun | No matching pass record |

Only one of three declared branches has a matching pass in these supplied records. The branch workbench retains two uncovered branches and a HOLD. It has not run any of them.

The associated synthetic acceptance table has three must-have holds, two failed records, two unrun records, and one requirement without a linked test. The manual-handling requirement also remains on hold: ten assumed exceptions need one hour, while only half an hour was allocated.

## Stage B: the records change; a decision is still missing

Stage B supplies matching pass records for all three paths and allocates one hour for the assumed manual handling. The branch comparison now finds three matching passes out of three.

The associated acceptance table has zero must-have holds, no failed records, one unrun record and one requirement without a linked test. The remaining gaps are:

| Requirement | Example priority | Supporting record | What remains open |
|---|---|---|---|
| R5 — Actual authorized operator signoff is recorded | should | T5 remains unrun | No actual accountable human decision |
| R6 — Client-readable file names are reviewed | could | No linked test | Filename review is not evidenced |

The example's R5 priority does not override a real project's approval policy. If the agreement requires a client or operator decision, that decision remains required even when the workbench reports zero must-have holds. Choose real project priorities according to the actual agreement.

**Handoff decision in this example: pending.** The changed synthetic records do not prove that a workflow ran in a client's environment, that credentials were connected, or that a human approved delivery.

## Apply the method to your own project

1. Start with the [blank handoff checklist](CLIENT_HANDOFF_CHECKLIST.en.md).
2. Have the responsible owner arrange authorized checks in the intended environment. Keep the actual execution evidence in the project's authorized location.
3. Enter the relevant path records in [Workflow Branch Test Coverage](https://tooljovia.com/tools/workflow-branch-test-coverage/). A supplied pass must match the declared ordered path.
4. Map the requirements and actual test statuses in [MVP Acceptance Traceability Builder](https://tooljovia.com/tools/mvp-acceptance-traceability-builder/).
5. Export and review the records. Preserve failed, unrun and uncovered work, then obtain the required owner's decision separately.

The two workbenches are separate. Transfer records manually; the example does not include automatic project loading or account history. Do not enter customer secrets into the tools or send customer records in optional feedback.

This is an example of reviewing supplied records. Nothing here establishes customer use, a time saving, payment or profit.
