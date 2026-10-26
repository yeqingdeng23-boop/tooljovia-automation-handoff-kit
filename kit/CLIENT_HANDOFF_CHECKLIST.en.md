# Client Project Delivery Checklist

Use this working checklist to record what was checked, what remains open, and who decides whether the project can be handed over. A completed document is not a substitute for actual execution records or the client's decision.

Project reference:  
Version and date:  
Prepared by / role:  
Client decision owner:  
Scope and agreed exclusions:

## 1. Agree on the environment and responsibilities

| Check | Owner | Status | Record or next action |
|---|---|---|---|
| Identify the exact workflow version and included deliverables. | | Not checked | |
| Identify the client's intended environment and who manages it. | | Not checked | |
| Name the owner of each required service account and permission. | | Not checked | |
| Have the authorized account owner complete any required connection or consent. | | Not checked | |
| Agree who pays for development tests, retries and ongoing use. | | Not checked | |
| Agree what must be checked again when moving from a development environment. | | Not checked | |

Record an account role or reference, not a password, API key, token, private connection string, or recovery code. Do not put customer records or secrets into this checklist or optional feedback.

## 2. Record checks in the intended environment

Plan any live tests with the responsible owner. Use authorized, harmless test data and an agreed cost limit. This checklist does not run tests, connect accounts, or prove that a connection works.

| Test ID | Environment / version | Expected behavior | Observed behavior | Status | Evidence reference | Performed by / date |
|---|---|---|---|---|---|---|
| | | | | Unrun | | |

Keep evidence in the project's authorized location. A reference can identify an execution record, review note or approved screenshot; it does not need to contain customer data. A successful check under the developer's account does not establish that the client's intended environment passed.

Use **Pass**, **Fail** and **Unrun** consistently. If something was only discussed or inspected, say so. Do not mark a live behavior as passed because a plan, fixture or document exists.

## 3. Review normal and exception paths

| Branch | Expected ordered path | Relevant test IDs | Actual result / gap | Next action and owner |
|---|---|---|---|---|
| Normal task | | | Unrun | |
| Failure or manual fallback | | | Unrun | |
| Duplicate or repeated task, if relevant | | | Unrun | |
| Other agreed path | | | Unrun | |

Choose branches that belong to the agreed scope. A record marked Pass must also describe the expected path. Preserve mismatches, failed tests and paths that were not run.

Optional: use ToolJovia's [Workflow Branch Test Coverage](https://tooljovia.com/tools/workflow-branch-test-coverage/) to compare the path records you enter. It does not execute the workflow or verify that your records are true.

## 4. Connect the requirements to the evidence

| Requirement | Required for handoff? | Supporting test IDs | Status and gap | Owner / next action |
|---|---|---|---|---|
| Agreed normal behavior | | | Not reviewed | |
| Agreed failure and manual handling | | | Not reviewed | |
| Checks in the client's intended environment | | | Not reviewed | |
| Operating instructions and support responsibilities | | | Not reviewed | |
| Required client or operator decision | | | Not recorded | |

Optional: use ToolJovia's [MVP Acceptance Traceability Builder](https://tooljovia.com/tools/mvp-acceptance-traceability-builder/) to organize requirements and supplied test statuses. Set priorities according to the actual agreement. A zero must-hold count does not create an approval or remove an independently required human decision.

## 5. Name the operating owner

| Responsibility | Owner / role | Where the instructions are kept | Review trigger |
|---|---|---|---|
| Monitor normal runs and usage costs | | | |
| Review failures and decide whether to retry | | | |
| Handle unresolved work manually | | | |
| Maintain account access and renew permissions | | | |
| Review changes and use the agreed rollback procedure | | | |
| Receive support requests within the agreed scope | | | |

State the agreed support scope and hours. If handling time or capacity is unknown, leave it unknown and name the next measurement. Tool output is not a commitment by a person to perform this work.

## 6. Record the decision separately

Current decision: Pending / Accepted / Accepted with named conditions / Rejected  
Decision owner and role:  
Decision date and evidence reference:  
Open conditions and their owners:  
Next review date:

Keep the failed, unrun and uncovered work with the handoff. The decision owner must assess whether the supplied evidence and open conditions meet the actual agreement.

ToolJovia's workbenches process the records you enter in your browser. They do not migrate credentials, execute live automation, inspect private accounts, approve a release, or establish a customer's acceptance. Keep the actual evidence and decision in the project's authorized records.
