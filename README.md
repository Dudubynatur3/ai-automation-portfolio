# AI Automation Portfolio

A curated collection of automation and AI workflow projects by **Aduroja Akintade**, focused on reliable business-process automation, integrations, AI-assisted workflows, and the infrastructure that supports them.

This repository complements my Cloud/DevOps repositories by documenting the automation side of my engineering work in an inspectable format: business problem, system architecture, implementation decisions, testing evidence, and sanitized workflow artifacts where available.

## Portfolio principles

- **Business problem first.** Each project explains the operational problem before the tooling.
- **Evidence over claims.** Tested routes, workflow exports, architecture diagrams, screenshots, and implementation notes are included where available.
- **Clear implementation status.** Commercial, independent portfolio, client-style synthetic-data, and training implementations are labelled separately.
- **Security by default.** Credentials, production webhook URLs, private document IDs, customer data, and secrets are removed from public artifacts.
- **Reliability matters.** Routing rules, fallbacks, duplicate protection, human review, error handling, and operational handoff are treated as part of the system design.

## Featured automation systems

| Project | Focus | Stack | Evidence status |
|---|---|---|---|
| [AI Agency Lead Capture & Qualification](./01-ai-agency-lead-qualification/) | Lead capture, deterministic qualification, CRM logging, acknowledgement | n8n, Google Sheets, Gmail | Workflow export recovered and sanitized; five routing outcomes tested |
| [MedFlow Intake OS](./02-medflow-intake-os/) | Structured intake, deduplication, linked records, routing, audit logging | Jotform, Make.com, Airtable, Google Sheets | Client-style portfolio system using synthetic data; detailed implementation package recovered |
| [Cupid Errands Intelligent Email Routing](./03-cupid-intelligent-email-routing/) | AI intent classification, duplicate protection, department routing, Slack/email notifications | n8n, OpenRouter, Email, Slack | Structured project implementation with architecture evidence |
| [RAG & AI Agent Workflows](./04-rag-ai-agent-workflows/) | Document ingestion, embeddings, vector retrieval, agent memory | n8n, OpenRouter, OpenAI Embeddings, Supabase | Training implementation, explicitly labelled as such |
| [WhatsApp / Chatwoot CRM Automation](./05-whatsapp-chatwoot-crm/) | Messaging ingestion, webhook processing, contact extraction, CRM-style logging | n8n, Chatwoot, WhatsApp, Google Sheets, Docker | Independent portfolio/development implementation |
| [AI-Assisted Support with Human Review](./06-ai-support-human-review/) | Knowledge retrieval, AI response drafting, approval boundary, CRM follow-up | LLM workflow, Gmail, HubSpot | Independent portfolio pattern |
| [Self-Hosted n8n Platform](./07-self-hosted-n8n-platform/) | Automation platform hosting and operational infrastructure | Docker, PostgreSQL, Redis, Traefik, HTTPS | Independent infrastructure implementation |

## Standalone automation repository

### WhatsApp AI Order Processor

A separate, fully packaged n8n portfolio repository demonstrating WhatsApp order intake, AI-assisted order parsing, payment-flow design, fulfilment notification, and an importable demo workflow.

**Repository:** https://github.com/Dudubynatur3/whatsapp-order-processor

It remains standalone rather than being duplicated here because it already has its own workflow JSON, screenshot, detailed README, and setup documentation.

## Commercial production case study

### YTRanker SaaS Platform Engineering

YTRanker is treated separately from these public workflow projects because it involved private production code. Portfolio evidence focuses on the engineering work rather than exposing proprietary source code.

Key validated scope includes:

- React, Supabase, and Vercel production platform work
- Gmail OAuth, Telegram, WhatsApp, OpenRouter, Anthropic, and external integrations
- AI-provider migration to OpenRouter
- Role-based permissions and operational workflow controls
- Regression testing across **6 user roles**
- Validation of **40+ feature branches** before handover
- Full technical handover documentation

## Related Cloud / DevOps work

The automation projects are backed by hands-on cloud and platform engineering work across Terraform, GCP, AWS, Azure, Docker, Kubernetes, GitHub Actions, Ansible, Linux, IAM, and cloud networking.

See the public repositories on my GitHub profile: https://github.com/Dudubynatur3

## Repository map

```text
ai-automation-portfolio/
├── 01-ai-agency-lead-qualification/
├── 02-medflow-intake-os/
├── 03-cupid-intelligent-email-routing/
├── 04-rag-ai-agent-workflows/
├── 05-whatsapp-chatwoot-crm/
├── 06-ai-support-human-review/
└── 07-self-hosted-n8n-platform/
```

## Contact

- LinkedIn: https://www.linkedin.com/in/akintade-aduroja
- GitHub: https://github.com/Dudubynatur3
- Location: Kokkola, Finland

---

**Note:** Public workflow artifacts are intentionally sanitized. Any placeholders must be replaced with the user's own configuration after import.
