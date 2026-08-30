# Evidence Status Register

This register separates what is directly published in this repository from evidence that exists in prior project records but has not yet been exported into a public artifact.

| Project | Documentation | Importable workflow / blueprint | Visual evidence | Classification |
|---|---|---|---|---|
| AI Agency Lead Capture & Qualification | Published | Published as portfolio-safe n8n JSON | Recovered, pending public image upload | Client-style project, synthetic data |
| MedFlow Intake OS | Published | Detailed Make.com/Jotform/Airtable design records recovered; public executable export not yet published | Recovered project documentation, visual assets still being curated | Client-style project, synthetic data |
| Cupid Errands Intelligent Email Routing | Published | Architecture and implementation logic recovered; public n8n export not yet published | Detailed architecture diagram recovered, pending public image upload | Structured AI automation project |
| RAG & AI Agent Workflows | Published | Training workflow configuration documented; public export not yet published | Training screenshots/notes recovered | Training implementation |
| WhatsApp / Chatwoot CRM Automation | Published | Development evidence recovered; no claim of a single production export | Prior development evidence recovered | Independent portfolio/development implementation |
| AI-Assisted Support with Human Review | Published | Workflow pattern documented; export not yet published | Documentation evidence recovered | Independent portfolio workflow pattern |
| Self-Hosted n8n Platform | Published | Infrastructure architecture documented | Deployment/walkthrough evidence exists in prior project records | Independent infrastructure implementation |
| WhatsApp AI Order Processor | Separate standalone repository | Importable demo workflow already published | Workflow screenshot already published | Portfolio demo, mocked external integrations |

## Important AI Agency export note

The public AI Agency workflow is a **portfolio-safe adaptation** of the recovered n8n export, not a byte-for-byte copy.

Security-sensitive references were removed, including:

- credential IDs
- private Google Sheet identifiers and cached URLs
- webhook IDs
- n8n instance identifier

There is also one presentation-safety refinement: the public customer acknowledgement does **not** expose the internal lead status. The recovered workflow record contained an email template that included the status, while the project presentation material described that status as internal. The public version follows the intended internal-status design and this difference is documented here rather than silently presented as an exact export.

## Publication rule

A project is never labelled as production simply because it was successfully executed in a portfolio or training environment. Commercial production evidence, independent portfolio builds, and structured training implementations remain clearly separated.
