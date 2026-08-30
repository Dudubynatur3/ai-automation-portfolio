# Evidence Status Register

This register separates what is directly published in this repository from evidence that exists in prior project records but has not been exported into a public artifact.

| Project | Documentation | Public implementation evidence | Visual evidence | Classification |
|---|---|---|---|---|
| AI Agency Lead Capture & Qualification | README + detailed `TESTING.md` published | Architecture, routing rules, data contract and test evidence published; complete reusable n8n export intentionally withheld from current branch | Original execution visuals recovered, pending safe public image publication | Client-style project, synthetic data |
| MedFlow Intake OS | README + recovered `IMPLEMENTATION_NOTES.md` + data model evidence published | Detailed Make.com/Jotform/Airtable design records recovered; complete account-specific scenario/export not published | Recovered project package and visual assets still being curated | Client-style project, synthetic data |
| Cupid Errands Intelligent Email Routing | README + detailed `ARCHITECTURE.md` published | Architecture and implementation logic recovered; complete reusable n8n export not published | Detailed original architecture diagram recovered, pending safe public image publication | Structured AI automation project |
| RAG & AI Agent Workflows | README + `INGESTION_AND_RETRIEVAL.md` published | Training workflow configuration documented; complete reusable export not published | Training screenshots/notes recovered | Training implementation |
| WhatsApp / Chatwoot CRM Automation | Published | Development architecture and implementation evidence documented; no claim of a turnkey production export | Prior development evidence recovered | Independent portfolio/development implementation |
| AI-Assisted Support with Human Review | Published | Workflow pattern documented; complete reusable export not published | Documentation evidence recovered | Independent portfolio workflow pattern |
| Self-Hosted n8n Platform | Published | Infrastructure architecture documented | Deployment/walkthrough evidence exists in prior project records | Independent infrastructure implementation |
| WhatsApp AI Order Processor | Separate standalone repository | **Intentionally open demo:** importable sample workflow published with mocked/simulated external integrations | Workflow screenshot already published | Portfolio demo, mocked external integrations |
| YTRanker | Public case study only; source remains private | Not applicable | Commercial evidence represented through scope, testing metrics, handover, and client feedback | Commercial production experience |

## Evidence-first publication rule

The purpose of the public portfolio is to prove engineering ability, not to publish a complete copy-and-deploy package for every project.

Default public evidence can include:

- business problem and architecture
- node/workflow maps
- routing rules and data contracts
- screenshots and test results
- selected sanitized implementation excerpts
- reliability, security, fallback, and handoff decisions

Complete reusable workflow exports are withheld by default. They are published only when a project is deliberately designed as an open demo/sample, as with the WhatsApp AI Order Processor.

## AI Agency evidence note

The AI Agency project was recovered from an n8n implementation and has enough evidence to substantiate the workflow design and testing without keeping the full reusable export on the current public branch.

The public evidence preserves:

- the exact deterministic timeline/budget routing model
- five tested final outcomes
- downstream Google Sheets persistence
- Gmail acknowledgement behaviour
- the distinction between internal status and customer-facing communication

The full reusable n8n export is intentionally not part of the current portfolio surface.

## Cloud portfolio audit

The cloud side has also been reviewed for authorship quality.

See [`CLOUD_REPOSITORY_AUDIT.md`](./CLOUD_REPOSITORY_AUDIT.md).

Current portfolio decisions:

- `3-Tier-MERN-App` is a fork with no personal implementation work and should not be used as personal portfolio evidence.
- `Azure-Terraform-Project` is a collaborative Cloud Advisory group project and should not be presented as independently authored.
- stronger original cloud evidence includes `aws-3tier-terraform-nextjs`, `gcp-exercise`, `epicbook-fullstack`, and `dev-onboarding-automation`.

## Classification rule

A project is never labelled as production simply because it was successfully executed in a portfolio or training environment. Commercial production evidence, independent portfolio builds, collaborative training work, and structured training implementations remain clearly separated.
