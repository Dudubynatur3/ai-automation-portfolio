# MedFlow Implementation Notes

## Scope

MedFlow Intake OS is a client-style portfolio implementation built with synthetic healthcare data. Its purpose is to demonstrate structured intake automation, data integrity, routing controls, auditability, and human handoff.

## Verified system flow

```text
Jotform
→ Make.com
→ Airtable
→ Google Sheets
→ Gmail / Outlook
→ Google Calendar
```

## Airtable data model recovered from the original project package

The original project documentation identifies four primary Airtable tables:

- `Patients`
- `Intakes`
- `Routing_Log`
- `Staff`

Public portfolio documentation uses this recovered source rather than the later six-table summary that appeared in career notes.

## Intake processing

The intake form collects structured information and passes it to Make.com for validation and downstream processing.

Key controls include:

- required-field validation
- normalized field mapping
- duplicate checking before patient creation
- consent-aware routing
- urgency-aware routing
- manual review when the automated path should not decide independently

## Duplicate checking

The documented matching sequence uses email first, with phone as a fallback identity check.

```text
Search by email
→ match found: update / reuse existing patient
→ no email match: check phone
→ no match: create patient record
```

The design goal is to avoid creating unnecessary duplicate patient identities before writing the intake event.

## Routing and notifications

The workflow separates operational routing from the form itself. Jotform can shape the intake experience, while Make.com determines downstream actions based on the submitted data.

Notifications are designed around minimum necessary information rather than copying the full intake record into every destination.

## Audit design

The `Routing_Log` is treated as an append-oriented audit surface.

It records enough information to understand:

- what happened
- which route was selected
- when processing occurred
- whether manual intervention was required

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
- Airtable relational workflow design
- cross-system field mapping
- duplicate prevention
- conditional routing
- notification design
- manual escalation
- audit logging
- privacy-conscious testing
