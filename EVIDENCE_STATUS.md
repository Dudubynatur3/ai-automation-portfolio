# Evidence Status Register

This register separates what is directly published in this repository from evidence that exists in prior project records but has not yet been exported into a public artifact.

| Project | Documentation | Importable workflow / blueprint | Visual evidence | Classification |
|---|---|---|---|---|
| AI Agency Lead Capture & Qualification | README + detailed `TESTING.md` published | Published as portfolio-safe n8n JSON | Original execution visuals recovered, pending safe public image publication | Client-style project, synthetic data |
| MedFlow Intake OS | README + recovered `IMPLEMENTATION_NOTES.md` published | Detailed Make.com/Jotform/Airtable design records recovered; public account-specific export not yet published | Recovered project package and visual assets still being curated | Client-style project, synthetic data |
| Cupid Errands Intelligent Email Routing | README + detailed `ARCHITECTURE.md` published | Architecture and implementation logic recovered; public n8n export not yet published | Detailed original architecture diagram recovered, pending safe public image publication | Structured AI automation project |
| RAG & AI Agent Workflows | README + `INGESTION_AND_RETRIEVAL.md` published | Training workflow configuration documented; public export not yet published | Training screenshots/notes recovered | Training implementation |
| WhatsApp / Chatwoot CRM Automation | Published | Development evidence recovered; no claim of a single production export | Prior development evidence recovered | Independent portfolio/development implementation |
| AI-Assisted Support with Human Review | Published | Workflow pattern documented; export not yet published | Documentation evidence recovered | Independent portfolio workflow pattern |
| Self-Hosted n8n Platform | Published | Infrastructure architecture documented | Deployment/walkthrough evidence exists in prior project records | Independent infrastructure implementation |
| WhatsApp AI Order Processor | Separate standalone repository | Importable demo workflow already published | Workflow screenshot already published | Portfolio demo, mocked external integrations |
| YTRanker | Public case study only; source remains private | Not applicable | Commercial evidence represented through scope, testing metrics, handover, and client feedback | Commercial production experience |

## AI Agency export note

The public AI Agency workflow is a **portfolio-safe adaptation** of the recovered n8n export, not a byte-for-byte copy.

Security-sensitive references were removed, including:

- credential IDs
- private Google Sheet identifiers and cached URLs
- webhook IDs
- n8n instance identifier

There is also one presentation-safety refinement: the public customer acknowledgement does **not** expose the internal lead status. The recovered workflow record contained an email template that included the status, while the project presentation material described that status as internal. The public version follows the intended internal-status design and this difference is documented here rather than silently presented as an exact export.

## Cloud portfolio audit

The cloud side has also been reviewed for authorship quality.

See [`CLOUD_REPOSITORY_AUDIT.md`](./CLOUD_REPOSITORY_AUDIT.md).

Current portfolio decisions:

- `3-Tier-MERN-App` is a fork with no personal implementation work and should not be used as personal portfolio evidence.
- `Azure-Terraform-Project` is a collaborative Cloud Advisory group project and should not be presented as independently authored.
- stronger original cloud evidence includes `aws-3tier-terraform-nextjs`, `gcp-exercise`, `epicbook-fullstack`, and `dev-onboarding-automation`.

## Publication rule

A project is never labelled as production simply because it was successfully executed in a portfolio or training environment. Commercial production evidence, independent portfolio builds, collaborative training work, and structured training implementations remain clearly separated.
