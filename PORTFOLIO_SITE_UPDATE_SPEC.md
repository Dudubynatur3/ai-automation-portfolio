# Portfolio Site Update Specification

This document defines the evidence and content rules for the published engineering portfolio at:

**https://aduroja-akintade.lovable.app**

## Keep the current visual system

The site already has a strong visual identity:

- cream / black / lime palette
- large editorial typography
- clear systems-engineering positioning
- distinct production-experience section
- direct GitHub / LinkedIn / email calls to action

A rebuild in another website builder is not required. The priority is evidence accuracy, stronger automation representation, and a non-turnkey public evidence policy.

## 1. Hero section

Keep:

> I engineer the systems behind the outcome.

Keep the supporting positioning around AI Automation with a Cloud / DevOps foundation.

Recommended metric block:

| Metric | Value |
|---|---:|
| Automation systems documented | 7 |
| Cloud platforms | 3 |
| Feature branches validated | 40+ |
| User roles regression tested | 6 |

## 2. Featured work

Featured cards should prioritise clearly authored, inspectable evidence.

### Featured card 1

**AI Agency Lead Capture & Qualification**  
Category: AI Automation  
Stack: n8n, Google Sheets, Gmail  
Proof: five tested routing outcomes, architecture, qualification logic, data contract, and sanitized implementation evidence  
Link: `https://github.com/Dudubynatur3/ai-automation-portfolio/tree/main/01-ai-agency-lead-qualification`

Suggested summary:

> Deterministic lead qualification system that classifies enquiries by timeline and budget, records the final status in Google Sheets, and triggers immediate customer acknowledgement. Five final routing outcomes were tested.

**Important:** Do not advertise a full public/importable n8n JSON for this project. The complete reusable export is intentionally withheld from the current public branch.

### Featured card 2

**WhatsApp AI Order Processor**  
Category: AI Automation  
Stack: n8n, Twilio pattern, OpenAI, Google Sheets, Stripe pattern, Telegram  
Proof: detailed README, workflow screenshot, importable demo JSON  
Link: `https://github.com/Dudubynatur3/whatsapp-order-processor`

Keep the repository's explicit **DEMO MODE** wording so mocked integrations are not represented as live commercial integrations. This intentionally open sample is the exception where a reusable workflow export is appropriate.

### Featured card 3

**AWS High-Availability 3-Tier System**  
Category: Cloud Infrastructure  
Stack: AWS, Terraform, EC2, ALB, RDS MySQL, NAT Gateway, Nginx, Next.js  
Link: `https://github.com/Dudubynatur3/aws-3tier-terraform-nextjs`

Reasons to feature:

- original repository, not a fork
- clear architecture documentation
- three network tiers
- public and internal ALBs
- RDS Multi-AZ and read replica
- infrastructure teardown guidance
- screenshots and troubleshooting evidence already present

## 3. Cloud supporting work

Immediately below the three headline cards, surface a compact Cloud / DevOps row with:

### GCP End-of-Training Terraform Project

Link: `https://github.com/Dudubynatur3/gcp-exercise`

Evidence includes Terraform VPC/subnets, Compute Engine, IAM, Linux, Flask, Cloud SQL, GKE, GCP folder hierarchy, and hands-on screenshots.

### EpicBook Full-stack Infrastructure

Link: `https://github.com/Dudubynatur3/epicbook-fullstack`

Evidence includes Azure, Terraform, Ansible, Nginx, and infrastructure automation.

### Automated Developer Onboarding

Link: `https://github.com/Dudubynatur3/dev-onboarding-automation`

Evidence includes Terraform, AWS, Bash, Linux user/group management, and repeatable onboarding automation.

## 4. Authorship exclusions

### `3-Tier-MERN-App`

This repository was only forked and no personal implementation work was performed in it.

**Decision: do not present it as personal engineering evidence.**

### `Azure-Terraform-Project`

This was a collaborative Cloud Advisory group project, with the shared repository created by another participant. Aduroja Akintade completed an assigned contribution but the repository is not independently authored.

**Decision: do not feature it as independently authored work.**

It may be mentioned only as collaborative training experience if the personal contribution is described precisely.

## 5. AI Automation Systems section

Heading:

> AI automation systems.  
> Built around operational failure points.

Include:

1. AI Agency Lead Capture & Qualification
2. MedFlow Intake OS
3. Cupid Errands Intelligent Email Routing
4. RAG & AI Agent Workflows
5. WhatsApp / Chatwoot CRM Automation
6. AI-Assisted Customer Support with Human Review
7. Self-Hosted n8n Platform
8. WhatsApp AI Order Processor, linked to its standalone repository

