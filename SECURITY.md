# Security and Evidence Publication Policy

This is a public portfolio repository. It must not contain live credentials, private customer data, production secrets, proprietary client source code, or unnecessary turnkey implementations.

## Never commit

- API keys or bearer tokens
- OAuth client secrets or access/refresh tokens
- n8n credential IDs tied to a private instance
- private webhook URLs
- Supabase service-role keys
- database passwords or connection strings containing secrets
- personal customer/patient data
- private document or spreadsheet IDs when they are not intentionally public
- proprietary client source code

## Default portfolio policy: evidence-first, not turnkey

For most portfolio systems, publish enough technical evidence to make the engineering inspectable without publishing the complete reusable deployment package.

Preferred public evidence includes:

- architecture and workflow/node maps
- business-routing rules and data contracts
- screenshots and execution/test evidence
- selected sanitized node/configuration excerpts
- reliability, fallback, deduplication, audit, and human-review decisions
- setup assumptions without private account details

Complete reusable workflow exports are **withheld by default**.

## Exception: intentionally open demo projects

A complete workflow export may be published when the project is deliberately an open demo/sample and reuse is part of the purpose of the repository.

The WhatsApp AI Order Processor is such an exception: it is explicitly labelled **DEMO MODE**, uses mocked/simulated external integrations, and is intentionally packaged as an importable sample.

## If a demo workflow export is published

Before publishing an n8n export:

1. remove the `credentials` objects
2. remove or replace webhook identifiers
3. replace private resource IDs with clear placeholders
4. remove pinned data that contains real names, email addresses, phone numbers, or business records
5. remove private instance metadata
6. inspect Code/HTTP Request nodes for embedded tokens, passwords, endpoints, or headers
7. verify that screenshots do not reveal secrets in side panels, URLs, browser tabs, or execution data
8. explicitly label whether integrations are mocked, simulated, or live

## Data policy

Portfolio demonstrations use synthetic or deliberately non-sensitive test data unless a public source is explicitly documented.

## Commercial work

Client or employer source code remains private unless there is explicit permission to publish it. Commercial work such as YTRanker is documented as a case study rather than copied into this repository.
