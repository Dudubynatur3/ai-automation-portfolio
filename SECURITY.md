# Security and Sanitization Policy

This is a public portfolio repository. It must not contain live credentials, private customer data, or production secrets.

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

## Public workflow exports

Before publishing an n8n export:

1. remove the `credentials` objects
2. remove or replace webhook identifiers
3. replace private resource IDs with clear placeholders
4. remove pinned data that contains real names, email addresses, phone numbers, or business records
5. remove private instance metadata
6. inspect Code/HTTP Request nodes for embedded tokens, passwords, endpoints, or headers
7. verify that screenshots do not reveal secrets in side panels, URLs, browser tabs, or execution data

## Data policy

Portfolio demonstrations use synthetic or deliberately non-sensitive test data unless a public source is explicitly documented.

## Commercial work

Client or employer source code remains private unless there is explicit permission to publish it. Commercial work such as YTRanker is documented as a case study rather than copied into this repository.
