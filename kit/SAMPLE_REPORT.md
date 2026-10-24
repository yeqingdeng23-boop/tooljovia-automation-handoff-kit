# Demonstration: a project that looks affordable but is not ready to hand over

**Hypothetical demonstration. All amounts are USD. The inputs, paths and statuses are synthetic. No customer project, live workflow execution, payment, time saving or release approval is evidenced.** This worked example reviews synthetic records; it does not establish live workflow execution or an authorized human approval.

Project reference: DEMO-AUTO-001  
Planning period: one month per hypothetical client  
Expected output: a cost worksheet, branch-record review, and traceable handoff record

## The commercial assumptions
A hypothetical service is priced at $150 per client per month. Delivery and review take an estimated 5 hours per client, valued at $20 per hour. Workflow cash cost is budgeted at $20 per client, payment fees at 3%, and studio overhead at $100 per month. Four planned clients use the full 20 delivery hours available.

The arithmetic leaves $25.50 per client after valuing delivery labor. Four clients leave only **$2 of modeled monthly surplus after overhead and owner labor**. This is not observed profit; acquisition, refunds, tax and additional work have not been established.

## The hidden delivery gap
The hypothetical workflow receives 100 jobs. With an assumed 20% initial failure rate, 20 jobs fail initially. Reserving up to two additional attempts for each creates a maximum 40-retry allowance. If half the initially failed jobs are assumed to recover, 10 exceptions remain.

At 6 minutes per exception, those exceptions require one hour of manual handling. Variant A allocates only half an hour, so five expected exceptions exceed the allocated capacity. The full handling budget remains $40: $20 cash plus $20 of labor. A budget for all work does not prove that enough time has been assigned to do it.

## The evidence gap
Three branch records are supplied in variant A. Only one matches its expected ordered path with a pass status. One is labelled pass but follows a different path; another is unrun. A pass label alone does not establish the expected path.

The acceptance worksheet consequently retains three must-have items on hold, two failed tests, two unrun tests, and one uncovered requirement.

## What changes in variant B
Variant B changes the allocated exception time to one hour and supplies matching synthetic records for all three branches. It illustrates how the record checks change.

**An actual authorized human signoff still remains unrun.** The optional filename review is also uncovered. A zero must-hold count must not be presented as overall release approval.

## Carrying the figures into the quote
Transfer only the $20 workflow cash budget into the pricing tool's variable cash field. The 5 delivery hours already include one hour of exception handling. Transferring the labor-inclusive $40 would count that exception labor twice.

## Review before any real handoff
- Replace assumptions with period-specific observed records where available.
- Preserve failed, unrun and uncovered work.
- Identify actual execution evidence and the authorized decision owner.
- Reconcile actual delivery, support, acquisition, refund and tax costs.
- Keep forecasts separate from actual client acceptance, payment and savings.

Use sample-inputs.json to locate each exact input field and the supplied records. sample-expected.json contains the independent expected figures. The editable blank worksheets are separate from the example.


