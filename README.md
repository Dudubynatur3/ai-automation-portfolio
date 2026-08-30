# AI Automation Portfolio

A curated collection of automation and AI workflow projects by **Aduroja Akintade**, focused on reliable business-process automation, integrations, AI-assisted workflows, and the infrastructure that supports them.

This repository complements my Cloud/DevOps repositories by documenting the automation side of my engineering work in an inspectable format: business problem, system architecture, implementation decisions, testing evidence, and selected sanitized implementation evidence where appropriate.

## Portfolio principles

- **Business problem first.** Each project explains the operational problem before the tooling.
- **Evidence over claims.** Architecture, test records, screenshots, routing logic, technical decisions, and selected sanitized implementation excerpts are published where useful.
- **Evidence-first, not turnkey.** Complete reusable workflow exports are not the default public artifact. Full exports are reserved for intentionally open demo/sample projects.
- **Clear implementation status.** Commercial, independent portfolio, client-style synthetic-data, and training implementations are labelled separately.
- **Security by default.** Credentials, production webhook URLs, private document IDs, customer data, secrets, and proprietary implementation details are excluded from public artifacts.
- **Reliability matters.** Routing rules, fallbacks, duplicate protection, human review, error handling, and operational handoff are treated as part of the system design.

For the exact publication state of each project, see [EVIDENCE_STATUS.md](./EVIDENCE_STATUS.md). Public-artifact rules are documented in [SECURITY.md](./SECURITY.md).

## Featured automation systems

| Project | Focus | Stack | Evidence status |
|---|---|---|---|
| [AI Agency Lead Capture & Qualification](./01-ai-agency-lead-qualification/) | Lead capture, deterministic qualification, CRM logging, acknowledgement | n8n, Google Sheets, Gmail | Architecture, routing logic and five-outcome test evidence published; complete reusable export intentionally withheld |
| [MedFlow Intake OS](./02-medflow-intake-os/) | Structured intake, deduplication, linked records, routing, audit logging | Jotform, Make.com, Airtable, Google Sheets | Client-style portfolio system using synthetic data; detailed implementation package recovered |
| [Cupid Errands Intelligent Email Routing](./03-cupid-intelligent-email-routing/) | AI intent classification, duplicate protection, department routing, Slack/email notifications | n8n, OpenRouter, Email, Slack | Structured project implementation with architecture evidence |
| [RAG & AI Agent Workflows](./04-rag-ai-agent-workflows/) | Document ingestion, embeddings, vector retrieval, agent memory | n8n, OpenRouter, OpenAI Embeddings, Supabase | Training implementation, explicitly labelled as such |
| [WhatsApp / Chatwoot CRM Automation](./05-whatsapp-chatwoot-crm/) | Messaging ingestion, webhook processing, contact extraction, CRM-style logging | n8n, Chatwoot, WhatsApp, Google Sheets, Docker | Independent portfolio/development implementation |
| [AI-Assisted Support with Human Review](./06-ai-support-human-review/) | Knowledge retrieval, AI response drafting, approval boundary, CRM follow-up | LLM workflow, Gmail, HubSpot | Independent portfolio pattern |
| [Self-Hosted n8n Platform](./07-self-hosted-n8n-platform/) | Automation platform hosting and operational infrastructure | Docker, PostgreSQL, Redis, Traefik, HTTPS | Independent infrastructure implementation |

## Evidence publication policy

The goal of this repository is to make engineering ability inspectable without turning every project into a copy-and-deploy package.

Public project evidence can include:

- business problem and system architecture
- workflow/node maps and routing rules
- screenshots and execution evidence
- test cases and validated outcomes
- selected sanitized configuration or implementation excerpts
- reliability, security, fallback, and handoff decisions

Complete reusable workflow exports are published only when the project is deliberately an open demo/sample. Commercial/private implementations remain case-study only.

## Standalone automation repository

### WhatsApp AI Order Processor

A separate, intentionally open **DEMO MODE** n8n portfolio repository demonstrating WhatsApp order intake, AI-assisted order parsing, payment-flow design, fulfilment notification, and an importable demo workflow using mocked/simulated external integrations.

**Repository:** https://github.com/Dudubynatur3/whatsapp-order-processor

It remains standalone rather than being duplicated here because it is deliberately a reusable sample and already has its own workflow JSON, screenshot, detailed README, and setup documentation.

## Commercial production case study

### YTRanker SaaS Platform Engineering

YTRanker is treated separately from these public workflow projects because it involved private production code. Portfolio evidence focuses on the engineering work rather than exposing proprietary source code.

Key validated scope includes:

- React, Supabase, and Vercel production platform work
- Gmail OAuth, Telegram, WhatsApp, OpenRouter, Anthropic, and external integrations
- AI-provider migration to OpenRouter
- role-based permissions and operational workflow controls
- regression testing across **6 user roles**
- validation of **40+ feature branches** before handover
- full technical handover documentation

Read the public case study: [commercial-case-studies/ytranker.md](./commercial-case-studies/ytranker.md)

Public Upwork profile for work-history verification: https://www.upwork.com/freelancers/~01c8ba1b4d2162d9f1?mp_source=share

## Related Cloud / DevOps work

The automation projects are backed by hands-on cloud and platform engineering work across Terraform, GCP, AWS, Azure, Docker, Kubernetes, GitHub Actions, Ansible, Linux, IAM, and cloud networking.

See the public repositories on my GitHub profile: https://github.com/Dudubynatur3

## Repository map

```text
ai-automation-portfolio/
├── README.md
├── EVIDENCE_STATUS.md
├── SECURITY.md
├── 01-ai-agency-lead-qualification/
│   ├── README.md
│   ├── TESTING.md
│   └── workflow/
│       └── README.md
├── 02-medflow-intake-os/
├── 03-cupid-intelligent-email-routing/
├── 04-rag-ai-agent-workflows/
├── 05-whatsapp-chatwoot-crm/
├── 06-ai-support-human-review/
├── 07-self-hosted-n8n-platform/
└── commercial-case-studies/
    └── ytranker.md
```

## Contact

- Portfolio: https://aduroja-akintade.lovable.app
- LinkedIn: https://www.linkedin.com/in/akintade-aduroja
- GitHub: https://github.com/Dudubynatur3
- Upwork: https://www.upwork.com/freelancers/~01c8ba1b4d2162d9f1?mp_source=share
- Location: Kokkola, Finland

---

**Note:** Public evidence is intentionally sanitized and scoped. A project being inspectable does not mean the complete reusable implementation is published.