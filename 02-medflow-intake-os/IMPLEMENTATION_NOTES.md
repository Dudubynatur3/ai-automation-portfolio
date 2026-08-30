# MedFlow Implementation Notes

## Scope

MedFlow Intake OS is a client-style portfolio implementation built with synthetic healthcare data. Its purpose is to demonstrate structured intake automation, data integrity, routing controls, auditability, case handling, task generation, and human handoff.

## Verified system flow

```text
Jotform
→ Make.com
→ Airtable
→ Google Sheets
→ Gmail / Outlook
→ Google Calendar
```

## Airtable data model, re-verified from the live base

Direct inspection of the connected MedFlow Airtable base confirms **six tables**:

- `Patients`
- `Intakes`
- `Cases`
- `Tasks`
- `Routing_Log`
- `Staff`

An earlier recovered documentation snapshot referenced four core tables, but the connected Airtable implementation is the stronger source of truth and confirms that `Cases` and `Tasks` are part of the implemented data model.

See [`DATA_MODEL.md`](./DATA_MODEL.md) for the relational structure and representative fields.

## Intake processing

The intake form collects structured information and passes it to Make.com for validation and downstream processing.

Key controls include:

- required-field validation
- normalized field mapping
- duplicate checking before patient creation
- patient create/update
- intake creation
- case creation
- task generation
- consent-aware routing
- urgency-aware routing
- manual review where the automated path should not decide independently

## Duplicate checking

The documented matching sequence uses email first, with normalized phone available as a fallback identity check.

```text
Search by email
→ match found: update / reuse existing patient
→ no email match: check phone
→ no match: create patient record
```

The design goal is to avoid creating unnecessary duplicate patient identities before writing the intake event.

## Case and task handling

The live Airtable schema separates operational handling from intake data:

- `Cases` tracks route, priority, status, patient, source intake, staff owner, timestamps, notes, and related tasks.
- `Tasks` tracks follow-up work, due/completed timestamps, status, notes, parent case, and assigned staff.

This separation makes operational ownership and follow-up work inspectable rather than hiding everything in a single record.

## Routing and notifications

The workflow separates operational routing from the form itself. Jotform can shape the intake experience, while Make.com determines downstream actions based on the submitted data.

Notifications are designed around minimum necessary information rather than copying the full intake record into every destination.

## Audit design

The `Routing_Log` is treated as an append-oriented audit surface.

The live schema includes fields for:

- routing result
- route
- priority
- routed timestamp
- action taken
- error message
- scenario run ID
- masked patient email
- patient phone last four digits
- consent status
- deduplication result
- linked intake
- assigned staff

Google Sheets provides an additional portfolio-visible audit / backup layer.

## Human-in-the-loop boundary

The system intentionally keeps a human handoff path for cases where automation should not make an unsupported decision.

That design choice is important because the project demonstrates workflow engineering, not autonomous clinical decision-making.

## Privacy boundary

- Synthetic data only
- No real patient data in the public portfolio
- No claim of HIPAA certification or production clinical compliance
- Credentials, private account identifiers, and sensitive endpoints are excluded

## What this project demonstrates

- Jotform form design
- Make.com orchestration
- six-table Airtable relational workflow design
- cross-system field mapping
- duplicate prevention
- patient/intake separation
- case creation
- task generation and assignment
- consent-aware conditional routing
- notification design
- manual escalation
- audit logging
- privacy-conscious testing
