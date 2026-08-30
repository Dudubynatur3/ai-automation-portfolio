# Testing Evidence

## Objective

Validate that each intended business route produces the correct internal status and downstream actions.

## Tested routing outcomes

The workflow was tested across five final outcomes:

1. **Priority Plus**
2. **Priority**
3. **Default**
4. **Warm**
5. **Cold**

## Test logic

The first Switch node classifies lead timing:

- `Immediately / This Week` → Hot
- `Later This Month` → Warm
- `Just Researching` → Cold

Only Hot leads continue to the budget Switch:

- `1,000,000 and above` → Priority Plus
- `500,000 - 999,999` → Priority
- lower Hot budget route → Default

Each route assigns the final internal status before the record is written to Google Sheets and the acknowledgement path is triggered.

## Representative validation case

A synthetic lead was submitted with:

- Service: AI Automation
- Timeline: Immediately / This Week
- Budget: 1,000,000 and above

Expected result:

```text
Form submission
→ Hot timeline branch
→ Priority Plus budget branch
→ Status = Priority Plus
→ Append to Google Sheets
→ Send acknowledgement email
```

The execution matched the expected route.

## Why deterministic routing was used

The form uses controlled dropdown values. For that reason, deterministic Switch-node logic is more transparent and testable than using an LLM for classification.

This keeps the workflow:

- easier to audit
- cheaper to run
- more predictable
- simpler to troubleshoot

## Evidence boundary

The project is a synthetic-data portfolio implementation. The tests validate workflow logic and routing behavior, not production-scale throughput or enterprise reliability.