Each item should expose:

- business problem
- workflow architecture
- stack
- implementation classification
- evidence link
- testing / control evidence

Do not imply that every evidence link contains a complete reusable workflow export.

## 6. MedFlow wording

The connected Airtable base is the strongest data-model source of truth and directly confirms a **six-table relational system**:

- `Patients`
- `Intakes`
- `Cases`
- `Tasks`
- `Routing_Log`
- `Staff`

Correct public evidence:

- Jotform → Make.com → Airtable → Google Sheets → Gmail/Outlook → Google Calendar
- duplicate checking using email with normalized-phone fallback
- patient create/update plus separate intake records
- case creation from routed intakes
- task generation and staff assignment
- relational links across patients, intakes, cases, tasks, routing logs, and staff
- synthetic data only
- HIPAA-aware design discussion, not HIPAA compliance
- append-oriented audit logging
- consent and missing-data routing controls
- masked identifiers in routing/audit evidence

The earlier four-table note came from an incomplete documentation snapshot and should no longer be used for the portfolio or CVs.

Detailed schema evidence: `02-medflow-intake-os/DATA_MODEL.md`.

## 7. Production experience: YTRanker

Keep:

- private production code label
- March 2026 to July 2026 timeframe
- React, Supabase, Vercel platform context
- 40+ feature branches validated
- 6 user roles regression tested
- technical handover
- verified client-feedback wording

Public case study:

`https://github.com/Dudubynatur3/ai-automation-portfolio/blob/main/commercial-case-studies/ytranker.md`

Public Upwork profile:

`https://www.upwork.com/freelancers/~01c8ba1b4d2162d9f1?mp_source=share`

### Required site improvement

Near the YTRanker client-feedback quote or case-study CTA, add a visible secondary link/button:

> **Verify on Upwork**

or

> **View Upwork profile**

The link should open in a new tab. Do not state that the portfolio independently verified the Upwork page. Explain only that recruiters/clients can inspect the public freelancer profile and available work-history evidence there.

Also add **Upwork** alongside GitHub, LinkedIn, and Email in the final contact/social surface.

Do not link to the private YTRanker source repository.

## 8. Evidence publication policy

The site should make the public-evidence philosophy clear without sounding defensive.

Recommended concise wording:

> Public case studies expose architecture, screenshots, test results, selected sanitized implementation evidence, and technical decisions. Complete reusable workflow exports are published only for intentionally open demo projects. Commercial/private implementations remain case-study only.

This policy applies across the portfolio.

For the AI Agency project, remove any visible wording such as:

- `public portfolio-safe n8n JSON`
- `importable workflow`
- `complete workflow export`

Replace with:

- architecture
- routing logic
- test evidence
- sanitized implementation excerpts/evidence

The WhatsApp AI Order Processor remains the explicit intentionally open DEMO MODE exception.

## 9. Working philosophy

Keep:

> Automation is useful. Reliability is the product.

Supporting copy should explicitly mention:

- deterministic logic where AI is unnecessary
- AI classification where interpretation is required
- fallbacks and human review
- deduplication
- auditability
- testing
- documentation and handover

## 10. Repository hierarchy

Prominently link:

`https://github.com/Dudubynatur3/ai-automation-portfolio`

Use four evidence tiers:

### Featured authored systems
High-confidence, inspectable work.

### Supporting authored repositories
Smaller app/infrastructure repositories supporting the engineering history.

### Collaborative training work
Group work with the user's own contribution described precisely.

### Forks / references
Not used as personal engineering evidence unless an independent contribution is explicitly documented.

See `CLOUD_REPOSITORY_AUDIT.md` for the current classification.

## 11. Navigation

Keep:

- Work
- Experience
- About
- Let's talk

Within Work, use:

`All | AI Automation | Cloud / DevOps | SaaS & Integrations`

## 12. Final publication gate

Before treating a site revision as complete:

- verify every project link
- keep the 3-Tier-MERN fork out of personal work
- keep the Azure group-project fork out of Featured Work
- retain the AI Automation Portfolio link
- test mobile layout
- test every CTA
- confirm email / LinkedIn / GitHub links
- add and test the Upwork verification link
- verify no screenshot exposes credentials or customer data
- ensure project classifications are visible
- ensure MedFlow is consistently described as the verified six-table implementation
- ensure AI Agency no longer advertises a full reusable JSON/workflow export
- keep WhatsApp AI Order Processor clearly labelled as the intentionally open DEMO MODE exception
