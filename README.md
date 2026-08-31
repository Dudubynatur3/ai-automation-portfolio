# AI Automation Portfolio

A curated collection of automation and AI workflow projects by **Aduroja Akintade**, focused on reliable business-process automation, integrations, AI-assisted workflows, and the infrastructure that supports them.

This repository complements my Cloud/DevOps work by making the automation side of my engineering portfolio inspectable through business context, architecture, testing evidence, screenshots, routing logic, technical decisions, and selected sanitized implementation evidence.

## Portfolio principles

- **Business problem first.** Each project explains the operational problem before the tooling.
- **Evidence over claims.** Architecture, execution evidence, test records, screenshots, routing logic, and technical decisions are used to demonstrate the work.
- **Evidence-first, not turnkey.** Complete reusable workflow exports are not the default public artifact. Full exports are reserved for intentionally open demo/sample projects.
- **Clear implementation status.** Commercial, independent portfolio, client-style synthetic-data, and training implementations are labelled separately.
- **Security by default.** Credentials, production webhook URLs, private document IDs, customer data, secrets, and proprietary implementation details are excluded.
- **Reliability matters.** Fallbacks, duplicate protection, human review, auditability, testing, documentation, and handover are treated as part of the system design.

## Featured automation systems

| Project | Focus | Stack | Public evidence |
|---|---|---|---|
| [AI Agency Lead Capture & Qualification](./01-ai-agency-lead-qualification/) | Lead capture, deterministic qualification, CRM logging, acknowledgement | n8n, Google Sheets, Gmail | Architecture, routing logic and five tested outcomes |
| [MedFlow Intake OS](./02-medflow-intake-os/) | Structured intake, deduplication, linked records, routing, audit logging | Jotform, Make.com, Airtable, Google Sheets | Six-table relational model and implementation evidence |
| [Cupid Errands Intelligent Email Routing](./03-cupid-intelligent-email-routing/) | AI intent classification, duplicate protection, department routing | n8n, OpenRouter, Email, Slack | Architecture and routing evidence |
| [RAG & AI Agent Workflows](./04-rag-ai-agent-workflows/) | Document ingestion, embeddings, vector retrieval, agent memory | n8n, OpenRouter, OpenAI Embeddings, Supabase | Training implementation evidence |
| [WhatsApp / Chatwoot CRM Automation](./05-whatsapp-chatwoot-crm/) | Messaging ingestion, webhook processing, CRM-style logging | n8n, Chatwoot, WhatsApp, Google Sheets, Docker | Development and architecture evidence |
| [AI-Assisted Support with Human Review](./06-ai-support-human-review/) | Context retrieval, AI drafting, approval boundary, CRM follow-up | LLM workflow, Gmail, HubSpot | Human-in-the-loop workflow evidence |
| [Self-Hosted n8n Platform](./07-self-hosted-n8n-platform/) | Automation platform hosting and operational infrastructure | Docker, PostgreSQL, Redis, Traefik, HTTPS | Infrastructure and deployment evidence |

## Open demo repository

### WhatsApp AI Order Processor

A separate **DEMO MODE** n8n project demonstrating WhatsApp order intake, AI-assisted order parsing, payment-flow design, order logging and fulfilment notification using mocked/simulated external integrations.

**Repository:** https://github.com/Dudubynatur3/whatsapp-order-processor

This is intentionally published as a reusable sample. The other portfolio systems prioritize inspectable evidence rather than complete copy-and-deploy exports.

## Commercial production case study

### YTRanker SaaS Platform Engineering

YTRanker is represented as a case study because the production source code is private.

Validated scope includes:

- React, Supabase and Vercel production platform work
- Gmail OAuth, Telegram, WhatsApp, OpenRouter, Anthropic and external integrations
- AI-provider migration to OpenRouter
- role-based permissions and operational workflow controls
- regression testing across **6 user roles**
- validation of **40+ feature branches** before handover
- full technical handover documentation

[Read the public YTRanker case study](./commercial-case-studies/ytranker.md)

Public Upwork profile for work-history verification: https://www.upwork.com/freelancers/~01c8ba1b4d2162d9f1?mp_source=share

## Related Cloud / DevOps work

My automation work is backed by hands-on engineering across Terraform, GCP, AWS, Azure, Docker, Kubernetes, GitHub Actions, Ansible, Linux, IAM and cloud networking.

See all public repositories: https://github.com/Dudubynatur3

## Contact

- Portfolio: https://aduroja-akintade.lovable.app
- LinkedIn: https://www.linkedin.com/in/akintade-aduroja
- GitHub: https://github.com/Dudubynatur3
- Upwork: https://www.upwork.com/freelancers/~01c8ba1b4d2162d9f1?mp_source=share
- Location: Kokkola, Finland

---

**Note:** Public evidence is intentionally sanitized and scoped. A project being inspectable does not mean the complete reusable implementation is published.